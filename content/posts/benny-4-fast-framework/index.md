+++
date = '2025-09-30T15:44:06+09:00'
draft = false # Change to false to publish
title = '베니, 템플릿 프레임워크를 만들어라.'
description = '속도는 생명' # post's summary or description
tags = ['svelte', 'framework']
authors = ['benny']
featured_image = '001.png' # e.g. '001.png'
slug = 'fast-svelte-framework' # uri. e.g. 'awesome-post-name'
audio = []
vedios = []
series = []
images = ['001.Png']
+++

![](./001.png)

얼마전에 이런 과제가 있었습니다.

"기본적인 기능들이 포함되어 있고 빠르게 프로젝트를 시작할 수 있는 프레임워크가 필요합니다."

다시 말해 프론트와 백엔드를 아우를 수 있는 풀스택 프레임워크이고,
환경 변수만 바꿔주면 결제와 OAuth2 로그인이 가능하게끔 할 수 있는 그런 작업을 맡게 됐습니다.

## 풀스택 프레임워크 선택

먼저 Next JS가 생각났습니다.

지금같은 AI 시대에는 Next JS를 선택하는 것이 굉장히 유리하다고 생각합니다.
코드도 많고 사용하는 사람이 많기 때문에 공략법이 많이 나와있는 루트를 선택하는 것 같은 느낌입니다.

하지만 저에게는 Next JS는 개발 경험이 아주 별로입니다.
너무 느리고 메모리를 아주 많이 잡아먹습니다.

![](./002.png)

레딧에서도 종종 관련 글이 올라오는 정도입니다.
Next JS가 느린 이유는 그 동작 원리에 있으나 이 글에서 다룰 이야기는 아니기에 패스하겠습니다.

이후 많은 고민끝에 기본적으로 선언형으로 프로그래밍이 가능하고 React와 크게 다르지 않은 **SvelteKit**으로 결정했습니다.

## 선택한 기술 스택

최종적으로 선택한 기술 스택은 다음과 같습니다:

- **프론트엔드**: SvelteKit + TypeScript
- **데이터베이스**: MongoDB
- **ORM**: Prisma
- **인증**: OAuth 2.0 기반 소셜 로그인 (Google, GitHub, Facebook)
- **분석**: Google Analytics
- **결제**: Paddle

## 환경변수만 바꾸면 동작하게끔

```env
# This is an example file. Copy this to .env and fill in your actual values.
# Do NOT commit your .env file to version control.

# --- MongoDB Docker Script Settings ---
# These variables are used by the scripts in the /scripts directory.
MONGO_CONTAINER_NAME=mongodb
MONGO_PORT=27017
MONGO_INITDB_ROOT_USERNAME=root
MONGO_INITDB_ROOT_PASSWORD=your_secret_password_here
MONGO_REPLICA_SET_NAME=rs0
MONGO_IMAGE=mongo:latest

# --- Application Database Settings ---
# This is the database your SvelteKit application will connect to.
# For consistency, it should be constructed from the variables above.
DB_NAME=example
DATABASE_URL="mongodb://${MONGO_INITDB_ROOT_USERNAME}:${MONGO_INITDB_ROOT_PASSWORD}@localhost:${MONGO_PORT}/${DB_NAME}?authSource=admin&replicaSet=${MONGO_REPLICA_SET_NAME}"

# GOOGLE
GOOGLE_CLIENT_ID="YOUR_GOOGLE_CLIENT_ID"
GOOGLE_CLIENT_SECRET="YOUR_GOOGLE_CLIENT_SECRET"

# GITHUB
GITHUB_CLIENT_ID="YOUR_GITHUB_CLIENT_ID"
GITHUB_CLIENT_SECRET="YOUR_GITHUB_CLIENT_SECRET"

# GA TAG
PUBLIC_GA_MEASUREMENT_ID=G-XXXXXXXXXX

# PADDLE TOKEN
PUBLIC_PADDLE_TOKEN=test_XXXXXXXXXXXXXXXXXXXXXXXXXXX
PADDLE_WEBHOOK_SECRET=
PADDLE_API_KEY=
```

위는 사용자가 입력해야할 환경변수입니다.

환경변수만 변경하면 동작하게끔 되어있지만, 각 사이트에 가서 직접 찾아서 입력해야하는 문제는 어쩔 수가 없습니다.

## 데이터베이스

초기에 데이터베이스를 구축하는 것은 정말 귀찮은 일입니다

그래서 저는 직접 DB를 띄우는 것보다는 도커를 이용해서 띄우는 것을 선호하는 편입니다.
그런데 터미널에 직접 도커 명령어를 입력하는 것조차도 정말 정말 귀찮은 일이죠

따라서 저는 거의 모든 프로젝트를 궁극의 딸깍 스크립트를 작성하곤 합니다.
아래는 DB를 초기화하는 쉘 스크립트입니다.

