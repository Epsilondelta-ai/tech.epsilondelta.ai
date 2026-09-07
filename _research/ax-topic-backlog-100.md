# 기업 AX 테크블로그 주제 100선

조사 기준일: 2026-09-07

기업의 AX를 상위 카테고리로 두고, **각각 독립적으로 읽을 수 있는 포스트 100개**를 기획했다. 주요 독자는 AI·AX에 관심 있는 경영진과 사업·현업 책임자다. 기술을 설명할 때는 그 기술이 바꾸는 업무, 투자 판단, 운영 책임까지 연결한다. 도메인은 영업·재무·인사 같은 업무 기능과 제조·금융·의료 같은 산업을 모두 포함한다.

기존 「AX는 암묵지를 자산화할 수 있어야 성공합니다」, 「AI 에이전트 엔지니어링 겉핥기」, 「Context Graph란?」의 개론을 토대로, 실제 도입과 운영에서 부딪히는 문제로 범위를 넓혔다. 생성형 AI와 에이전트뿐 아니라 예측·최적화·비전 AI도 본업을 바꾸는 데 필요한 경우 포함했다.

해외 개념 소개 후보와 에이전트 구성 요소도 100개 안에 포함했다. 문서 후반의 별도 색인에서 해당 주제를 모아 볼 수 있다.

## 선정 기준과 읽는 법

- 포스트마다 경영진이나 현업 책임자가 판단할 질문 하나를 중심에 둔다.
- 같은 기술이라도 비용·품질·권한·인력 등 의사결정이 다를 때만 별도 주제로 선정한다.
- 실제 도입 사례, 연구·조사, 기술 문서, 법령을 구분한다. **아래 제목과 설명은 자료를 바탕으로 한 편집 제안**이며, 기술 문서에 연결한 업무 예시는 도입 실적을 뜻하지 않는다.
- 사례는 기업·공급사가 공개한 범위에서 활용한다. 파일럿·계획은 해당 상태를 표시했으며, 한 기업의 결과를 모든 기업의 예상 성과로 바꾸지 않는다.
- 기본 형식은 단독 포스트다. 설명이 길어지는 주제만 문서 후반의 제안처럼 2~3편으로 나눈다.

| 구분 | 주제 번호 | 주요 관심사 |
|---|---|---|
| A. AX 전략과 투자 판단 | 001–010 | 첫 과제, ROI, 투자 우선순위, 도입 방식 |
| B. 조직·인재·일하는 방식 | 011–020 | 책임자, 교육, 직무 변화, 현업 참여 |
| C. 데이터·지식·조직의 기억 | 021–030 | 검색, 데이터 의미, 최신성, 피드백, 업무 관찰 |
| D. 기술 트렌드와 구성 선택 | 031–040 | 범용 에이전트, MCP·A2A, 작은 모델, Computer Use, Physical AI |
| E. 평가·운영·비용 관리 | 041–050 | 업무 완료, 품질 검증, 장애 대응, 비용과 성능 |
| F. 거버넌스·보안·규제 | 051–060 | 책임·승인·감사, 개인정보, 국내외 규제, 보안 |
| G. 영업·마케팅·고객 경험 | 061–070 | 상담, 영업 기회, CRM, 콘텐츠, 개인화, 신사업 |
| H. 재무·구매·법무·인사·IT | 071–080 | 숫자 검증, 미수금, 계약, 협상, HR, 레거시 |
| I. 제조·공급망·물류·건설·에너지 | 081–090 | 품질, 조업, 설비, 재고, 납기, 현장 운영 |
| J. 금융·보험·의료·제약·공공·서비스 | 091–100 | 산업별 전문 판단, 고객 접점, 규제와 서비스 변화 |

## A. AX 전략과 투자 판단

독자: CEO, COO, CFO, 전략·사업개발 책임자.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 001 | AI로 시간을 아꼈는데 회사 이익은 왜 그대로일까? | 개인의 시간 절약이 처리량·고객 서비스·매출로 이어지는 조건을 살핀다. 현장 실험과 기업 설문을 비교해 생산성의 측정 단위를 설명한다. | 실험·[NBER][nber-workplace], 조사·[McKinsey 2026][mckinsey] |
| 002 | AI가 잘하는 일의 경계는 고르지 않습니다: 첫 AX 과제 선정 | Jagged Technological Frontier를 바탕으로 비슷해 보이는 과업의 AI 성과가 다른 이유를 설명한다. 실제 업무 시험과 병목·비용을 함께 보며 첫 과제를 고른다. | 현장 실험 논문·[Jagged Technological Frontier][jagged], 조사·[WEF][wef-org] |
| 003 | 시범사업을 끝내는 법: 확대·개선·중단의 기준 | 데모 이후 실제 사용, 품질, 운영 담당자, 총비용을 확인하는 기준을 제안한다. 성과가 부족한 실험에서도 재사용할 지식을 남기는 방법을 다룬다. | 조사·[WEF 조직 전환][wef-org] |
| 004 | 에이전트의 업무 명세서: 목표·완료 조건·중단 조건 | 프롬프트에 업무 목적, 입력 자료, 산출물, 해서는 안 되는 행동을 명시한다. ‘보고서 작성’과 ‘근거가 확인된 보고서 완성’의 차이를 예시로 설명한다. | 적용 설계·[Google Cloud][google-patterns], [업무 평가][evals] |
| 005 | AI를 직접 만들까, 사서 쓸까, 함께 만들까? | 기존 SaaS, 범용 에이전트의 사내 구성, 맞춤 개발을 비교한다. 개발비와 함께 통합·유지보수·데이터 이동 비용을 계산한다. | 조사·[McKinsey 2026][mckinsey], 비용 체계·[FinOps][finops] |
| 006 | 부서 하나의 자동화가 회사 전체를 느리게 만들 수도 있다 | 앞 단계의 산출물이 늘었을 때 검토·승인이 병목으로 옮겨가는 상황을 다룬다. 주문부터 현금 회수까지 전체 흐름을 기준으로 AX를 설계한다. | 사례·[Siemens 프로세스 분석][celonis], 실험·[NBER][nber-workplace] |
| 007 | 전담 AI팀 없는 중소기업의 AX 시작법 | 인력과 예산이 적은 조직에서 현업 담당자와 외부 파트너의 역할을 나누고, 반복 업무 하나를 운영 가능한 크기로 만드는 방법을 제안한다. | 중소기업 조사·[OECD][oecd-sme] |
| 008 | AX 사업계획서의 ‘절감 시간’을 돈으로 계산하는 법 | 여유 시간, 초과근무 감소, 추가 처리량, 채용 회피를 구분한다. 같은 시간을 인건비 절감과 매출 증가에 중복 반영하지 않는 계산법을 다룬다. | 비용 체계·[FinOps][finops], 노동시장 연구·[NBER][nber-labor] |
| 009 | AI를 쓴 만큼 낼까, 해결한 만큼 낼까? | 좌석·사용량·성과 기반 과금의 차이를 설명한다. ‘해결’과 ‘인계 완료’의 정의에 따라 구매자가 부담하는 비용과 위험이 달라지는 점을 짚는다. | 실제 제품 정책·[Intercom의 outcome 과금][intercom-outcomes] |
| 010 | CEO가 월간 AX 보고서에서 봐야 할 숫자 | 계정 수와 사용량에 더해 완료율·재작업·업무시간·매출 기여·운영비를 보는 성과표를 제안한다. 현업 지표와 전사 손익을 연결하는 데 초점을 둔다. | 조사·[McKinsey 2026][mckinsey], 비용 체계·[FinOps][finops] |

## B. 조직·인재·일하는 방식

