# [사전 조사] AX와 암묵지 자산화

- 작성일: 2026-09-03 (1차), 2026-09-03 (2차 추가)
- 용도: tech.epsilondelta.ai 포스팅(geoff) 사전 자료 조사 노트
- 포스팅 성격(확정): AX 전체가 아니라 **AX 접근법 중 하나인 "에이전트를 활용한 암묵지 자산화"** 를 설명하고, 엡실론델타가 이를 해줄 수 있다는 것을 보여주는 **영업 성격의 글**. 학술 논의는 근거용 각주 수준으로만.
- 구성: Part 1(1차 조사, 이론·정책·통계) → **Part 2(2차 조사, 지식노동 사례·고충·유사 서비스·글 구조)**. 글을 쓸 때는 Part 2를 먼저 보면 됨.

---

# Part 2. 2차 조사 — 영업 포스팅 관점

## A. 국내 지식노동 분야 AI 에이전트 도입 사례 (금융·법무·회계·PE)

### A-1. 은행 (가장 활발, 그리고 "노하우 반영"을 명시적으로 말하는 유일한 분야)

| 기관 | 내용 | 암묵지 관련 표현 / 포스팅 활용 포인트 |
|---|---|---|
| **신한은행 – 여신심사지원 Agent** (2026.3) | 생성형 AI로 기업 정보(업황, 재무, 산업 동향, 거래 흐름, 담보 회수가치, 기술경쟁력)를 분석해 심사 의견서 작성 지원. 제조·SW 등 **12개 주요 업종별 맞춤 분석 엔진**(LLM만 쓰지 않고 업종별 재무분석 로직 적용) | 보도자료가 **"축적된 기업여신 노하우와 데이터를 반영"** 했다고 명시. "AI의 빠른 분석과 직원의 전문적 판단의 결합". → **어떻게 반영했는지는 어디에도 안 나옴.** 이 글이 설명해야 할 빈칸. |
| **신한은행 – 감정평가서 검증 에이전트** | 부동산 담보대출 감정평가서 검증, 건당 검토시간 약 70% 절감. 아파트·오피스텔부터 시작해 확대 | "좁은 업무 하나로 시작해 확대"의 실례 |
| **IBK기업은행 – IBK GenAI '제니'** (2025.8~) | 내규·업무매뉴얼 등 **행내 업무지식 12만 건 학습**. 2026.5 기준 **직원이 직접 만든 에이전트 1,000개 돌파**(신용장 개설 지원, 퇴직연금 상황별 업무처리 안내, 여신심사). 목표를 주면 계획 세우고 도구 써서 다단계 처리 | "현업이 직접 에이전트를 만든다"는 모델. 단, 12만 건은 **이미 문서화된 형식지**. 문서에 없는 판단 기준은 어떻게 하나? → 이 글의 질문 |
| **NH농협은행** | 기업여신 AI 사전심사(예비 평가·보고서 자동화) | |
| **우리은행** | 삼성SDS와 884억 규모, 5개 부문 29개 과제, 175개+ 에이전트(연내 90개) | 대형사는 수백억 단위 → 중견·중소는 이 방식 불가 |
| **KB금융** | 2026년 내 300여 개 에이전트 목표. 창구뿐 아니라 자산관리·여신심사·기획 등 본사 핵심 인력 업무까지 | |
| **웰컴저축은행** | 9월 전직원 "1인 1에이전트" 플랫폼 | |
| **금융위 AI 가이드라인** (2026.6) | AI는 최종 결정자가 아닌 **보조 수단**. 은행들이 리스크관리·내부통제로 구체화 중 | "판단은 사람, 판단 기준은 시스템에" 프레임과 정확히 부합 |

- **PwC컨설팅 "기업여신 비즈니스의 지능형 진화: AI Agent가 그리는 금융의 미래"** (2026.4): 기업여신은 "심사역의 경험과 정성적 판단에 크게 의존"해 왔고, 이제 "**기존에는 사람의 경험에만 의존하던 영역에 대한 기술적 지원이 현실화**". Master Agent(여신 정책·기준 통제) + Sub Agent 5개(상담→신청→평가→실행→사후관리). 생태계 4계층: **Expert(도메인 지식 보유 현업) – Bridger(현업-기술 연결) – Data Engineer – AI Infra**. 기업대출 잔액 859.8조(’26.3), 은행 직원 중 여신 담당 약 50% 이상. → 엡실론델타의 포지션은 정확히 "Bridger". 이 용어를 빌려 쓸 수 있음.