```shell
#!/bin/bash
set -e
cd "$(dirname "$0")"

# --- MongoDB 키 파일 확인 및 생성 ---
KEY_FILE_PATH="../mongo-key/mongodb.key"
MONGO_KEY_DIR="../mongo-key"

echo "--- Checking for MongoDB key file ---"
# mongo-key 디렉토리가 없으면 생성
if [ ! -d "$MONGO_KEY_DIR" ]; then
    echo "Directory '$MONGO_KEY_DIR' not found. Creating it..."
    mkdir -p "$MONGO_KEY_DIR"
fi

# 키 파일이 없으면 생성
if [ ! -f "$KEY_FILE_PATH" ]; then
    echo "MongoDB key file not found. Generating a new key..."
    openssl rand -base64 756 > "$KEY_FILE_PATH"
    chmod 400 "$KEY_FILE_PATH"
    echo "New key file created and permissions set to 400."
else
    echo "Key file already exists. Skipping generation."
fi
# --- 키 파일 확인 종료 ---

# 스크립트 시작 시, 기존 컨테이너가 있다면 먼저 정리합니다.
echo "--- Ensuring previous container is stopped and removed ---"
bash ./stop-mongo.sh
echo "--- Cleanup finished. Pausing for 2 seconds before restart... ---"
sleep 2 # OS가 네트워크 포트를 완전히 해제할 시간을 줍니다.

# .env 파일이 있으면 환경변수를 로드합니다.
if [ -f ../.env ]; then
  set -a # 자동으로 모든 변수를 export 합니다.
  source ../.env
  set +a
else
  echo "오류: .env 파일을 찾을 수 없습니다. 스크립트를 실행하기 전에 .env 파일을 생성하고 필요한 변수를 설정해주세요."
  exit 1
fi

# 필수 환경변수가 설정되었는지 확인하고, 없으면 에러를 발생시킵니다.
: ${MONGO_CONTAINER_NAME:?오류: MONGO_CONTAINER_NAME 변수가 .env 파일에 설정되어야 합니다.}
: ${MONGO_PORT:?오류: MONGO_PORT 변수가 .env 파일에 설정되어야 합니다.}
: ${MONGO_INITDB_ROOT_USERNAME:?오류: MONGO_INITDB_ROOT_USERNAME 변수가 .env 파일에 설정되어야 합니다.}
: ${MONGO_INITDB_ROOT_PASSWORD:?오류: MONGO_INITDB_ROOT_PASSWORD 변수가 .env 파일에 설정되어야 합니다.}
: ${MONGO_REPLICA_SET_NAME:?오류: MONGO_REPLICA_SET_NAME 변수가 .env 파일에 설정되어야 합니다.}

# 프로젝트 루트 디렉토리의 절대 경로를 구합니다.
PROJECT_ROOT=$(cd .. && pwd)

# MongoDB 컨테이너를 시작합니다.
echo "Starting MongoDB container (${MONGO_CONTAINER_NAME})..."
docker run -d --name ${MONGO_CONTAINER_NAME} -p ${MONGO_PORT}:${MONGO_PORT} -v "${PROJECT_ROOT}/mongodb_data:/data/db" -v "${PROJECT_ROOT}/mongo-key/mongodb.key:/auth/mongodb.key" -e MONGO_INITDB_ROOT_USERNAME=${MONGO_INITDB_ROOT_USERNAME} -e MONGO_INITDB_ROOT_PASSWORD=${MONGO_INITDB_ROOT_PASSWORD} mongo:latest --replSet ${MONGO_REPLICA_SET_NAME} --keyFile /auth/mongodb.key

# MongoDB 컨테이너가 시작되고 연결을 받을 준비가 될 때까지 잠시 대기합니다.
echo "Waiting for MongoDB to be ready..."
sleep 5

# Docker 컨테이너 내부에서 mongosh를 실행하여 레플리카 셋을 초기화합니다.
echo "Initiating MongoDB replica set..."
docker exec ${MONGO_CONTAINER_NAME} mongosh -u "${MONGO_INITDB_ROOT_USERNAME}" -p "${MONGO_INITDB_ROOT_PASSWORD}" --authenticationDatabase admin --eval "rs.initiate({ _id: '${MONGO_REPLICA_SET_NAME}', members: [{ _id: 0, host: 'localhost:${MONGO_PORT}' }] })"

echo "Replica set initiated successfully."

echo "--- Applying Prisma schema to the database ---"
cd .. && npx prisma db push

echo "--- MongoDB setup complete ---"
```

그리고 이 기능은 package.json의 scripts로 사용되고 있습니다.

```json
{
  ...
  "scripts": {
    ...
		"db:start": "bash scripts/init-mongo.sh",
		"db:stop": "bash scripts/stop-mongo.sh"
  }
}
```

## 사용법

이제 종합적으로 봤을 때 이 템플릿 프레임워크를 사용한 개발 모드를 올리는 방법은 다음과 같습니다.

1. git clone [템플릿_레포지토리]
2. cd [템플릿_레포지토리]
3. pnpm install --frozen-lockfile
4. cp .env.example .env
5. 환경변수 작성
6. pnpm db:start
7. pnpm dev

## 결론

![](003.gif)

위의 화면과 같이 로그인 및 결제 연동이라는 번거로운 작업을 템플릿으로 만들어서 쉽게 사용할 수 있게 되었습니다.

근데 솔직히 사용법이 너무 길고 귀찮습니다.
아무래도 전용 CLI를 만들어서 과정을 명령어 하나로 딸깍 할 수 있는 시스템을 만들어야 할 것 같습니다.

그리고 Google, Paddle, Github, Facebook, GA Tag 환경 변수를 한번에 호출해서 바로 적용만 하면 되게끔 만들면
그제서야 템플릿 프레임워크라고 할 수 있지 않을까요?

아무래도 성국님한테 건의를 드려야할 것 같습니다.

만약 성국님이 허락한다면 전용 라이브러리를 만들고 템플릿 프레임워크 2편으로 돌아오겠습니다.