독자: 경영진, HR, 부서장, AX 추진 조직. 기술 도입 뒤 실제로 누가 어떤 일을 맡는지 다룬다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 011 | AX의 주인은 IT 부서일까, 현업일까? | 공통 기술 기반, 업무 성과, 위험 관리의 책임을 나눈다. 중앙 전담팀과 부서별 담당자가 함께 일하는 구조를 설명한다. | 조사·[WEF 조직 전환][wef-org] |
| 012 | AI를 잘 쓰는 직원의 노하우를 전사로 퍼뜨리는 방법 | 현업 지원자, 업무별 예시, 동료 교육을 통해 개인의 활용법을 조직의 사용 방식으로 옮긴다. BBVA의 내부 확산 활동을 출발점으로 삼는다. | 사례·[BBVA][bbva] |
| 013 | AI가 들어오면 직무기술서부터 다시 써야 할까? | 직업 전체를 대체 대상으로 보기보다 조사·판단·작성·승인 같은 과업을 나눈다. 사람에게 남길 책임과 AI 감독 업무까지 직무에 반영한다. | 연구·[ILO 직무 노출 분석][ilo], [NBER 업무 재조직 연구][nber-labor] |
| 014 | AI 시대의 신입 교육: 일을 잘 끝내는 것과 배우는 것 | AI가 만든 결과를 검토·수정·설명하는 과정을 온보딩에 넣는다. AI를 잠시 끈 상태에서도 지식이 남는지 확인하는 교육 평가를 제안한다. | 업무형 과제 실험·[NBER][nber-learning] |
| 015 | FDE란? AI 엔지니어가 고객 현장으로 들어가는 이유 | Forward Deployed Engineer가 실제 데이터·업무 예외를 파악하고 구현·통합·운영을 잇는 역할임을 설명한다. 이런 역할의 채용·육성·외부 협업을 검토한다. | 역할·사업 발표·[Palantir][fde-palantir], [AWS][fde-aws], 국내 인력 연구·[한국은행][bok-talent] |
| 016 | AI 교육의 성과를 수강률로만 재면 놓치는 것 | 교육 이후 업무 적용, 사용 지속, 오류 발견, 결과물 품질을 평가한다. 일반 프롬프트 강의에서 업무별 실습으로 옮기는 방법을 다룬다. | 조사·[OECD 중소기업 준비도][oecd-training] |
| 017 | Workslop: 내가 아낀 시간이 동료의 재작업이 된다면 | 그럴듯하지만 업무를 진전시키지 못하는 AI 산출물을 다룬다. 작성자에게 절약된 시간과 수신자의 해석·검증·수정 부담을 함께 측정하는 방법을 제안한다. | 설문 연구·[BetterUp·Stanford 연구팀][workslop] |
| 018 | 업무를 관찰하는 AI와 직원 감시의 경계 | 암묵지를 수집하는 화면·대화·행동 기록에서 목적, 수집 범위, 열람자, 보관 기간을 정하는 방법을 다룬다. 직원의 참여와 신뢰를 함께 살핀다. | 공식 지침·[개인정보보호위원회][pipc], 연구·[ILO][ilo] |
| 019 | 직원들은 이미 AI를 쓰고 있습니다: Shadow AI 대응 | 비공식 사용 현황을 파악하고 허용 도구·데이터 기준·도움받을 창구를 마련한다. 개인 활용률과 회사의 공식 도입률을 구분해 설명한다. | 국내 조사·[한국은행 AI 활용][bok-adoption], 공식 지침·[개인정보보호위원회][pipc] |
| 020 | 현업이 직접 만든 AI 도구의 운영자는 누구일까? | 직원이 만든 업무 도구에 소유자, 검증 기준, 변경 이력, 퇴사 시 인계 방법을 붙인다. 시민 개발이 늘어날 때 생기는 운영 문제를 다룬다. | 기업의 도입 발표·[Moderna][moderna], 위험 관리·[NIST][nist] |

## C. 데이터·지식·조직의 기억

독자: CIO, 데이터 책임자, 지식관리·현업 담당자. 기존 암묵지·Context Graph 글을 구체적인 설계 과제로 확장하는 묶음이다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 021 | 사내 검색 AI는 왜 제품번호를 자꾸 틀릴까? | 의미가 비슷한 자료 검색과 정확한 계약·제품 코드 검색을 구분한다. 키워드와 벡터 검색을 조합하는 이유를 현업 질문으로 설명한다. | 기술·[Microsoft RAG 검색 설계][rag] |
| 022 | Context Rot: 자료를 더 넣었는데 AI가 더 못하는 이유 | 입력이 길어질 때 정보 활용과 과업 성능이 달라지는 현상을 설명한다. 문서의 노후화와 구분하고, 자료 선별·분할·요약을 실제 업무로 비교한다. | 평가 연구·[Chroma Context Rot][context-rot] |
| 023 | PDF를 넣었는데 견적 금액이 달라졌다 | 표의 열·단위·각주·문서 구조를 잃으면 생기는 오류를 설명한다. OCR과 문서 파싱의 품질을 실제 계약서·견적서로 검증하는 방법을 제안한다. | 기술·[Azure Document Intelligence][doc-ai] |
| 024 | 영업팀과 재무팀의 ‘매출’이 다르면 AI도 헷갈립니다 | 부서마다 다른 지표 정의를 공통으로 관리하는 Semantic Layer를 설명한다. 자연어 데이터 분석에 앞서 계산식과 집계 기준을 정하는 이유를 다룬다. | 기술·[dbt Semantic Layer][dbt] |
| 025 | 같은 고객인데 이름이 셋: AX와 기준정보 관리 | CRM·ERP·고객지원 시스템의 고객과 상품을 맞추는 문제를 다룬다. 잘못 합친 대상의 정보가 다음 판단에 미치는 영향과 수정 이력을 설명한다. | 기술·[Graphiti의 엔터티·관계 모델][graphiti] |
| 026 | 정책은 바뀌었는데 AI는 작년 규정을 말합니다 | 공식 문서·메모·이전 정책의 우선순위와 유효 버전을 관리한다. 변경·폐기·권한 변경을 검색과 기억에 반영하는 경로를 설명한다. | 사례·[Covered California의 문서 관리][covered], 기술·[Graphiti][graphiti] |
| 027 | 직원이 AI를 고쳐줄 때, 회사에는 무엇이 남아야 할까? | 일회성 답변 수정, 검색 자료 갱신, 업무 규칙 변경, 모델 학습을 구분한다. 현업의 교정을 검증된 지식과 평가 사례로 남기는 방법을 다룬다. | 기술·[Context Engineering][context], [에이전트 평가][evals] |
| 028 | 에이전트 메모리: 대화 기록·사실·경험·절차를 나누는 법 | 단기·장기는 기억의 적용 범위, 사실·경험·절차는 기억 내용의 구분임을 설명한다. 무엇을 저장·검색·갱신하고 언제 지울지 업무별로 설계한다. | 기술·[LangGraph Memory][memory], 공식 지침·[개인정보보호위원회][pipc] |
| 029 | 사진·음성·센서에 남은 현장 지식을 AI가 읽으려면 | 멀티모달 AI가 업무 입력을 어떻게 바꾸는지 설명한다. 화면에 보이는 현상과 센서 값, 작업자의 설명을 같은 사건에 연결하는 설계를 제안한다. | 기술·[Gemma 멀티모달 모델][gemma], 현장 사례·[BMW AIQX][bmw-aiqx] |
| 030 | 매뉴얼 속 업무와 실제 업무가 다른 이유: Process Mining | 시스템의 실제 처리 이력에서 대기·재작업·예외 경로를 찾는 방법을 설명한다. 자동화할 업무를 고르는 데 프로세스 분석을 활용한다. | 사례·[Siemens와 Celonis][celonis] |

## D. 기술 트렌드와 구성 선택