출처: [전자신문 – 신한 여신심사지원 에이전트](https://www.etnews.com/20260327000203), [신한금융그룹 보도자료](https://www.shinhangroup.com/kr/archive/press/detail/679), [뉴스프리존 – 은행권 AI 에이전트 확산](https://www.newsfreezone.co.kr/news/articleView.html?idxno=703499), [아주경제 – IBK 에이전트 1000개](https://www.ajunews.com/view/20260625150404908), [일간투데이 – IBK 직원이 만든 에이전트](https://www.dtoday.co.kr/news/articleView.html?idxno=776285), [PwC컨설팅 – 기업여신 AI Agent PDF](https://www.pwcconsulting.co.kr/ko/insight/pwcconsulting_credit-ai-agent.pdf), [파이낸셜뉴스 – 금융권 AX 대전환](https://www.fnnews.com/news/202607221814149178)

### A-2. 증권·자산운용

- **미래에셋증권 "AI 리서치센터" 개편, RA(리서치 어시스턴트) 채용 중단** (2026.4): 기존 RA 7명은 애널리스트로 승격, 이후 보조 업무는 AI로. 업계 반응: "미래 애널리스트 육성 포기", "AI가 일부 업무는 하지만 **애널리스트의 관록과 통찰을 대신할 순 없다**". 배경은 법인영업 수익성 악화.
- **포스팅 활용**: 암묵지가 전수되던 **사다리(RA → 애널리스트)** 를 AI가 끊는 사례. RA가 하던 "보조 업무"가 사실 도제식 학습이었다는 점. 자산화 없이 사다리만 끊으면 10년 뒤 "관록"은 어디서 오는가 → 자산화의 필요성을 역설적으로 보여줌.
- 출처: [인베스트조선](https://www.investchosun.com/site/data/html_dir/2026/04/28/2026042880123.html), [디지털데일리 – 증권가 AI 경쟁](https://www.ddaily.co.kr/page/view/2026051515452401442)

### A-3. PE (사모펀드)

- **아시아경제 "[PE는 지금] 수조원 투자하는 그들이 AI와 함께 일하는 법"** (2026.2): 국내 PE 대표들이 **개인적으로** ChatGPT·Gemini 사용. 용도 3가지 — 보고 받기 전 산업 훑기(회의를 설명→토론 중심으로), '악마의 대변인'으로 논리 약점 검토, 교차 검증. "AI는 그럴듯한 거짓말쟁이"(S사 M대표), 거래 세부사항엔 부적합. 공통 원칙: "**AI가 결정하는 것은 없고, 결정 직전의 사고 과정을 함께**". 블랙스톤은 자체 생성형 AI 플랫폼으로 조직 인프라화 단계.
- **포스팅 활용**: 국내 PE는 대표 개인의 ChatGPT 활용 단계 = 판단 기준이 **개인에 머물고 조직 자산이 안 됨**. MIT가 말한 shadow AI 그대로. 여기서 "하우스의 투자 기준을 에이전트에 심는다"는 제안이 나올 수 있음. (기존 리서치: MBK '프로젝트 아테나'가 국내 유일 문서화된 PE AI 사례.)
- 출처: [아시아경제](https://www.asiae.co.kr/article/2026022010143901152), [브런치 – 사모펀드가 인수한 회사에 AI를 도입한다는 것](https://brunch.co.kr/@168381316761446/11)

### A-4. 법무

- **법무법인 태평양, 전사 AI 업무체계** (2026.7.31): Harvey(7/1, 국제계약·외국법), Lbox·슈퍼로이어(국내 판례), ChatGPT Enterprise(8/1, 문서 초안·번역)를 업무 유형별로 배치. 약 700명 변호사·스태프. **"내부 지식과 업무 데이터 기반 자체 AI" 9월 베타, 11월 본격.** 경영진: "**도구 추가가 아닌 워크플로 전환**", "결과를 결정하는 본질은 도구가 아니라 쓰는 사람과 일하는 방식".
- **대형로펌 AI 전담팀** (아시아경제 2026.6): 김앤장 TMT 내 AI팀 70명, 태평양 2019년 국내 첫 AI팀 40명+, 세종 AI센터(2024.1), 광장 Tech&AI팀 100명+, 율촌 90명+ (LG AI연구원과 학습데이터 검증), 화우 AI센터 20명. → 이건 "AI **자문**" 조직이라 내부 업무 AX 사례로는 약함. 인용 시 구분 필요.
- **BHSN '앨리비 에이전트 for Legal'**: 법률 업무 전 과정 올인원 리걸AI, "개인 변호사도 대형 로펌처럼". 국내 리걸테크 에이전트 제품 대표 사례.
- **포스팅 활용**: 태평양의 "내부 지식·업무 데이터 기반 자체 AI"가 정확히 암묵지 자산화 시도인데, 대형 로펌은 700명분 데이터와 예산이 있음. **중소 로펌·사내 법무팀은?** → 타깃.
- 출처: [머니투데이 – 태평양](https://www.mt.co.kr/society/2026/07/31/2026073112041379783), [아시아경제 – 대형로펌 AI 전담팀](https://view.asiae.co.kr/article/2026063010084333889), [법률신문 – BHSN 앨리비 에이전트](https://www.lawtimes.co.kr/news/articleView.html?idxno=215362), [파이낸셜뉴스 – 대형로펌 상반기 실적](https://www.fnnews.com/news/202607071455402838)

### A-5. 회계

- **EY한영, 감사 업무에 AI 에이전트 전면 도입** (2026.4.20): 국내 대형 회계법인 최초. 'EY 캔버스' 감사 플랫폼에 멀티 에이전트 내재화, MS Azure·Foundry·Fabric 기반. 2028년까지 감사 전 과정. 철학: "**반복 업무 자동화로 감사인 전문 판단 강화**".
- 출처: [EY한영 보도자료](https://www.ey.com/ko_kr/newsroom/2026/04/ey-korea-news-release-2026-04-20), [네이트뉴스 – EY한영 비욘드 뷰](https://news.nate.com/view/20260518n36864), [KPMG 삼정 보도자료](https://kpmg.com/kr/ko/media/press-releases/2025/09/press-release-08.html)

### A-6. 사례들을 관통하는 관찰 (글의 논지 재료)

1. **공통 문법**: 모든 사례가 "AI는 보조, 판단은 사람"이라고 말한다(금융위 가이드라인, 신한, EY, PE 대표들). 그런데 **"사람의 판단 기준을 어떻게 시스템에 넣었는가"는 아무도 설명하지 않는다.** 신한의 "축적된 노하우 반영", 태평양의 "내부 지식 기반 자체 AI"가 전부 블랙박스. 이 글은 그 블랙박스를 열어 보여주는 글이 될 수 있다.
2. **규모의 벽**: 우리은행 884억, 태평양 700명, IBK 12만 건 문서. 이 방식은 문서와 예산이 있는 조직의 방식이다. **중견·중소 지식노동 조직(PE 하우스, 부티크 로펌, 회계·세무법인, 자문사, 사내 법무·재무팀)** 은 대표 개인의 ChatGPT 단계에 있고, 그들의 노하우는 문서가 아니라 사람에게 있다. → 타깃 독자.
3. **사다리 붕괴**: 미래에셋 RA 중단, 은행 40대 희망퇴직(아래 B). 도제식 전수가 끊기는 속도가 자산화 속도보다 빠르다.
4. **형식지 학습 ≠ 암묵지 자산화**: IBK 12만 건은 내규·매뉴얼이다. 매뉴얼에 없는 "이 거래처는 재무제표 좋아도 조심해야 한다"는 판단은 그 안에 없다. 형식지 RAG와 암묵지 자산화를 구분하는 것이 글의 핵심 차별점.

## B. 의사결정자가 실제로 겪는 고충 — 도입부 장면과 숫자

### B-1. "도입했는데 안 쓴다"

- **딜로이트 김수연 파트너, 2026 한경 AX 서밋** (2026.7): "**근로자 49%가 업무에 AI를 전혀 쓰지 않는다**". 글로벌 기업 88% AI 도입, 전사 배포는 7%. 해법으로 개발자가 아닌 현업 **'키맨'** 이 조직 내 확산을 이끈다고 주장. ([한국경제](https://www.hankyung.com/article/202607068325g))
- **한국은행 "AI 도입은 생산성을 높이는가?"**: 2025년 국내 취업자 51.8% 이상이 생성형 AI를 업무에 활용(인터넷 보급보다 8배 빠름), 그러나 지난 3년 국가 생산성 지표에 큰 변화 없음. ([한국은행 블로그](https://www.bok.or.kr/portal/bbs/B0000347/view.do?menuNo=201106&nttId=10098529), [KDI – 초기 3년 효과 분석](https://eiec.kdi.re.kr/policy/domesticView.do?ac=0000205512))
- **koreadeep 블로그**(한은 'AI 활용 실태조사 2025' 인용): 근로자 63.5%가 AI 사용, **54.1%는 사용 후에도 업무시간이 줄지 않았다**고 응답. "공공과 기업 문서의 90% 이상이 PDF, HWP, 스캔 이미지". 인용 가능 문장: "**개인은 이미 AI 시대에 들어섰다. 그러나 조직의 데이터 환경은 여전히 10년 전의 문서 중심 패러다임에 머물러 있다.**" ※ 63.5%(koreadeep)와 51.8%(한은 블로그)가 다름 — 조사 기준 차이일 수 있으니 한은 원자료 확인 후 인용. ([koreadeep](https://www.koreadeep.com/blog/ai-document-structure-issues))
- **대한상의 SGI** (2026.6): 국내 중소기업 10곳 중 7곳 생성형 AI 도입 계획 없음. 활용률 대기업 66.5% vs 중소 52.7%(13.8%p 차). **맞춤형 AI 도구 보유: 대기업 11.4% vs 중소 5.7%**. 지원·역량·태도를 통제하면 격차 4%p로 축소 → 규모가 아니라 조직 환경 문제. 대기업은 절약한 시간을 "새 프로젝트"에, 중소는 "휴식"에. ([글로벌이코노믹](https://www.g-enews.com/article/Industry/2026/06/2026061008033196493084322ec9_1), [대한상의 – 국내 기업 AI 기술 활용 실태](https://www.korcham.net/nCham/Service/Economy/appl/KcciReportDetail.asp?SEQ_NO_C010=20120938915&CHAM_CD=B001))
- 1차 조사 재인용: KOSA 제조업 AI 활용률 17.9%, 실패 4유형(R&R 불명확, 운영 모니터링 부재, 현장 데이터 편차, 거버넌스 부재), "HWP로 들어오는 순간 프로젝트 절반은 입력 처리".

### B-2. "사람이 나가면 판단이 같이 나간다"

- **5대 은행 희망퇴직 2,470명**(2025년, 2021년 이후 최대), 신규 채용은 1,170명으로 전년 절반. 희망퇴직 대상이 **40대까지 확대**(하나은행: 만 40세·15년 이상, 최대 28개월). KB 300개 에이전트 목표 → 여신심사·자산관리·기획 등 본사 핵심 인력이 대체 대상. ([뉴스웨이](https://www.newsway.co.kr/news/view?ud=2026062414343024268), [뉴시스](https://www.newsis.com/view/NISX20260602_0003654129), [데이터뉴스](https://datanews.co.kr/news/article.html?no=145019))
- **미래에셋 RA 채용 중단** (A-2) — 전수 사다리 붕괴.
- **Deloitte Insights "Capturing institutional knowledge"**: "**조사 대상 조직의 92%가 곧 은퇴할 직원의 지식을 일관되게 포착하지 못한다**"(eGain/APQC), C레벨 85%가 지식 유출을 중대~치명적 위협으로 인식. 평균 재직기간 4.6년→3.9년. 권고 5단계 중 핵심: 20%의 지식이 80%의 문제를 해결(고영향 지식에 집중), **Expert–Next'pert–Practitioner** 모델, **일회성 아닌 일상 워크플로에 포착을 내장**. ([Deloitte](https://www.deloitte.com/us/en/insights/topics/talent/knowledge-management-plan.html))
- IDC "Fortune 500, 지식 미공유로 연 315억 달러 손실" — 2018년 이전 자료로 오래됨. 인용 시 "오래된 추정치" 명시하거나 생략 권장. ([Nuclino](https://blog.nuclino.com/not-sharing-knowledge-costs-fortune-500-companies-31-5-billion-a-year))
- 국내 지식노동 인력 이탈 통계는 은행 외에는 약함(회계법인·로펌 어쏘 이직률 등은 3차 조사 필요).

### B-3. 도입부 장면 후보 (금융·법무·PE 독자 기준)

1. 20년차 여신 심사역이 희망퇴직으로 나간 다음 달, 후임이 같은 거래처 심사 의견서를 쓰는데 "이 업종은 매출채권 회전일을 먼저 본다"는 기준을 아무도 모른다. 내규에는 없다.
2. PE 하우스 대표가 ChatGPT로 산업 리서치를 훑고 회의에 들어온다. 회의는 좋아졌다. 그런데 대표가 어떤 딜을 왜 거르는지는 여전히 대표 머릿속에만 있고, 심사역 3명은 각자 다른 ChatGPT에 각자 다른 질문을 한다.
3. 사내 법무팀이 계약 검토 AI를 도입했다. 표준 조항은 잘 잡는데 "우리 회사는 이 거래처와는 손해배상 상한을 절대 안 받는다"는 걸 몰라서 결국 팀장이 다 다시 본다. 3개월 뒤 아무도 안 쓴다.
4. IBK처럼 매뉴얼 12만 건을 학습시켰다. 매뉴얼에 있는 건 답한다. 매뉴얼에 없는 걸 물으면 그럴듯하게 틀린다. 직원들은 "매뉴얼에 있는 건 나도 안다"고 말한다.

## C. 유사 서비스·경쟁자의 설명 방식 (포지셔닝 참고)

| 유형 | 대표 사례 | 메시지 | 한계 (= 엡실론델타 차별점) |
|---|---|---|---|
| **오프보딩 인터뷰형** | **Sensay** "세계 최초 AI 오프보딩 플랫폼": 퇴사 통보 기간 중 AI 음성 인터뷰 2~3회(1~2주), 역할별 맞춤 질문 + 파일 업로드 → 핸드오버 브리프, 검색 가능한 전사본, Slack/Teams 챗봇. "매일 기업은 사람이 떠날 때 수년의 경험을 잃는다." 고객·가격 미공개 | **퇴사 시점의 일회성 추출**. 결과물은 읽는 문서/챗봇이지 **일하는 에이전트가 아님**. 교정·축적 루프 없음 |
| **엔터프라이즈 검색형** | **Glean**: 250+ 데이터 소스 연결, "당신의 회사를 이해하는 엔터프라이즈 AI", 온보딩 가속. 은퇴자 지식 이전을 별도 메시지로 내세우지 않음 | **문서가 있어야** 작동. 문서화되지 않은 판단 기준은 검색할 수 없음 (IBK 12만 건과 같은 한계) |
| **컨설팅 프레임워크형** | **Deloitte** 5단계, Expert–Next'pert–Practitioner, "일상 워크플로에 포착 내장" | 방법론은 좋으나 실행 도구가 없음. 결국 사람이 문서 쓰는 KM으로 회귀 |
| **제조 피지컬 AI형** | HD현대(30년 용접사의 판단을 온톨로지로), 원프레딕트("숙련자 경험을 조직이 소유·학습하는 제조 운영지능") | 센서·영상 데이터 기반, 지식노동에는 해당 없음. 다만 **"조직이 소유하고 계속 학습하는 자산"이라는 표현은 차용 가치 높음** |
| **데이터 카탈로그형** | Atlan "Tacit Knowledge Capture for AI Agents" | 메타데이터·컨텍스트 관리 관점, 판단 기준 추출은 아님 |

출처: [Barchart – Sensay 출시](https://www.barchart.com/story/news/36018738/sensay-launches-worlds-first-ai-offboarding-platform-for-knowledge-transfer), [Globe and Mail – Retiring? An AI agent will see you now](https://www.theglobeandmail.com/investing/personal-finance/retirement/article-retiring-an-ai-agent-will-see-you-now-to-download-your-knowledge/) (robots 차단, 제목만 확인), [Glean](https://www.glean.com/perspectives/how-ai-facilitates-knowledge-transfer-from-retiring-engineers), [Deloitte](https://www.deloitte.com/us/en/insights/topics/talent/knowledge-management-plan.html), [Ideagen – When your best expert retires](https://www.ideagen.com/noram/thought-leadership/blog/when-your-best-expert-retires-how-ai-preserves-irreplaceable-ehs), [Atlan](https://atlan.com/know/ai-agent/data-for-ai/tacit-knowledge-capture-for-ai-agents/)

**엡실론델타 포지셔닝 문장 초안**: 퇴사자 인터뷰(Sensay)도, 문서 검색(Glean, IBK)도 아니다. **현직자의 판단 기준을 에이전트가 인터뷰로 꺼내고, 그 기준으로 실제 업무를 처리하게 하고, 담당자의 교정이 다시 기준에 쌓이는 구조**를 만든다. 결과물은 매뉴얼이 아니라 "우리 회사 기준으로 일하는 에이전트"이고, 그 에이전트가 쌓는 판단 이력이 회사 자산이 된다. (학술 근거: PKAI의 인터뷰 에이전트 설계, Uchihira의 단편 지식 조립, MIT의 learning gap — Part 1 참조)

## D. 글 구조 (영업 포스팅 버전)

1. **장면** — B-3 중 1~2개. 숫자 한 줄(49% 안 쓴다 / 92% 조직이 은퇴자 지식 못 잡는다 / 5대 은행 2,470명).
2. **왜 AI 도입해도 안 바뀌는가** — 지금까지 넣은 건 문서(형식지)였고, 실제 일은 문서에 없는 판단(암묵지)으로 돌아간다. 신한·IBK·태평양 다 "노하우 반영"이라 말하지만 어떻게인지는 안 말한다. 여기서 암묵지 개념을 **한 단락**으로만.
3. **에이전트로 암묵지를 자산화한다는 것의 실제 모습** — 가상 업무 하나(기업여신 1차 심사 / PE 딜 스크리닝 / 계약 1차 리뷰 중 택1)로 처음부터 끝까지: 인터뷰 → 되묻기(실제 사례 제시) → 기준 구조화·확인 → 실제 업무 실행 → 교정 → 기준 갱신. 이 절이 글의 60%.
4. **왜 ChatGPT 열어놓고 팀장한테 물어보게 하면 안 되는가** — 인터뷰 설계, 실행 가능한 형태로의 엔지니어링(Skills/규칙/메모리 — 개발자용 단락, 건너뛰어도 되게), 축적 루프. 없으면 또 하나의 안 읽는 매뉴얼(KM 30년 실패).
5. **누가 시작할 수 있나** — 핵심 인력 1~2명에게 판단이 몰린 업무가 있고, 그 사람이 병목이거나 몇 달 내 빠질 수 있는 조직. 업무 하나로 시작. 대형사처럼 수백억 안 든다.
6. **한 문장 신뢰 요소** — 지식 제공자 인센티브 설계도 함께 다룬다(한국노총 쟁점 참조). 금융위 가이드라인처럼 "판단은 사람"이 규제 방향과도 맞다.

## E. 3차에서 확인할 것

- 한은 'AI 활용 실태조사 2025' 원자료: 51.8% vs 63.5%, 54.1% 수치 확정.
- 신한 여신심사지원 Agent의 "노하우 반영" 방식에 대한 추가 보도(인터뷰 기사 등) — 없으면 "공개된 바 없다"로 기술.
- 태평양 자체 AI 9월 베타 관련 후속 기사(이 글 발행 시점에 나올 수 있음).
- 회계법인·로펌 어쏘 이직률, 사내 법무·재무팀 인력 관련 국내 통계.
- 가상 업무 사례를 어느 도메인으로 잡을지 결정 후, 해당 도메인의 실제 심사 항목·체크리스트 공개 자료(예: 기업여신 심사 항목, PE IC 메모 구조) 확보.
- Globe and Mail 기사 원문(오프보딩 AI 인터뷰 업체 목록·비판) — 다른 경로로 확인.

---

# Part 1. 1차 조사 — 이론·정책·통계 (근거 자료)

---

## 0. 한 줄 요약

AX(AI Transformation) 담론은 2026년 현재 "도입"에서 "운영 재설계"로 초점이 옮겨가고 있고, 그 병목으로 반복 지목되는 것이 **조직에 문서화되지 않은 판단 기준(암묵지)**이다. 한편 정부(산업부 480억 "제조 암묵지 기반 AI모델")·대기업(HD현대 명장 에이전트)·학계(GenAI SECI 모델, LLM 기반 암묵지 추출 연구)가 동시에 "암묵지를 디지털 자산으로 바꾸는 것"을 AX의 핵심 과제로 보기 시작했다. 다만 철학적 반론(Collins: 집단적 암묵지는 텍스트로 전달 불가)과 사회적 쟁점(숙련공 보상·지식 소유권)이 함께 존재하므로, 포스팅은 "암묵지를 전부 형식지로 바꿀 수 있다"는 낙관론과 "불가능하다"는 회의론 사이에서 **실무적으로 무엇이 자산화 가능한가**를 다루는 것이 차별화 포인트가 될 수 있다.

---

## 1. AX(AI Transformation) 담론 현황

### 1.1 정의와 DX와의 차이 (국내 담론)

- 국내에서 AX는 대체로 "DX의 다음 단계"로 소개된다. DX가 프로세스의 디지털화·데이터화였다면, AX는 그 데이터 위에서 AI가 판단·실행까지 담당해 **일하는 방식 자체**를 바꾸는 것으로 정리된다. ([MSAP.ai – AX vs DX](https://www.msap.ai/ax/ax-vs-dx/), [MSAP.ai – AX란 무엇인가](https://www.msap.ai/ax/what-is-ax/), [flex – AX 뜻과 핵심요소](https://flex.team/blog/2025/10/27/ax), [이글루코퍼레이션 – 보안 101 AX](https://www.igloo.co.kr/security-information/%EB%B3%B4%EC%95%88-101-%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5-%EC%A0%84%ED%99%98ax%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80%EC%9A%94/))
- 카카오벤처스 인터뷰(신재인 바이버스 AI 대표)는 AX를 "소프트웨어 생산 비용이 기하급수적으로 줄어드는 거대한 흐름"으로 정의하고, 경쟁의 판이 "생산 효율"에서 "기획"으로 옮겨왔다고 주장. 도입 단계에 머문 DX와 달리 AX는 조직 내부의 일하는 방식을 바꾸는 데 초점. ([카카오벤처스 – AX란 무엇인가](https://www.kakao.vc/blog/ax-ai-transition-strategy))
- 참고: "AX"라는 약어는 한국·일본에서 주로 쓰이고, 영어권에서는 "AI transformation" 또는 "enterprise AI adoption"으로 표현된다. 포스팅에서 용어의 지역성을 한 번 짚어주면 좋음(프롬프트 엔지니어링 포스팅에서 버즈워드를 다룬 톤과 연결 가능).

### 1.2 정부 정책 (2026)

- 과기정통부·산업부·중기부 3개 부처가 2026년 3월 "주요 인공지능 전환(AX) 사업"을 통합 공고. AI 에이전트 핵심기술(과기부), 제조현장 AI 에이전트 개발·실증 및 산업 AI 솔루션 실증·확산(산업부), 중소 제조 AI 다중 에이전트·스마트공장(중기부). ([다음뉴스 – 정부 AX 사업 공동 추진](https://v.daum.net/v/20260312110035947))
- 중소기업 대상 "AX 원스톱 바우처 지원사업"(2026) 수요기업 모집. ([기업마당 공고](https://www.bizinfo.go.kr/sii/siia/selectSIIA200Detail.do?pblancId=PBLN_000000000120085))
- 「대한민국 인공지능행동계획(인공지능 기본계획 2026~2028)」(2026.2, 국가인공지능전략위원회·과기정통부) — 원문 PDF. 2차 조사에서 "암묵지/산업 데이터" 관련 문구 확인 필요. ([PDF](https://smartcity.go.kr/wp-content/uploads/2026/03/%EC%95%88%EA%B1%B41%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%ED%96%89%EB%8F%99%EA%B3%84%ED%9A%8D%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%EA%B8%B0%EB%B3%B8%EA%B3%84%ED%9A%8D20262028.pdf))

### 1.3 "AX 실패" 통계 — 왜 도입해도 안 바뀌나

| 출처 | 핵심 수치 | 실패/성공 요인 |
|---|---|---|
| MIT NANDA "The GenAI Divide" (2025.8) | 미국 기업 GenAI 투자 350~400억 달러, 파일럿의 95%가 P&L 영향 0, 5%만 프로덕션 스케일 | 모델 성능이 아닌 **"learning gap"**: 대부분의 GenAI 시스템이 피드백을 유지하지 않고, 맥락에 적응하지 않고, 시간이 지나도 개선되지 않음. 직원 90% 이상이 개인적으로 ChatGPT 등을 사용("shadow AI"), 성공 기업은 깊은 커스터마이징과 벤더를 비즈니스 지표로 책임지게 함 | 
| McKinsey State of AI (2026.8.25) | 응답자 ~90%가 1개 이상 기능에서 AI 정기 사용, 44%가 전사 스케일링, EBIT 영향 보고 37%(전년과 동일), "high performer" 6% | high performer는 기존 프로세스에 도구를 끼워넣는 대신 **"AI 사용을 이유로 워크플로를 근본적으로 재설계"**, 경영진의 커밋과 측정 프로세스 |
| KOSA / 초거대AI추진협의회 사례집 (아주경제 2026.5) | 제조업 AI 활용률 17.9% | 실패 유형 4가지: R&R 불명확, 운영 모니터링 부재, 현장 데이터 편차 미대응, 거버넌스 부재. "AI가 읽을 재료가 HWP로 들어오는 순간 프로젝트의 절반은 생성이 아니라 입력 처리" |
| 한국무역협회 "AX 우수사례로 본 AI 도입 효과 극대화 방안" (2025.11.21) | 10개 사례(수요 6, 공급 4) | 조직 공감대, 인재·역량, 비용, 데이터 인프라, **현장 주도 문제 발굴(problem-driven)** 5요소. 일회성 프로젝트 아닌 순환형 추진 |

출처: [Mind the Product – MIT 2025 AI Report](https://www.mindtheproduct.com/why-most-ai-products-fail-key-findings-from-mits-2025-ai-report/), [Forbes – MIT finds 95% fail because companies avoid friction](https://www.forbes.com/sites/jasonsnyder/2025/08/26/mit-finds-95-of-genai-pilots-fail-because-companies-avoid-friction/), [McKinsey – The state of AI](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai), [아주경제 – AX에 실패하는 기업들](https://www.ajunews.com/view/20260511141644195), [KDI 경제교육정보센터 – 무협 보고서](https://eiec.kdi.re.kr/policy/domesticView.do?ac=0000200330&pg=&pp=20&issus=M), [Salesforce KR – AX 전환이 실패하는 5가지 이유](https://www.salesforce.com/kr/blog/ai-transformation-ax/), [서치라이트 – AX 95%가 실패하는 진짜 이유](https://blog.searchright.net/ax-transformation-success-conditions/)

**포스팅 연결 포인트**: MIT의 "learning gap"(시스템이 맥락을 기억·학습하지 않음)과 McKinsey의 "워크플로 재설계"는 결국 같은 이야기다. 워크플로를 재설계하려면 현재 워크플로가 어떻게 돌아가는지 알아야 하는데, 그 대부분은 사람 머릿속(암묵지)에만 있다. 여기서 암묵지 자산화가 AX의 선행 조건이라는 논리가 성립.

---

## 2. 암묵지(Tacit Knowledge) 이론 정리

### 2.1 고전

- **Michael Polanyi, 《The Tacit Dimension》(1966)**: "We can know more than we can tell." 암묵지 = 경험으로 익히지만 말로 다 옮길 수 없는 지식(얼굴 인식, 자전거 타기). ([Wikipedia – Polanyi's paradox](https://en.wikipedia.org/wiki/Polanyi%27s_paradox))
- **Polanyi's Paradox (David Autor, 2014)**: 자동화가 과대평가된 이유 — 기계는 규칙으로 명시되지 않은 상식·유연성·판단이 필요한 일을 못 한다. 그 결과 직업 양극화(추상적 업무 vs 육체적 업무는 남고, 코드화 가능한 루틴 업무만 사라짐). 낙관론자들은 ML(AlphaGo 등)이 "규칙을 명시하지 않고 데이터에서 직접 암묵적 패턴을 학습"함으로써 이 역설을 우회한다고 주장. → **LLM 시대에 이 역설이 깨졌는가**가 포스팅의 좋은 철학적 프레임.
- **Nonaka & Takeuchi, SECI 모델 (1995)**: 공동화(Socialization, 암묵→암묵) → 표출화(Externalization, 암묵→형식) → 연결화(Combination, 형식→형식) → 내면화(Internalization, 형식→암묵). 지식창조는 이 나선의 반복. ([나무위키 – SECI 모델](https://namu.wiki/w/SECI%20%EB%AA%A8%EB%8D%B8), [KIRD – R&D인력 전문성의 핵심: 암묵지](https://www.kird.re.kr/newsletter/html/vol122/sub02.html))
- **Harry Collins, 《Tacit and Explicit Knowledge》(2010)**: 암묵지를 3층으로 구분 — Relational(관계적: 원리상 말할 수 있지만 안 말해진 것), Somatic(신체적: 몸이 아는 것), Collective(집단적: 사회에 참여해야만 얻는 것). ([시카고대 출판부](https://press.uchicago.edu/ucp/books/book/chicago/T/bo8461024.html), [Composition Forum 리뷰](https://compositionforum.com/issue/49/amidon-collins-review.php)) → **자산화 가능성은 층마다 다르다**는 논리를 세우는 데 유용. Relational은 인터뷰/에이전트로 추출 가능, Somatic은 센서·영상 데이터(제조 암묵지 사업의 접근), Collective는 가장 어려움.

### 2.2 GenAI 시대의 SECI 재해석 (2025~2026 학술 동향)

RealKM(2026.6.5)이 세 관점을 정리:

1. **GRAI 프레임워크** — Böhm & Durst (2025, *VINE Journal*): SECI 각 단계를 인간/기계 관점으로 나눠 8개 상호작용 필드. "기계를 참여자로 봐야 한다."
2. **Hybrid SECI** — Cerchione, Liccardo & Passaro (2026, *Journal of Innovation & Knowledge*): GenAI는 인간 지식창조 루프와 분리된 **"machine dimension"** 에서 작동. 대화형 AI는 공동화를 흉내내지만 "감정적·경험적 깊이가 없다." ([ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2444569X25002112))
3. **GenAI SECI 모델** — Naoshi Uchihira(JAIST) (2026, arXiv 2603.21866; RealKM은 Nishimura, Ijuin을 공저자로 표기하나 arXiv 초록 페이지에는 Uchihira 단독 — 원문 PDF에서 확인 필요): 핵심 개념은 **"Digital Fragmented Knowledge(디지털 단편 지식)"** — 완전히 형식화되지 않은 채 사이버공간(채팅, 사진, 로그, 메모)에 쌓이는 부분적 지식. 명시지/잠재지/암묵지 3층 연속체. GenAI가 이 단편들을 표출화(의미 단위로 집계)·연결화(지식그래프)·내면화(관련 단편을 골라 제시) 단계에서 보조. 공동화는 여전히 인간의 영역. GenAI는 "엄밀히 보조 수단"이며 **symbol grounding(의미 해석)은 인간이 워크숍 등에서 수행**. 초기 제안 단계, 실증 미완(Digital Knowledge Twin System 개발 중). ([arXiv PDF](https://arxiv.org/pdf/2603.21866), [RealKM 정리](https://realkm.com/2026/06/05/rethinking-the-seci-model-for-genai-three-perspectives-including-one-from-japan/))

**포스팅 연결 포인트**: "Digital Fragmented Knowledge"는 실무 감각과 정확히 맞는 개념이다. 기업의 암묵지는 완전한 백지 상태가 아니라 슬랙 스레드, 카톡, 이메일, 회의록 초안, 엑셀 주석 같은 **단편**으로 이미 반쯤 새어 나와 있고, LLM은 이 단편을 모아 의미 단위로 만드는 데 특히 강하다. 에이전트 관점에서 "완전한 문서화"를 요구하지 않고 단편으로 작업하는 접근이 현실적.

---

## 3. LLM/에이전트 기반 암묵지 추출 연구

| 연구 | 방법 | 결과 | 한계 |
|---|---|---|---|
| Zuin et al., "Leveraging LLMs for Tacit Knowledge Discovery in Organizational Contexts" (IJCNN 2025, arXiv 2507.03811) | LLM 에이전트가 직원들과 반복 대화하며 지식을 재구성. 지식 전파를 SI 감염 모델로 모사, 864회 시뮬레이션 | 도메인 전문가에 직접 접근하지 않고도 **94.9% full-knowledge recall**. 조직 위계와 비공식 네트워크를 탐색해 단편 지식 수집 | 합성 조직 구조(실조직 아님) |
| Schinckus, Simonofski, Bono Rosselló, "LLMs for Process Knowledge Acquisition" (BISE 2025, Springer) | 통신사 8개월 참여관찰 + 분석가 인터뷰 11건 → **PKAI** 멀티에이전트 시스템(준비 → 공동화: 에이전트가 전문가와 반구조화 인터뷰, 응답 품질에 따라 후속 질문 → 표출화: BPMN·문서 생성) | 유용성 5.36/7, 사용성 5.44/7. 준실험(n=26)에서 PKAI 지원 그룹의 모델 품질이 의미·실용 차원에서 우수. 비동기·표준화된 지식 획득 | 생성 모델은 숙련 분석가의 보정 필요, 환각, 표본 작음, 대량 문서 시 토큰 비용 |
| Rank et al., "LLMs for Tacit Knowledge Elicitation in Industry 5.0: A Literature Review" (AHFE 2025) | 1,904건 중 15편 체계적 리뷰 | 추출 방법 5유형: 작업자 대화 에이전트, NLP 보조 지식 워크숍, 이상 발생 시 트리거되는 LLM 리플렉션 시스템, 실천공동체 내 개인 지식 비서, 유지보수 문서 의미검색. 대화형 접근이 문서 추출보다 사회적 맥락 보존에 유리 | 조직 도입 실증 연구가 매우 적음. 작업자 수용성·동기·용어 정렬 문제 |
| "Code Digital Twin: Empowering LLMs with Tacit Knowledge for Complex Software Development" (arXiv 2503.07967) | 소프트웨어 개발의 암묵지(설계 의도, 변경 이력 배경)를 LLM에 제공하는 구조 | (2차 조사에서 상세 확인) | |

출처: [arXiv 2507.03811](https://arxiv.org/abs/2507.03811), [Springer BISE](https://link.springer.com/article/10.1007/s12599-025-00976-w), [ResearchGate – Industry 5.0 리뷰](https://www.researchgate.net/publication/393130708_Large_Language_Models_for_Tacit_Knowledge_Elicitation_in_Industry_50_A_Literature_Review), [arXiv 2503.07967](https://arxiv.org/html/2503.07967v3), [Atlan – Tacit Knowledge Capture for AI Agents](https://atlan.com/know/ai-agent/data-for-ai/tacit-knowledge-capture-for-ai-agents/), [Enterprise Knowledge – Make tacit knowledge accessible](https://enterprise-knowledge.com/how-to-make-tacit-knowledge-accessible-for-the-enterprise/), [Colrows – Semantic compilation vs document retrieval](https://colrows.com/blogs/capturing-tacit-knowledge-at-scale/)

**포스팅 연결 포인트**: 공통 패턴은 "**에이전트가 인터뷰어가 된다**" — 사람이 문서를 쓰게 하는 대신 에이전트가 묻고, 답의 품질을 평가해 되묻고, 구조화된 산출물(BPMN, 규칙, 체크리스트)을 만든다. 이것이 엡실론델타가 실제로 하는 에이전트 구축 방식(PE 고객의 투자 판단 기준 등)과 연결될 수 있음.

---

## 4. 국내 산업·정책 사례 (2026 상반기~)

### 4.1 산업부 "제조 암묵지 기반 AI모델 개발" (480억, 2026.6~)

- 추경 480억 원. 30개 공정(위험성 높고 구인난 심각한 분야 우선), 과제당 연 16억. 자동차·전자·조선·철강·화학·바이오·기계. 제조기업+AI기업 컨소시엄.
- 데이터 구축 방식: **작업자의 판단 기준과 이유를 수집** + 영상·이미지 데이터 → AI 학습 → 신규 숙련공 교육 및 현장 적용.
- 배경: 제조업 50대 이상 비중 2010년 15.7% → 2020년 30.1%. 암묵지 예시: "기계의 미세한 소리나 진동만으로 설비 이상을 감지".
- 사례: 성원(스테인리스 강관 용접, 육안 판단·조절을 AI 보조), 카라멜라(청년 AI기업).
- 발언: 김성열 산업부 실장 "명장의 암묵지를 보전하고 전수"; 김동선 기아 책임엔지니어 "사업 지속가능성을 위해 노동자 적정 보상체계 필요".
- 출처: [머니투데이](https://www.mt.co.kr/economy/2026/06/12/2026061210401082835), [헤럴드경제](https://biz.heraldcorp.com/article/10726837), [이코노밍글 – 보상 쟁점](https://econmingle.com/economy/manufacturing-tacit-knowledge-ai-project-la/), [이투데이 – 데이터 개방·입법 속도](https://www.etoday.co.kr/news/view/2612668)

### 4.2 HD현대 "조선 AI 마스터(명장) 에이전트"

- 숙련공 암묵지를 **온톨로지**로 구조화해 설계·생산·안전·품질에 걸친 통합 마스터 에이전트로. 3층 구조: 공통(HD Agent) / 도메인(설계·생산 전문 에이전트) / 통합(마스터).
- 김영옥 HD현대 CAIO: "가장 가치 있는 자산은 30년 용접사의 판단인데, 이 지식은 제대로 문서화된 적이 없다."
- 2025.12 지멘스를 설계-생산 통합 플랫폼 파트너로 선정, 2028 배포 시작. 휴머노이드 용접로봇(2026 프로토타입), 디지털트윈 TWINPOS 병행.
- 출처: [아이티데일리](https://www.itdaily.kr/news/articleView.html?idxno=240936), [이투데이 – "족장, 뺑끼 알아듣는 AI"](https://www.etoday.co.kr/news/view/2533387), [뉴스핌 – 정부·HD현대·학계 피지컬 AI 3각 동맹](https://www.newspim.com/news/view/20251120001137), [이데일리 – 조선소 암묵지까지 데이터화](https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=01098806645486312)

### 4.3 원프레딕트 "제조 운영지능" (아시아투데이 2026.9.1)

- 제조업 취업자 438.2만 명(전년 -7.3만), 15~29세 -6.1만, 60세 이상 +5.4만 → "경험의 단절".
- 개념: 숙련자 경험을 데이터·AI·업무 과정으로 구조화해 **조직이 지속적으로 소유하고 학습할 수 있는 자산**으로 전환. 개별 공정 AI 추가가 아니라 현장 판단 결과를 조직 지식으로 축적하는 "AI 네이티브 팩토리".
- 제품: 싸이클론(설비·공정·생산·품질·정비 데이터를 설비/시간/제품/레시피 기준으로 연결), pdx(AI가 제시한 이상 유형·원인을 실제 업무로 연결하고 점검·조치 효과를 기록해 운영 이력으로 축적).
- 출처: [아시아투데이](https://www.asiatoday.co.kr/kn/view.php?key=20260901010000490)

### 4.4 담론 칼럼

- 이원섭 "형식지는 복제돼도 암묵지는 못 옮긴다 … 대한민국, '제조 암묵지'로 피지컬 AI 제국 연다" — 암묵지를 한국 제조업의 방어 가능한 경쟁우위로 보는 국가주의적 프레임. 포스팅에서 인용·비판 대상으로 쓸 수 있음. ([워크투데이](http://www.worktoday.co.kr/news/articleView.html?idxno=87043))

**관찰**: 국내 "암묵지 자산화" 담론은 거의 전부 **제조·피지컬 AI**(용접, 설비 소리, 조선)에 집중되어 있다. **지식노동(투자심사, 법무, 회계, 컨설팅, 영업)의 암묵지**를 에이전트로 자산화하는 이야기는 국내에 거의 없음 → 엡실론델타 포스팅이 채울 수 있는 빈 자리.

---

## 5. 에이전트 실무와의 연결 고리 (기술 측면)

- **Anthropic Agent Skills**: SKILL.md + 참고문서 + 스크립트로 "도메인 전문성, 워크플로, 절차적 지식"을 패키징. 3단계 progressive disclosure(메타데이터 ~50토큰 → 본문 ~500 → 참고자료 2,000+). 조직이 워크플로·컴플라이언스·도메인 전문성을 **재현 가능한 절차로 코드화**한다는 프레이밍. ([Claude 블로그](https://claude.com/blog/building-agents-with-skills-equipping-agents-for-specialized-work), [플랫폼 문서](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview), [agentskills.io](https://agentskills.io/home)) → 즉 Skills는 사실상 "표출화된 암묵지의 컨테이너". 프롬프트 엔지니어링 포스팅에서 다룬 promptDB 관점과 이어짐.
- **MIT 보고서의 "learning gap"**과 에이전트 메모리: 시스템이 피드백을 유지하고 적응하지 않는 것이 실패 원인이라면, 암묵지 자산화는 일회성 추출이 아니라 **에이전트 운영 중 지속 축적되는 메모리/평가 루프**여야 함. (원프레딕트 pdx의 "조치 효과를 기록해 운영 이력으로 축적"과 동일 구조.) 기존 리서치(agent memory: Mem0, Hindsight, Mastra Observational Memory)와 연결 가능.
- **Polanyi's paradox 우회 방식 두 갈래**: (a) 데이터에서 직접 학습(제조: 센서·영상 → 모델), (b) 언어로 표출화(지식노동: 인터뷰 에이전트 → 규칙·체크리스트·Skills). 포스팅에서 이 둘을 구분하면 논지가 선명해짐.

---

## 6. 반론과 쟁점 (포스팅에 반드시 다룰 것)

1. **철학적 한계** — Collins & Thorne, "Large language models and scientific discourse: Where's the intelligence?" (*Synthese*, 2026): LLM은 문자 텍스트에 의존하므로 소수 전문가 집단 내 **구어 담화와 사회화로만 얻어지는 집단적 암묵지(CTK)** 를 가질 수 없다. 주류/비주류 과학의 구분 기준조차 "거의 전적으로 암묵적". ([Springer](https://link.springer.com/article/10.1007/s11229-026-05531-y)) → "자산화"는 CTK 전체가 아니라 Relational 층의 표출화 + Somatic 층의 데이터화에 한정된다는 것을 인정하는 게 오히려 설득력을 높임.
2. **보상·소유권** — 한국노총: "데이터를 제공한 노동자에 대한 권리 보장과 보상 체계가 선행해야". 정부 공고에 보상 기준·성과 공유 방안 미명시. 일본 건설업, HD현대 모두 지식 소유권·대가 산정 기준 미정립. ([이코노밍글](https://econmingle.com/economy/manufacturing-tacit-knowledge-ai-project-la/), [다음뉴스 – "기업만 이익 독점" 비판](https://v.daum.net/v/PSqDrvMVWj)) → 지식노동에서도 동일: 시니어 심사역의 판단 기준을 에이전트에 넣으면 그 사람의 협상력은 어떻게 되는가.
3. **"완전한 문서화" 환상** — GenAI SECI의 Digital Fragmented Knowledge 개념이 시사하듯, 실무에서 요구해야 하는 건 완전한 매뉴얼이 아니라 단편의 축적 + 인간의 symbol grounding. 그리고 Hybrid SECI의 지적처럼 대화형 AI의 "공동화"는 경험적 깊이가 없다.
4. **Autor의 직업 양극화**: 암묵지가 자산화되면 Polanyi가 지켜주던 일자리 방어선이 어디까지 밀리는가.

---

## 7. 포스팅 앵글 후보

A. **"AX가 안 되는 이유는 모델이 아니라 당신 머릿속에 있다"** — MIT 95%/McKinsey 6%를 도입부로, 실패 원인이 "learning gap = 조직 암묵지가 시스템에 없음"임을 보이고, 에이전트가 인터뷰어가 되어 암묵지를 Skills/규칙/메모리로 자산화하는 방법론 제시. (프롬프트 엔지니어링 포스팅과 톤 일관, 실무 중심)

B. **"암묵지 자산화, 제조업만의 이야기가 아니다"** — 정부 480억·HD현대·원프레딕트가 전부 제조인데, 사실 지식노동(PE 투자심사, 법무, 회계)의 암묵지가 더 빨리 자산화되고 있다. Collins의 3층 구분으로 "무엇이 자산화 가능한가"를 정리. (국내 담론의 빈 자리 공략)

C. **"Polanyi's Paradox는 깨졌는가"** — 철학적 프레임 중심. 1966 Polanyi → 2014 Autor → 2026 LLM. GenAI SECI, Hybrid SECI, Collins&Thorne을 종합해 "무엇은 깨졌고 무엇은 남았는가". (사고 실험형, 조회수보다 깊이)

D. **A+B 결합** — 도입부는 A(실패 통계), 본론은 B(제조 vs 지식노동, 3층 구분), 결론에서 엡실론델타의 에이전트 구축 방식(에이전트 인터뷰 → Skills → 운영 중 메모리 축적)으로 마무리. 가장 자연스럽지만 길어질 위험.

---

## 8. 2차 조사에서 확인할 것

- 인공지능 기본계획(2026~2028) 원문에서 "암묵지/현장 데이터/산업 AI" 관련 문구.
- Uchihira GenAI SECI 논문 원문의 그림(3층 연속체, Digital Fragmented Knowledge 도식) — 포스팅 그림 재구성용.
- Code Digital Twin(arXiv 2503.07967) 상세 — 소프트웨어 암묵지 사례로 개발자 독자층에 어필.
- Collins & Thorne(Synthese 2026) 원문의 LLM 관련 논증 부분 직접 확인(현재 요약은 2차 자료).
- HD현대 "명장 에이전트" 이투데이 인터뷰("족장, 뺑끼 알아듣는 AI") 원문 — 현장 용어 학습 사례 인용용.
- MIT NANDA 보고서 원문(Forbes는 403) — 정확한 수치 재확인. buy vs build: 2차 자료(Dataiku)는 "외부 파트너십이 내부 구축보다 약 2배 성공"으로 요약. 정확한 비율(흔히 67% vs 33%로 인용됨)은 원문에서 확인 필요.
- 지식노동 분야 국내 사례(금융·법무 에이전트 도입) — 이번 서치에서는 거의 안 나옴. 영문 키워드로 재탐색 필요.

---

## 전체 출처 목록

### AX 담론·정책
- [MSAP.ai – AX vs DX](https://www.msap.ai/ax/ax-vs-dx/) / [MSAP.ai – AX란 무엇인가](https://www.msap.ai/ax/what-is-ax/)
- [flex – AX 뜻과 핵심요소](https://flex.team/blog/2025/10/27/ax)
- [카카오벤처스 – 'AX'란 무엇인가](https://www.kakao.vc/blog/ax-ai-transition-strategy)
- [이글루코퍼레이션 – AI 전환(AX)의 시대](https://www.igloo.co.kr/security-information/ai-%EC%A0%84%ED%99%98ax%EC%9D%98-%EC%8B%9C%EB%8C%80-%EC%9A%B0%EB%A6%AC%EA%B0%80-%EB%A7%88%EC%A3%BC%ED%95%9C-%ED%98%84%EC%8B%A4%EA%B3%BC-%EC%A7%88%EB%AC%B8%EB%93%A4/)
- [클로브 – AX DX 차이](https://clobe.ai/blog/ax-vs-dx-sme-strategy) / [CJ대한통운 더 운반 – 2026 AX 트렌드](https://www.unban.ai/blog/ax-trend-complete-guide)
- [GeekNews – 2026년 전망 종합(35개 자료)](https://news.hada.io/topic?id=25465)
- [다음뉴스 – 정부 AX 사업 통합 공고](https://v.daum.net/v/20260312110035947)
- [기업마당 – 2026 AX 원스톱 바우처](https://www.bizinfo.go.kr/sii/siia/selectSIIA200Detail.do?pblancId=PBLN_000000000120085)
- [인공지능 기본계획 2026~2028 PDF](https://smartcity.go.kr/wp-content/uploads/2026/03/%EC%95%88%EA%B1%B41%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%ED%96%89%EB%8F%99%EA%B3%84%ED%9A%8D%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%EA%B8%B0%EB%B3%B8%EA%B3%84%ED%9A%8D20262028.pdf)

### 실패/성공 통계
- [Mind the Product – MIT 2025 AI Report](https://www.mindtheproduct.com/why-most-ai-products-fail-key-findings-from-mits-2025-ai-report/)
- [Forbes – MIT 95% fail, friction](https://www.forbes.com/sites/jasonsnyder/2025/08/26/mit-finds-95-of-genai-pilots-fail-because-companies-avoid-friction/)
- [Forbes – What the 5% do right](https://www.forbes.com/sites/jaimecatmull/2025/08/22/mit-says-95-of-enterprise-ai-failsheres-what-the-5-are-doing-right/)
- [McKinsey – The state of AI (2026)](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai)
- [아주경제 – AX에 실패하는 기업들](https://www.ajunews.com/view/20260511141644195)
- [KDI – 무협 AX 우수사례 보고서](https://eiec.kdi.re.kr/policy/domesticView.do?ac=0000200330&pg=&pp=20&issus=M)
- [Salesforce KR – AX 실패 5가지 이유](https://www.salesforce.com/kr/blog/ai-transformation-ax/)
- [벤처스퀘어 – "AI 도입은 끝났다"](https://www.venturesquare.net/1104216)

### 암묵지 이론
- [Wikipedia – Polanyi's paradox](https://en.wikipedia.org/wiki/Polanyi%27s_paradox)
- [나무위키 – SECI 모델](https://namu.wiki/w/SECI%20%EB%AA%A8%EB%8D%B8)
- [KIRD – 암묵지 발현과 공유](https://www.kird.re.kr/newsletter/html/vol122/sub02.html)
- [Collins – Tacit and Explicit Knowledge (U. Chicago Press)](https://press.uchicago.edu/ucp/books/book/chicago/T/bo8461024.html)
- [Cynefin – What We Cannot Say](https://thecynefin.co/what-we-cannot-say/)
- [MDPI – AI-Enabled Tacit Knowledge Co-Evolution](https://www.mdpi.com/2673-9585/6/1/1)

### GenAI × 지식경영 학술
- [arXiv 2603.21866 – GenAI SECI Model (Uchihira et al.)](https://arxiv.org/pdf/2603.21866)
- [RealKM – Rethinking SECI for GenAI](https://realkm.com/2026/06/05/rethinking-the-seci-model-for-genai-three-perspectives-including-one-from-japan/)
- [ScienceDirect – Artificial knowledge generation (Cerchione et al.)](https://www.sciencedirect.com/science/article/pii/S2444569X25002112)
- [Springer Synthese – Collins & Thorne, LLMs and scientific discourse](https://link.springer.com/article/10.1007/s11229-026-05531-y)

### LLM 기반 암묵지 추출
- [arXiv 2507.03811 – Zuin et al.](https://arxiv.org/abs/2507.03811)
- [Springer BISE – Schinckus et al., PKAI](https://link.springer.com/article/10.1007/s12599-025-00976-w)
- [ResearchGate – Rank et al., Industry 5.0 review](https://www.researchgate.net/publication/393130708_Large_Language_Models_for_Tacit_Knowledge_Elicitation_in_Industry_50_A_Literature_Review)
- [arXiv 2503.07967 – Code Digital Twin](https://arxiv.org/html/2503.07967v3)
- [Atlan – Tacit Knowledge Capture](https://atlan.com/know/ai-agent/data-for-ai/tacit-knowledge-capture-for-ai-agents/)
- [Enterprise Knowledge](https://enterprise-knowledge.com/how-to-make-tacit-knowledge-accessible-for-the-enterprise/) / [Colrows](https://colrows.com/blogs/capturing-tacit-knowledge-at-scale/)

### 국내 산업 사례
- [머니투데이 – 암묵지 데이터 구축 480억](https://www.mt.co.kr/economy/2026/06/12/2026061210401082835)
- [헤럴드경제 – 산업부 제조 암묵지 AI모델](https://biz.heraldcorp.com/article/10726837)
- [이코노밍글 – 숙련공 노하우, 보상은 누가](https://econmingle.com/economy/manufacturing-tacit-knowledge-ai-project-la/)
- [다음뉴스 – "기업만 이익 독점" 비판](https://v.daum.net/v/PSqDrvMVWj)
- [아시아투데이 – 제조 운영지능(원프레딕트)](https://www.asiatoday.co.kr/kn/view.php?key=20260901010000490)
- [아이티데일리 – HD현대 조선 마스터 에이전트](https://www.itdaily.kr/news/articleView.html?idxno=240936)
- [이투데이 – "족장, 뺑끼 알아듣는 AI"](https://www.etoday.co.kr/news/view/2533387)
- [뉴스핌 – 조선 AI 대전환 3각 동맹](https://www.newspim.com/news/view/20251120001137)
- [이데일리 – 조선소 암묵지 데이터화](https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=01098806645486312)
- [워크투데이 – 이원섭 칼럼](http://www.worktoday.co.kr/news/articleView.html?idxno=87043)

### 에이전트 기술
- [Claude 블로그 – Building Agents with Skills](https://claude.com/blog/building-agents-with-skills-equipping-agents-for-specialized-work)
- [Claude 플랫폼 문서 – Agent Skills](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview)
- [agentskills.io](https://agentskills.io/home)
