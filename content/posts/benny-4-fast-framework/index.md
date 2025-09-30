+++
date = '2025-09-30T15:44:06+09:00'
draft = false # Change to false to publish
title = '빠르게 프로젝트를 시작하기 위하여'
description = '속도는 생명' # post's summary or description
tags = ['svelte', 'framework']
authors = ['benny']
featured_image = 'thumbnail.gif' # e.g. 'thumbnail.png'
slug = 'fast-svelte-framework' # uri. e.g. 'awesome-post-name'
audio = []
vedios = []
series = []
images = ['thumbnail.gif']
+++

![](./thumbnail.gif)

얼마전에 이런 과제가 있었습니다.

"기본적인 기능들이 포함되어 있고 빠르게 프로젝트를 시작할 수 있는 프레임워크가 필요합니다."

다시 말해 프론트와 백엔드를 아우를 수 있는 풀스택 프레임워크이고,
환경 변수만 바꿔주면 결제와 OAuth2 로그인이 가능하게끔 할 수 있는 그런 작업을 맡게 됐습니다.

![](./001.png)

## 풀스택 프레임워크 선택

먼저 Next JS가 생각났습니다.

지금같은 AI 시대에는 Next JS를 선택하는 것이 굉장히 유리하다고 생각합니다.
코드도 많고 사용하는 사람이 많기 때문에 공략법이 많이 나와있는 루트를 선택하는 것 같은 느낌입니다.

하지만 저에게는 Next JS는 개발 경험이 아주 별로입니다.
너무 느리고 메모리를 아주 많이 잡아먹습니다.

![](./002.png)

레딧에서도 종종 관련 글이 올라오는 정도입니다.
Next JS가 느린 이유는 그 동작 원리에 있으나 이 글에서 다룰 이야기는 아니기에 패스하겠습니다.

이후 많은 고민끝에 기본적으로 선언형으로 프로그래밍이 가능하고 React에서 크게 변형된 사용이 아닌 **SvelteKit**으로 결정했습니다.

## 선택한 기술 스택

최종적으로 선택한 기술 스택은 다음과 같습니다:

- **프론트엔드**: SvelteKit + TypeScript
- **데이터베이스**: MongoDB
- **ORM**: Prisma
- **인증**: OAuth 2.0 기반 소셜 로그인 (Google, GitHub, Facebook)
- **분석**: Google Analytics
- **결제**: Paddle

## 왜 이 스택을 선택했나?

### SvelteKit + TypeScript

SvelteKit은 컴파일 타임에 최적화되어 런타임 오버헤드가 거의 없습니다.
React의 복잡한 상태 관리나 Virtual DOM 없이도 빠르고 직관적인 개발이 가능합니다.

```javascript
// SvelteKit의 간단한 상태 관리
let count = 0;
$: doubled = count * 2;

function increment() {
  count += 1;
}
```

### MongoDB + Prisma

MongoDB는 NoSQL의 유연성을 제공하면서도 Prisma를 통해 타입 세이프한 데이터베이스 접근이 가능합니다.

```javascript
// Prisma 스키마 예시
model User {
  id        String    @id @default(auto()) @map("_id") @db.ObjectId
  email     String    @unique
  username  String
  paddleCustomerId String? @unique
  accounts  Account[]
  sessions  Session[]
}

model Account {
  id                String  @id @default(auto()) @map("_id") @db.ObjectId
  userId            String  @db.ObjectId
  provider          String
  providerAccountId String
  avatar_url        String?

  user User @relation(fields: [userId], references: [id], onDelete: Cascade)

  @@unique([provider, providerAccountId])
}
```