독자: 경영진, CTO·CIO, AX 담당자. 기술 용어마다 기업이 선택해야 할 구성을 연결한다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 031 | Agent Skills: 범용 에이전트에 우리 회사 일을 가르치는 방법 | 업무 지침·스크립트·참고자료를 재사용 가능한 묶음으로 배포한다. Prompt·Tool·Skill의 차이와 필요한 내용만 불러오는 Progressive Disclosure를 설명한다. | 기술·[Anthropic Agent Skills][skills] |
| 032 | Compound AI Systems: 우리 회사 AI는 무엇을 조립해서 만들까? | 모델·검색기·코드·외부 도구·검증기가 함께 일하는 구성을 설명한다. 멀티에이전트를 포함할 수 있는 더 넓은 구성 관점에서 각 요소의 책임을 다룬다. | 개념 제안·[Berkeley AI Research][compound] |
| 033 | Planner와 Router: AI는 다음 할 일을 어떻게 고를까? | 목표를 작업으로 나누는 계획과 요청을 담당 도구·에이전트로 보내는 라우팅을 설명한다. 계획 수정, 승인 대기, 완료·중단 판단을 업무 사례에 연결한다. | 기술·[Google Cloud 에이전트 설계 패턴][google-patterns] |
| 034 | 작은 모델이 맡을 일, 큰 모델이 맡을 일 | 좁은 분류·추출 업무에 작은 모델이나 특화 모델을 쓰고 어려운 요청을 큰 모델로 넘기는 구성을 살핀다. 증류·특화의 효과는 실제 업무로 검증한다. | 연구 제안·[NVIDIA SLM 연구][small-models], 기술·[AWS 라우팅][routing] |
| 035 | 공개 모델을 사내에서 돌리면 정말 유리할까? | API 이용과 공개 가중치 모델의 자체 운영을 비교한다. 장비·동시 사용자·유지보수·데이터 위치·모델 라이선스가 결정에 미치는 영향을 다룬다. | 기술·[Gemma][gemma], 비용 체계·[FinOps][finops] |
| 036 | MCP는 사내 시스템 연결에서 무엇을 바꾸나? | 에이전트와 도구를 연결하는 표준이 해결하는 범위를 설명한다. 연결 이후 필요한 인증, 도구 설계, 사내 업무 규칙까지 함께 살핀다. | 표준·[MCP 보안 지침][mcp], 구현 설명·[MCP와 코드 실행][mcp-code] |
| 037 | 우리 회사 AI와 협력사 AI가 일을 주고받는다면 | A2A의 기능 발견·작업 상태·결과물 전달을 설명한다. 구매 요청을 협력사에 위임하는 예시로 기업 간 인증과 책임 경계를 검토한다. | 표준·[A2A 명세][a2a] — 기업 간 적용은 기획 예시 |
| 038 | AI도 팀을 꾸리면 더 잘할까? | 멀티에이전트의 병렬 조사·분업 이익을 중복 작업·결과 충돌·조율 비용과 비교한다. 에이전트 수를 늘릴 만한 업무의 조건을 다룬다. | 기술·[Google Cloud 에이전트 설계 패턴][google-patterns] |
| 039 | API 없는 사내 프로그램도 AI가 사용할 수 있을까? | 화면을 보고 클릭하는 Computer Use의 가능성을 살핀다. 화면 변경, 느린 처리, 로그인, 외부 발송과 승인 같은 실제 운영 조건을 설명한다. | 기술·[Anthropic Computer Use][computer-use] |
| 040 | Physical AI를 현실에 투입하기 전 가상 공간에서 시험하는 이유 | 디지털 트윈, 비전 AI, 로봇 제어의 관계를 설명한다. 가상 공장의 검증과 실제 공장의 안전·데이터 갱신을 연결한다. | 사례·[BMW FactoryExplorer][bmw-twin], 전환 계획·[삼성 AI 자율공장][samsung-factory] |

## E. 평가·운영·비용 관리

독자: AX 운영 책임자, 현업 품질 담당자, CTO·CFO. 시범 화면이 실제 서비스가 되는 데 필요한 운영 과제를 다룬다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 041 | 우리 회사 AI의 시험문제는 누가 만들어야 할까? | 실제 문의·실패·예외 사례를 평가용 문제로 만드는 과정을 설명한다. 현업과 개발자가 함께 합격 기준을 정하는 방법이 핵심이다. | 기술·[Anthropic 에이전트 평가][evals] |
| 042 | AI가 ‘처리했습니다’라고 말하면 일이 끝난 걸까? | 답변의 자연스러움과 실제 업무 완료를 구분한다. CRM 수정·발주·메일 발송 결과를 업무 시스템에서 확인하는 평가를 설계한다. | 기술·[Anthropic 에이전트 평가][evals] |
| 043 | 모델을 업그레이드했는데 업무 품질이 떨어졌다 | 기존 업무를 다시 시험하는 회귀 평가, 일부 사용자 배포, 이전 버전 복귀를 설명한다. 모델 교체를 운영 변경으로 관리하는 글이다. | 기술·[Anthropic 에이전트 평가][evals] |
| 044 | AI의 답을 다른 AI가 채점해도 될까? | 자동 채점의 효율과 판단 편향을 살핀다. 규칙 검사·실행 결과·현업 전문가의 검토를 조합해 평가 기준을 보정한다. | 기술·[Anthropic 에이전트 평가][evals] |
| 045 | 에이전트가 같은 주문을 두 번 넣지 않게 하려면 | A2A 메시지 중복 탐지와 업무 시스템의 실행 멱등성을 구분한다. 재시도·중단 복구에서 같은 주문이나 결제를 반복하지 않도록 작업 키와 실행 결과를 관리한다. | 기술·[A2A 명세][a2a], [Stripe 멱등 요청][idempotency] |
| 046 | Durable Execution: 결재자가 내일 승인해도 AI 업무가 이어지려면 | 실행 상태와 이력을 보존해 장애·재시작·사람의 응답 대기 후 작업을 이어가는 방식을 설명한다. 대화 메모리와 실행 복구, 중복 방지를 구분한다. | 기술·[Temporal Durable Execution][durable] |
| 047 | AI가 왜 틀렸는지 추적할 수 있는 운영 기록 | 모델 호출, 자료 검색, 도구 실행, 재시도를 연결해 보는 관측 체계를 설명한다. 오류·느린 응답·비용 증가의 원인을 찾는 데 초점을 둔다. | 기술·[OpenTelemetry GenAI 관측][telemetry] |
| 048 | 토큰 가격보다 중요한 ‘업무 한 건당 AI 비용’ | 모델·검색·도구·검토·재작업을 포함한 AI FinOps를 설명한다. 추론 예산, 반복 횟수, 동시 처리 한도와 중단 조건을 품질·업무 단가에 연결한다. | 비용 체계·[FinOps][finops], 기술 발표·[Google thinking budget][thinking] |
| 049 | Sandbox: 에이전트의 작업 공간을 어디까지 열어줄까? | Runtime은 실제 실행 환경, Sandbox는 접근 경계를 강제하는 장치로 구분한다. 파일·명령·네트워크와 하위 프로세스의 접근 범위를 다룬다. | 기술·[Anthropic Sandboxing][sandbox] |
| 050 | 사내 AI가 멈춘 날에도 회사는 돌아가야 합니다 | AI·연결 시스템 장애 시 사람에게 넘기거나 기존 절차로 돌아가는 방법을 정한다. 중지 권한, 복구 순서, 장애 이후 검토를 다룬다. | 위험 관리·[NIST AI RMF][nist], 위협 분석·[OWASP][owasp] |

## F. 거버넌스·보안·규제

독자: 경영진, 준법·감사·법무, CISO·CPO, AX 책임자. 국가별 적용 대상과 역할이 다른 규제는 구분해서 다룬다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 051 | Agent Control Plane: 부서마다 만든 에이전트를 누가 관리할까? | 흩어진 에이전트의 목록, 소유자, 신원·권한과 활동을 관리하는 운영 계층을 설명한다. 제품이 내세우는 기능과 조직이 정할 책임·위험 기준을 구분한다. | 제품·구조 설명·[Microsoft Agent 365][control-plane], 위험 관리·[NIST][nist] |
| 052 | AI에게 결재선을 만드는 법 | 환불·발주·대외 발송을 예로 자동 실행, 사람의 확인, 업무 시스템 승인을 나눈다. 사람을 형식적으로 끼워 넣지 않는 승인 화면과 판단 정보를 다룬다. | 구현 예제·[AWS 사람 승인][human-approval] |
| 053 | 감사팀은 AI의 어떤 기록을 봐야 할까? | 당시 입력과 정책, 적용 모델, 승인자, 실제 실행 결과를 남기는 방법을 설명한다. 내부 추론을 읽었다고 주장하지 않고 확인 가능한 근거로 감사를 구성한다. | 공식 체계·[NIST][nist], 기술·[OpenTelemetry][telemetry] |
| 054 | Agent Control Standard: 실행되는 순간 AI를 통제하는 방법 | 여러 에이전트 프레임워크의 실행 지점에 공통 정책을 적용하려는 ACS를 소개한다. 프롬프트의 지시와 실행 시점의 검사·차단을 구분하며 초기 표준 프로젝트의 범위를 설명한다. | 공개 표준 프로젝트·[OWASP ACS][acs] — 소개 페이지 게시일 2026-09-01 |
| 055 | 한국 AI 기본법, 우리 회사에는 어떤 질문을 던지나? | AI를 개발·제공·이용하는 역할과 서비스 성격부터 구분한다. 투명성·고영향 AI 등 관련 의무를 검토할 때 필요한 현황 자료를 정리한다. | 법령·[국가법령정보센터][korea-law] |
| 056 | 유럽 고객에게 AI 서비스를 팔 때 달라지는 일 | EU AI Act의 공급자·배포자 역할과 위험 분류를 설명한다. 국내 내부 업무 도입과 유럽 시장에 AI 제품을 제공하는 경우를 나누어 살핀다. | 공식 안내·[유럽연합 집행위원회][eu-act] |
| 057 | 사내 데이터를 AI에 넣는 것과 학습시키는 것은 어떻게 다를까? | 프롬프트·검색 자료·로그·모델 학습에서 개인정보가 이동하는 경로를 구분한다. 처리 목적, 계약, 보관·삭제 기준을 검토하는 방법을 다룬다. | 공식 지침·[개인정보보호위원회][pipc] |
| 058 | 외부 문서 한 줄이 사내 에이전트의 행동을 바꿀 수 있다 | 프롬프트 인젝션을 문서·웹페이지 처리 상황으로 설명한다. 읽어야 할 자료와 실행 지시를 구분하고 도구 권한·격리·승인을 함께 설계한다. | 위협 분석·[OWASP][owasp], 기술·[Computer Use][computer-use] |
| 059 | AI 에이전트에도 사번이 필요한 이유: Non-Human Identity | 에이전트의 신원, 위임받은 권한, 유효기간과 회수를 다룬다. 누가 어떤 권한으로 행동했는지 확인하고 도구의 읽기·수정 권한을 나누는 구조를 설명한다. | 표준·[MCP 인증·보안 지침][mcp], 제품·구조·[Agent 365][control-plane] |
| 060 | AI로 만든 광고·문서·코드의 권리는 누구에게 있을까? | 결과물의 권리 확보, 사람의 창작 기여, 입력 자료의 이용 권한을 구분한다. 미국 저작권청의 분석을 출발점으로 국가별 차이를 검토하는 글이다. | 공식 보고서·[미국 저작권청][copyright] |

## G. 영업·마케팅·고객 경험

독자: 영업·마케팅·고객지원 책임자. 응답 속도 외에 전환, 약속 이행, 브랜드 품질과 실제 해결을 다룬다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 061 | 고객센터 AI는 언제 사람을 불러야 할까? | 비밀번호 재설정·결제 문의·환불의 책임 차이에 따라 자동화 범위를 나눈다. 사람에게 넘길 때 고객이 설명을 반복하지 않게 만드는 방법을 다룬다. | 사례·[Wiley][wiley] — 자율 처리 일부는 파일럿 |
| 062 | 상담 AI의 해결률이 높아도 고객은 불만일 수 있습니다 | 대화 종료와 실제 문제 해결을 구분한다. 재문의·이관·취소·만족도를 함께 보며 상담 AI의 성과 지표를 설계한다. | 실제 측정 정책·[Intercom outcome 정의][intercom-outcomes] |
| 063 | 영업 AI가 가져온 잠재고객은 정말 영업 기회일까? | 문의량보다 고객 적합성·관심 수준·영업 인계 기준을 정하는 데 집중한다. AI의 고객 선별과 실제 수주 성과를 연결해 평가한다. | 제품 정책·[Fin for Sales][fin-sales] |
| 064 | 영업 에이전트가 지켜야 할 ‘약속의 한도’ | 견적·할인·납기·제품 성능을 어디까지 안내할 수 있는지 정한다. 최신 상품 정보, 가격 규칙, 승인권자를 연결하는 구성을 예시로 설명한다. | 적용 설계·[AWS 승인 패턴][human-approval], 위험 관리·[NIST][nist] |
| 065 | 상담 녹취가 CRM과 후속 업무로 이어지려면 | 회의 요약에서 고객 약속·할 일·후속 이메일 초안을 추출한다. 동의, 사람의 검토, CRM 기록 수정, 후속 업무 완료까지 연결한다. | 사례·[Morgan Stanley Debrief][morgan] |
| 066 | AI 광고에서 제품의 모양과 색을 지키는 방법 | 제품 디지털 트윈을 활용한 콘텐츠 제작을 살핀다. 생성 속도와 함께 제품 표현의 정확성, 국가별 소재 검수, 재작업을 관리한다. | 구축 파트너 사례·[Unilever·Collective][unilever] |
| 067 | AI 마케팅의 성과를 확인하는 실험 설계 | 광고·고객 매칭·상담의 효과를 구분해 비교한다. 클릭·매출·반품 등 여러 지표를 함께 보고 계절성과 다른 캠페인의 영향을 살핀다. | 현장 실험 논문·[온라인 유통의 생성형 AI][sales-study] |
| 068 | 개인화 추천은 누구의 문제를 풀어야 할까? | 고객의 탐색 부담과 회사의 판매 목표를 함께 살핀다. 전환율뿐 아니라 반품·불만·재구매까지 평가하는 개인화 과제를 제안한다. | 현장 실험 논문·[온라인 유통의 생성형 AI][sales-study] |
| 069 | Machine Payments: AI가 회사의 지식과 서비스를 구매한다면 | 검색·분석·문서 처리 기능을 API나 업무 단위 상품으로 제공하는 신사업을 검토한다. 에이전트가 고객이 될 때의 인증·지출 위임·과금이 주제다. | 기술·사업 발표·[Stripe Machine Payments][stripe-payments] |
| 070 | Agent Experience: 우리 서비스는 AI가 쓰기에도 편할까? | 고객의 에이전트가 기능을 찾고 사용하도록 문서·인터페이스·오류 응답을 설계한다. 사람의 UX, 개발자의 DX와 비교하되 기업의 AI 전환을 뜻하는 AX와 구분한다. | 개념 제안·[Netlify Agent Experience][agent-experience] |

## H. 재무·구매·법무·인사·IT

독자: CFO, 구매·법무·인사·IT 책임자. 거래 정확성, 예외 승인, 내부통제와 검토 부담이 중심이다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 071 | Tool 설계: 회계 API를 연결했는데 AI가 못 쓰는 이유 | 에이전트가 이해할 도구 이름·입출력 형식·단위·오류 메시지를 설계한다. 잔액 조회와 전표 확정을 나누는 예시로 API와 업무용 Tool의 차이를 설명한다. | 기술·[Anthropic Tool 설계][tools] — 회계 적용은 기획 예시 |
| 072 | 미수금 회수의 AX: 독촉 메일보다 먼저 바뀌는 일 | 입금·청구·고객 대화를 연결해 매칭과 사례 분류, 대응을 돕는다. 회수 우선순위와 분쟁 처리, 재무 내부통제까지 살핀다. | 사례·[Microsoft 재무팀][ms-finance] |
| 073 | 계약 검토 AI에 우리 회사의 협상 기준을 가르치는 법 | 반드시 지킬 조항과 양보 가능한 조건을 구분한다. 계약 초안·변경 이유·승인 이력을 연결해 법무팀의 검토 부담을 줄이는 방향을 다룬다. | 사례·[A&O Shearman Harvey][ao-harvey], [ContractMatrix][ao-contract] |
| 074 | 구매팀이 손대지 못한 소액 계약을 AI가 협상한다면 | 소액·다수 공급사 계약의 가격과 지급조건 협상을 살핀다. 협상 범위와 최저 조건, 사람에게 넘길 예외, 공급사 관계를 함께 다룬다. | 공급사 공개 사례·[Walmart·Pactum][pactum] |
| 075 | 가장 싼 부품이 가장 좋은 구매는 아닙니다 | 공급사·가격·부품 수명주기 정보를 연결한 구매 지원을 살핀다. 납기와 단종 위험까지 반영할 때 필요한 자료와 검토 기준을 제안한다. | 사례·[Jabil Intelligent Procurement Assistant][jabil] |
| 076 | 휴가·급여·증명서 문의를 실제 처리로 연결하는 HR AI | 직원별 권한과 국가별 정책을 지키며 인사 시스템을 연결한다. 일반 문의와 사람의 판단이 필요한 상담을 나누는 운영을 다룬다. | 사례·[IBM AskHR][ibm-hr] |
| 077 | 채용·인사평가 AI는 무엇을 추천하고 누가 결정해야 할까? | 편향, 설명, 이의 제기, 최종 결정권을 다룬다. 평가 초안 지원과 사람의 기회를 결정하는 자동 판단을 구분해 도입 범위를 설계한다. | 규제·[EU AI Act][eu-act], 위험 관리·[NIST][nist] |
| 078 | 제안서 수십 권을 비교하는 AI의 평가표 | RFP의 필수 조건·배점·근거 페이지를 구조화하는 적용안을 제안한다. 누락 항목과 확인할 주장을 드러내고 평가위원의 판단을 보조한다. | [Covered California의 RFP 검토][covered]에서 확장한 기획 — 세부 구현은 제안 |
| 079 | 투자회사의 조직 기억을 딜소싱과 실사에 연결하는 법 | EQT Motherbrain의 과거 딜·산업 지식 공유를 살핀다. 이를 바탕으로 투자 검토에서 근거와 가설, 추가 확인할 질문을 구분하는 적용안을 제안한다. | 기업 공식 사례·[EQT Motherbrain][eqt] — 세부 실사 구성은 제안 |
| 080 | 낡은 업무 시스템을 AI로 고칠 때 실제로 줄어드는 일 | 코드·의존성 분석부터 변환 계획과 수정까지의 현대화 작업을 살핀다. 자동 변환 뒤에도 필요한 기능·보안·운영 검증을 설명한다. | 사례·[Thomson Reuters와 AWS Transform][tr-modernize] |

## I. 제조·공급망·물류·건설·에너지

독자: 생산·품질·설비·구매·물류·현장 책임자. 불량, 가동 중단, 납기, 재고와 물리적 안전을 중심으로 풀어간다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 081 | 불량검사 AI의 정확도 99%는 충분할까? | 놓친 불량과 정상 제품의 재검사 비용을 함께 계산한다. 제품·조명·생산라인이 바뀔 때의 검증과 현장 피드백을 다룬다. | 사례·[BMW AIQX][bmw-aiqx] — 제목의 99%는 판단을 위한 가정 |
| 082 | 숙련공이 소리로 찾던 이상을 AI가 검사하려면 | 정상·불량 음원을 모으고 주변 소음을 구분하는 문제를 설명한다. 설비나 제품이 바뀌었을 때 재검증이 필요한 이유를 다룬다. | 사례·[BMW의 음향 품질검사][bmw-aiqx] |
| 083 | 포스코 자율조업에서 보는 제조 AX의 핵심 | 쇳물 예비처리 공정의 자율화 사례를 통해 센서·조업 조건·기존 제어 시스템의 연결을 살핀다. 특정 공정의 자동화와 공장 전체 자율화를 구분한다. | 국내 사례·[포스코 쇳물 예비처리 자율화][posco] |
| 084 | 공장 PLC 코드를 AI가 쓰면 검증은 누가 할까? | 설비 제어 코드와 화면 생성을 지원하는 AI를 살핀다. 시뮬레이션, 엔지니어 승인, 버전 관리와 현장 반영 절차가 중심이다. | 사례·[thyssenkrupp·Siemens Industrial Copilot][siemens-copilot] |
| 085 | 설비가 멈춘 순간 필요한 AI는 어떤 모습일까? | 오류 코드·매뉴얼·정비 이력을 연결해 정비사의 다음 확인을 돕는다. 잘못된 조치 방지와 복구시간, 교대근무 인수인계를 다룬다. | 현장 사례·[Siemens Erlangen 공장][siemens-copilot] |
| 086 | 수요예측을 잘해도 재고가 남는 이유 | 예측 결과가 발주·재배치·진열·폐기에 반영되는 과정을 살핀다. 품절과 재고금액 사이의 균형을 업무 규칙으로 만드는 것이 주제다. | 사례·[Walmart 공급망][walmart-supply] |
| 087 | “기사님, 언제 도착하세요?”를 AI에게 맡긴 DHL | 전화·메일로 하는 예약과 운송 상태 확인을 운영 시스템에 연결한다. 소음·억양·연결 실패와 일정 변경의 승인 범위를 다룬다. | 기업 공식 사례·[DHL·HappyRobot][dhl] |
| 088 | 배송 AI는 가장 짧은 길만 찾지 않습니다 | 납기·집하·차량·운전자·고객 약속을 함께 고려하는 경로 최적화를 설명한다. 예측, 최적화 알고리즘, 생성형 AI의 역할을 구분한다. | 사례·[UPS ORION][ups] |
| 089 | 공정회의의 “거의 끝났다”를 데이터로 바꾸는 AI | 현장 영상과 BIM·공정표로 진척과 작업속도를 확인한다. 지연 위험을 발견한 뒤 협력사와 대응계획을 바꾸는 업무까지 살핀다. | 현장 책임자 사례·[Wates·Buildots][wates] |
| 090 | 전력비를 줄이는 AI는 어떤 설비를 어떻게 움직일까? | 냉각·공조 운영의 예측과 제어를 설명한다. 절감량뿐 아니라 온도·압력 같은 운전 제약과 현장 검증을 함께 다룬다. | 선행 현장 사례·[Google DeepMind 데이터센터 냉각][cooling] — 2016년 사례 |

## J. 금융·보험·의료·제약·공공·서비스

독자: 각 산업의 사업·운영 책임자. 전문 판단의 근거, 고객 권리, 규정과 실제 서비스 성과를 함께 다룬다.

| 번호 | 포스팅 제목 후보 | 간단한 기획 설명 | 조사 근거·출발 사례 |
|---|---|---|---|
| 091 | 금융상담사의 지식을 모든 지점에서 꺼내 쓰는 방법 | 사내 리서치·상품 지식·정책을 상담 현장에 연결한다. 최신성과 고객에게 공유 가능한 범위, 답변 검증을 설계한다. | 기업 공식 사례·[Morgan Stanley Assistant][morgan] |
| 092 | 금융사 이상거래 탐지에서 AI의 설명이 중요한 이유 | 의심 거래 탐지와 조사·조치를 잇는 과정을 살핀다. 경보 정확성, 조사 부담, 고객 불편과 감사 근거를 함께 다룬다. | 기업 연차보고서·[DBS 위험관리][dbs] |
| 093 | 보험 청구서의 짧은 설명에 숨어 있는 재보험 회수금 | 재해 관련 청구를 분류해 연결하는 Zurich 사례를 살핀다. 분류 근거·재보험 조건·사람의 검토가 어떻게 이어지는지 설명한다. | 기업 공식 사례·[Zurich CATIA][zurich] — 2023년 파일럿 공개 |
| 094 | 의사가 환자를 보게 만드는 AI: 진료기록 자동화 | 진료 대화에서 기록 초안을 만드는 도구를 살핀다. 기록 수정량, 누락, 환자 동의와 의료진의 문서 부담을 평가하며 진단 자동화와 구분한다. | 실제 도입 분석·[The Permanente Medical Group][permanente] |
| 095 | 제약사의 AI는 어떤 연구를 계속할지 판단하는 데 쓰입니다 | Sanofi의 연구개발 포트폴리오 지원을 통해 비용·임상 일정·성공 가능성의 분석을 살핀다. 예측과 시나리오를 전문가의 투자 판단에 연결한다. | 기업 공식 사례·[Sanofi Plai][sanofi] |
| 096 | 같은 농업 질문에도 지역과 작물이 바뀌면 답이 달라집니다 | 시험 결과·재배 조건·지역·제품 정보를 결합하는 전문 AI를 살핀다. 적용 조건을 빠뜨리지 않고 농학자가 검증하는 구조가 핵심이다. | 기업 공식 파일럿·[Bayer 농업 전문가 AI][bayer] |
| 097 | 공공기관 AX: 정책 검색에서 실제 업무 지원까지 | 법안·정책 분석, 내부 문서와 서비스 업무를 연결한 사례를 살핀다. 원래의 접근권한과 사람의 검토를 유지하면서 확장하는 방식이 주제다. | 공급사 공개 사례·[Covered California][covered] |
| 098 | 호텔 예약을 돕는 AI는 고객의 어떤 수고를 줄일까? | 목적지·호텔·편의시설 탐색을 돕는 대화형 서비스를 살핀다. 추천 품질, 정보 최신성, 예약 전환과 현장 서비스 약속을 함께 평가한다. | 기업 공식 베타 출시·[Hilton AI Planner][hilton] |
| 099 | 유행을 발견한 뒤 매장에 걸리기까지: 상품기획의 AX | 트렌드 분석·디자인·상품개발을 연결하는 Walmart 사례를 살핀다. 기획 속도와 실제 판매율·재고 위험을 구분해 평가한다. | 기업 공식 사례·[Walmart Trend-to-Product][walmart-trend] |
| 100 | 고객의 AI가 우리 상품을 고르고 결제하는 시대 | Agentic Commerce에서 상품·가격·재고·결제·환불 정보가 연결되는 방식을 설명한다. 판매 채널과 고객 관계, 구매 위임의 통제를 검토한다. | 기술·사업 발표·[Stripe Agentic Commerce Suite][stripe-commerce] |

## 국내 독자에게 소개할 만한 해외 개념 12개

아래는 **100개 안에 포함된 주제의 별도 색인**이다. 해외 원문과 기업의 적용 논의를 확인해 추렸으며, 국내 인지도 순위는 아니다. 신생 프로젝트와 기존 개념의 재조명을 구분했다. Context Rot은 이미 [한국어 공식 문서][context-rot-ko]에서도 확인되므로 ‘국내 최초’나 ‘아직 소개되지 않음’으로 표현하지 않는다.

| 개념 | 주제 번호 | 해외 원문에서 확인한 흐름 | 경영진에게 설명할 이유 |
|---|---|---|---|
| Forward Deployed Engineer, FDE | 015 | 기존 현장 엔지니어 역할을 [AWS가 2026년 기업 AI 적용 조직으로 확대하는 발표][fde-aws]를 했다. | 모델을 도입한 뒤 남는 데이터·업무 예외·구현·운영을 누가 연결할지 설명할 수 있다. |
| Workslop | 017 | [BetterUp·Stanford 연구팀의 2025년 설문][workslop]에서 동료에게 검토 부담을 넘기는 AI 산출물을 다뤘다. | 개인의 작성 속도와 팀의 실제 생산성을 구분하는 데 유용하다. |
| Agent Skills / Progressive Disclosure | 031 | [Anthropic이 2025년 10월 구조를 소개][skills]했고, 12월 공개 표준화 업데이트를 알렸다. | 업무 지침·스크립트·참고자료를 필요한 시점에 불러오는 방식과 소유·검증·갱신 책임을 설명할 수 있다. |
| Context Rot | 022 | [Chroma가 2025년 7월 긴 입력의 과업 성능을 평가][context-rot]했다. | 사내 자료를 많이 넣는 것과 필요한 정보를 잘 활용하는 것의 차이를 설명한다. |
| Durable Execution | 046 | 기존 분산 실행 기술을 [Temporal이 2025년 에이전트 운영과 연결][durable]해 설명했다. | 하루 뒤 승인이나 장애 이후에도 이어져야 하는 발주·가입·계정 발급 업무와 연결된다. |
| Agent Control Plane | 051 | [Microsoft가 2025년 11월 Agent 365를 이 용어로 소개][control-plane]했다. | 부서별로 늘어난 에이전트의 목록·신원·권한·운영 책임을 관리하는 과제다. |
| Agent Control Standard, ACS | 054 | [OWASP 소개 페이지가 2026년 9월 1일 게시된 표준 프로젝트][acs]다. | 서로 다른 프레임워크에서 실행 시점의 공통 정책을 적용하려는 시도를 소개할 수 있다. 법적 의무나 인증은 아니다. |
| Agent Experience | 070 | [Netlify가 2025년 1월 에이전트가 서비스를 사용하는 경험][agent-experience]을 제안했다. | 고객의 AI가 자사 서비스를 발견·이해·사용할 수 있도록 제품과 문서를 설계하는 관점이다. |
| Machine Payments | 069 | [Stripe가 2026년 3월 MPP와 참여 서비스들을 발표][stripe-payments]했다. | 에이전트가 API·분석·정보에 비용을 지불할 때의 위임, 과금과 상품화를 다룰 수 있다. |
| Compound AI Systems | 032 | [BAIR의 2024년 개념 제안][compound]으로, 여러 모델·검색·코드·도구를 조합하는 시스템을 설명한다. | 모델 한 개의 성능과 기업 서비스 전체의 성능을 구분하는 데 유용하다. |
| Jagged Technological Frontier | 002 | 2023년 작업논문 이후 [2026년 정식 게재된 현장 실험][jagged]이다. | 같은 직무 안에서도 AI에 맡길 과업을 따로 시험해야 하는 이유를 설명한다. |
| Outcome-based Pricing | 009·062·063 | [Intercom의 2026년 정책][intercom-outcomes]은 해결·정해진 인계·고객 선별 등 결과 단위의 과금을 구체화했다. | ‘성과가 나면 지불’하는 계약에서 성과의 정의와 비용 분담을 검토할 수 있다. |

이 묶음에서 첫 소개 후보로는 **015 FDE, 017 Workslop, 031 Agent Skills, 054 ACS, 070 Agent Experience**를 권한다. 기존 글의 문제의식과 연결하면서 현업·조직·기술·거버넌스·고객 접점을 각각 다룰 수 있다.

## 에이전트 구성 요소별 주제 색인

이 표도 새 주제를 추가한 것이 아니라 위 100개를 구성 요소 관점으로 다시 찾기 위한 색인이다. Memory는 무엇을 유지할지, Tool은 무엇을 실행할 수 있는지, Skill은 일을 수행하는 지침과 자료를 어떻게 묶을지에 초점을 둔다.

| 구성 요소 | 설명할 핵심 질문 | 연결 주제 |
|---|---|---|
| 목표·지시·Prompt | 무엇을 맡기고 어떤 결과를 완료로 인정할까? | 004 |
| Model·모델 선택 | 어떤 과업을 어느 모델에 맡기고 어디에서 실행할까? | 033·034·035 |
| Context | 이번 판단에 어떤 자료를 얼마나 보여줄까? | 022·023·024 |
| Retrieval·검색 | 관련 근거와 정확한 코드, 최신 정책을 어떻게 찾을까? | 021·026 |
| Memory | 현재 작업과 여러 작업에 걸친 사실·경험·절차를 어떻게 기억할까? | 027·028 |
| Tool | 외부 시스템을 어떤 입력·출력·오류 규칙으로 사용할까? | 071·036·039 |
| Skill | 업무 지침·스크립트·참고자료를 어떻게 재사용하고 갱신할까? | 031 |
| Planner·Router | 목표를 어떻게 나누고 어느 도구·에이전트에 보낼까? | 033 |
| Loop·Orchestrator·협업 | 결과를 본 뒤 반복·분기·위임·합류를 어떻게 결정할까? | 032·033·037·038 |
| Runtime·Sandbox | 파일·코드·네트워크가 실제 실행되는 환경과 접근 경계는 무엇일까? | 035·049 |
| State·Checkpoint·실행 복구 | 중단·재시작·승인 대기 이후 무엇부터 이어갈까? | 045·046 |
| Identity·권한·Guardrail | 누구의 권한으로 행동하며 실행 중 어떤 정책을 적용할까? | 051·054·058·059 |
| Human-in-the-loop | 어느 지점에서 사람이 무슨 정보를 보고 승인할까? | 052·061·077 |
| Evaluation·Verifier | 답변뿐 아니라 실행 결과를 어떻게 검증할까? | 041·042·043·044 |
| Observability·감사 기록 | 실패·지연·비용·승인의 경로를 어떻게 추적할까? | 047·053 |
| Budget·종료·복구 절차 | 언제 멈추고 비용 한도를 어떻게 지키며 누구에게 넘길까? | 004·048·050 |

## 먼저 발행하기 좋은 12개

아래 순서는 검색량 예측이 아니라 **기존 포스트와의 연결성, 경영진의 관심, 사례의 구체성, 실제 도입 상담으로 이어질 여지**를 기준으로 한 편집 의견이다. 전략·기술·현장 사례를 번갈아 배치했다.

| 순서 | 후보 | 추천 이유 |
|---|---|---|
| 1 | 052. AI에게 결재선을 만드는 법 | 기존 에이전트·Context Graph 글을 실제 업무 권한과 승인 설계로 연결할 수 있다. |
| 2 | 001. AI로 시간을 아꼈는데 회사 이익은 왜 그대로일까? | 경영진이 체감하는 투자성과 문제를 연구와 현장 지표로 풀 수 있다. |
| 3 | 072. 미수금 회수의 AX | 익숙한 재무 업무에서 데이터 연결·예외 처리·현금흐름을 함께 설명할 수 있다. |
| 4 | 036. MCP는 사내 시스템 연결에서 무엇을 바꾸나? | 기술 트렌드와 실제 시스템 연동 비용·인증·업무 규칙을 연결하기 좋다. |
| 5 | 083. 포스코 자율조업에서 보는 제조 AX의 핵심 | 국내 제조 현장 사례로 생성형 AI를 넘어선 AX를 보여줄 수 있다. |
| 6 | 041. 우리 회사 AI의 시험문제는 누가 만들어야 할까? | ‘우리 업무를 잘한다’를 검증 가능한 기준으로 바꾸는 과정을 설명할 수 있다. |
| 7 | 073. 계약 검토 AI에 우리 회사의 협상 기준을 가르치는 법 | 암묵지 자산화가 법무·구매의 판단 기준으로 이어지는 구체적인 후속 글이다. |
| 8 | 031. Agent Skills로 우리 회사 일을 가르치는 방법 | 기존 암묵지 글을 재사용 가능한 업무 지침과 도구의 배포·갱신으로 연결할 수 있다. |
| 9 | 057. 사내 데이터를 넣는 것과 학습시키는 것의 차이 | 도입 논의에서 자주 섞이는 데이터 흐름과 개인정보 쟁점을 정리할 수 있다. |
| 10 | 089. 공정회의의 “거의 끝났다”를 데이터로 바꾸는 AI | 건설 현장의 납기·협력사 조율이라는 명확한 문제와 연결된다. |
| 11 | 002. AI 능력의 고르지 않은 경계와 첫 AX 과제 선정 | 기술의 인상적인 성능과 실제 업무의 적합성을 구분해 도입 범위를 정하도록 돕는다. |
| 12 | 100. 고객의 AI가 우리 상품을 고르고 결제하는 시대 | 내부 효율 개선에서 고객 접점과 새로운 판매 방식으로 시야를 넓힐 수 있다. |

## 분량이 커질 때의 시리즈 확장안

100개를 순서대로 읽어야 하는 강좌로 만들 필요는 없다. 다음 주제만 필요에 따라 나누고, 각 편에서도 문제·사례·판단 기준을 완결한다.

| 중심 주제 | 2~3편으로 나누는 방법 |
|---|---|
| 002·003·004 첫 AX 과제 | 과제 선택 → 목표·완료 조건 명세 → 실증과 확대·중단 판단 |
| 021·023·024 사내 데이터 활용 | 자료를 찾는 문제 → 문서 구조를 읽는 문제 → 숫자의 의미를 맞추는 문제 |
| 027·028 조직의 AI 메모리 | 무엇을 기억할지 → 교정을 검증하는 방법 → 정정·삭제·보관 기간 |
| 031·071 Agent Skills와 Tool | 지시·도구·스킬의 차이 → 업무용 도구 설계 → 지침과 스크립트의 검증·배포 |
| 036 MCP | 연결 표준의 의미 → 사내 도구·인증 설계 → 실제 업무 연결 사례 |
| 041·042·043 AI 평가 | 현업 시험문제 → 실제 완료 확인 → 변경 이후 품질 유지 |
| 048 AI FinOps | 업무 단가 계산 → 비용을 줄이는 구성 → 부서별 예산과 배분 |
| 051·052·053 AI 거버넌스 | 목록과 책임자 → 권한·승인 → 감사와 운영 기록 |
| 040·083·084 제조 AI | 가상 검증 → 실제 공정의 데이터·제어 → 변경 승인과 현장 운영 |
| 100 Agentic Commerce | 상품 발견 → 구매 위임과 결제 → 주문·환불·고객 관계 |

## 각 글을 구성할 때의 공통 방향

들어가며는 현장의 한 장면이나 경영진의 질문으로 시작한다. 본문에서는 사례의 실제 업무, 사용 기술, 남아 있는 사람의 역할을 설명한다. 나가며에서는 독자가 자기 조직에서 확인할 조건을 짚고, 필요한 지원으로 이어간다.

엡실론델타의 상담으로 연결할 때는 글의 문제와 맞는 도움을 구체적으로 제안하는 편이 좋다. 전략 글은 과제 발굴과 실증 설계, 데이터 글은 지식·기준정보·권한 구성, 기술 글은 도구와 업무 시스템 연결, 운영 글은 평가와 비용 관리, 산업 글은 현장 제약에 맞춘 적용이 자연스럽다.

## 자료 활용 메모

- 최신 동향의 기준으로 확인한 McKinsey 자료는 **2026-08-25 공개된 2026년판**이다. 같은 URL의 과거 2025년판 설명과 섞지 않는다.
- NBER의 직장 내 AI 연구와 Jagged Frontier 현장 실험은 해당 과제와 표본의 결과로 읽는다. 개인의 시간 절감이 곧 인원 감축이나 전사 이익 증가를 뜻하지 않는다.
- OECD·한국은행의 활용 조사와 기업 고객 사례는 조사 대상·자기보고·공급사 발표라는 성격을 보존한다.
- Wiley의 자율 처리, Bayer 농업 AI, Zurich CATIA, Hilton AI Planner는 연결한 발표에서의 파일럿·베타 상태를 표시했다. 집필 시 후속 운영 상태를 확인할 가치가 있다.
- 삼성의 2030년 자율공장 전환은 계획이고, BMW 디지털 트윈 자료의 일부 절감 수치는 전망이다. 달성 실적으로 표현하지 않는다.
- Wates의 예상 지연 변화는 실제 준공기간 단축과 다르다. 포스코의 특정 공정 자율화도 전체 제철소의 무인 운영과 다르다.
- 법규 주제는 집필 시점의 법령·시행령·공식 안내와 적용 국가를 확인한다. EU와 미국의 제도를 국내 기업에 그대로 적용하지 않는다.

[mckinsey]: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai
[nber-workplace]: https://www.nber.org/papers/w33795
[wef-org]: https://www.weforum.org/publications/organizational-transformation-in-the-age-of-ai-how-organizations-maximize-ais-potential/
[oecd-sme]: https://www.oecd.org/en/publications/generative-ai-and-the-sme-workforce_2d08b99d-en/full-report/component-4.html
[oecd-training]: https://www.oecd.org/en/publications/generative-ai-and-the-sme-workforce_2d08b99d-en/full-report/component-6.html
[bok-adoption]: https://www.bok.or.kr/portal/bbs/P0002353/view.do?menuNo=200433&nttId=10093071
[bok-talent]: https://www.bok.or.kr/portal/bbs/P0002353/view.do?menuNo=200433&nttId=10094926
[nber-learning]: https://www.nber.org/papers/w34851
[nber-labor]: https://www.nber.org/papers/w33777
[ilo]: https://www.ilo.org/publications/generative-ai-and-jobs-2025-update
[finops]: https://www.finops.org/framework/technology-categories/ai/
[intercom-outcomes]: https://www.intercom.com/help/en/articles/8205718-fin-ai-agent-outcomes
[fin-sales]: https://www.intercom.com/help/en/articles/13927115-fin-for-sales-faqs
[bbva]: https://www.bbva.com/en/innovation/bbva-drives-ai-adoption-through-talent/
[moderna]: https://www.modernatx.com/en-US/media-center/all-media/blogs/collaboration-with-openai
[nist]: https://www.nist.gov/itl/ai-risk-management-framework
[pipc]: https://pipc.go.kr/np/cop/bbs/selectBoardArticle.do?bbsId=BS074&nttId=11410
[rag]: https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/rag/rag-information-retrieval
[doc-ai]: https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/concept/retrieval-augmented-generation?view=doc-intel-4.0.0
[covered]: https://www.glean.com/resources/customer-stories/covered-california
[graphiti]: https://github.com/getzep/graphiti
[dbt]: https://docs.getdbt.com/docs/use-dbt-semantic-layer/dbt-sl
[context]: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
[evals]: https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents
[gemma]: https://ai.google.dev/gemma/docs/core
[bmw-aiqx]: https://www.bmwgroup.com/content/grpw/websites/bmwgroup_com/en/news/general/2023/aiqx.html
[celonis]: https://www.celonis.com/solutions/stories/siemens-inventory-management
[google-patterns]: https://docs.cloud.google.com/architecture/choose-design-pattern-agentic-ai-system
[thinking]: https://blog.google/innovation-and-ai/products/google-io-2025-all-our-announcements/
[small-models]: https://research.nvidia.com/labs/lpr/slm-agents/
[routing]: https://docs.aws.amazon.com/bedrock/latest/userguide/prompt-routing.html
[mcp]: https://modelcontextprotocol.io/docs/2025-11-25/tutorials/security/security_best_practices
[mcp-code]: https://www.anthropic.com/engineering/code-execution-with-mcp
[a2a]: https://a2a-protocol.org/latest/specification/
[computer-use]: https://platform.claude.com/docs/en/agents-and-tools/tool-use/computer-use-tool
[bmw-twin]: https://www.nvidia.com/en-eu/case-studies/bmw-group-develop/
[samsung-factory]: https://news.samsung.com/kr/삼성전자-2030년까지-ai-자율공장-전환-추진
[telemetry]: https://opentelemetry.io/blog/2026/genai-observability/
[owasp]: https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/
[human-approval]: https://aws.amazon.com/blogs/machine-learning/implement-human-in-the-loop-confirmation-with-amazon-bedrock-agents/
[korea-law]: https://www.law.go.kr/법령/인공지능발전과신뢰기반조성등에관한기본법
[eu-act]: https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai
[copyright]: https://www.copyright.gov/newsnet/2025/1060.html
[wiley]: https://www.salesforce.com/customer-stories/wiley/
[morgan]: https://www.morganstanley.com/press-releases/ai-at-morgan-stanley-debrief-launch
[unilever]: https://collectiveworld.com/collective-unilever-content-production-ai-digital-twins/
[sales-study]: https://arxiv.org/abs/2510.12049
[stripe-payments]: https://stripe.com/blog/machine-payments-protocol
[ms-finance]: https://www.microsoft.com/insidetrack/blog/streamlining-finance-cash-collection-at-microsoft-with-ai/
[ao-harvey]: https://www.aoshearman.com/en/news/ao-announces-exclusive-launch-partnership-with-harvey
[ao-contract]: https://www.aoshearman.com/en/insights/2024-alumni-yearbook/were-creating-a-firm-like-no-other
[pactum]: https://pactum.com/clients
[jabil]: https://aws.amazon.com/solutions/case-studies/jabil-manufacturing-transformation-generative-ai/
[ibm-hr]: https://www.ibm.com/case-studies/ibm-askhr
[tr-modernize]: https://aws.amazon.com/solutions/case-studies/thomson-reuters-case-study/
[posco]: https://newsroom.posco.com/kr/포스코-쇳물-예비처리-전-공정-자율화-성공인텔리/
[siemens-copilot]: https://press.siemens.com/global/en/pressrelease/siemens-industrial-copilot-expanded-adopted-thyssenkrupp
[walmart-supply]: https://corporate.walmart.com/news/2025/07/17/walmarts-us-supply-chain-playbook-goes-global-and-its-reinventing-retail-at-scale
[dhl]: https://group.dhl.com/content/dam/deutschepostdhl/en/media-relations/press-releases/2025/pr-dhl-and-happyrobot-20251111.pdf
[ups]: https://www.ups.com/us/en/customized-shipping-logistic-services/manufacturing-logistics-services/lean-manufacturing-process
[wates]: https://buildots.com/blog/wates-project-manager-using-ai-on-site/
[cooling]: https://deepmind.google/blog/deepmind-ai-reduces-google-data-centre-cooling-bill-by-40/
[dbs]: https://www.dbs.com/annualreports/2025/cro-statement.html
[zurich]: https://www.zurich.com/commercial-insurance/sustainability-and-insights/commercial-insurance-risk-insights/how-accurate-data-and-ai-can-transform-claims-and-help-customers-build-resilience
[permanente]: https://permanente.org/analysis-ai-scribes-save-physicians-time-improve-patient-interactions-and-work-satisfaction/
[sanofi]: https://www.sanofi.com/en/magazine/ai-in-healthcare/ai-across-the-research-development-value-chain-portfolio-decision-making
[bayer]: https://www.bayer.com/media/en-us/bayer-pilots-unique-generative-ai-tool-for-agriculture/
[hilton]: https://stories.hilton.com/releases/hilton-introduces-the-hilton-ai-planner
[walmart-trend]: https://corporate.walmart.com/news/2025/04/09/in-an-ever-changing-environment-walmart-uses-genai-to-create-cool-for-customers
[stripe-commerce]: https://stripe.com/blog/agentic-commerce-suite
[jagged]: https://doi.org/10.1287/orsc.2025.21838
[fde-palantir]: https://blog.palantir.com/a-day-in-the-life-of-a-palantir-forward-deployed-software-engineer-45ef2de257b1
[fde-aws]: https://aws.amazon.com/blogs/apn/introducing-forward-deployed-engineering-for-partners-winning-the-future-of-enterprise-ai/
[workslop]: https://www.betterup.com/workslop
[context-rot]: https://www.trychroma.com/research/context-rot
[skills]: https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills
[compound]: https://bair.berkeley.edu/blog/2024/02/18/compound-ai-systems/
[durable]: https://temporal.io/blog/durable-execution-meets-ai-why-temporal-is-the-perfect-foundation-for-ai
[control-plane]: https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/18/microsoft-agent-365-the-control-plane-for-ai-agents/
[acs]: https://genai.owasp.org/resource/agent-control-standard-acs/
[agent-experience]: https://www.netlify.com/blog/the-era-of-agent-experience-ax/
[eqt]: https://eqtgroup.com/about/motherbrain
[memory]: https://docs.langchain.com/oss/python/concepts/memory
[tools]: https://www.anthropic.com/engineering/writing-tools-for-agents
[sandbox]: https://www.anthropic.com/engineering/claude-code-sandboxing
[context-rot-ko]: https://platform.claude.com/docs/ko/docs/build-with-claude/context-windows
[idempotency]: https://docs.stripe.com/api/idempotent_requests
