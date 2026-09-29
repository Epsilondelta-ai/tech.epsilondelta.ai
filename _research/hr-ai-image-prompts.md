# HR AI 이미지 제작 기록

- 도구: 내장 imagegen(일러스트 3장), 직접 작성 SVG(도해 6장).
- 파일 위치: content/posts/geoff-25-hr-ai/
- 9개 H2 섹션마다 1장. 본문 캡션 없음, 설명형 alt 사용.
- SVG 800×450. WebP 폭800px, 원본 종횡비 유지. 블로그 높이500px 기준도 충족.
- 도해는 본문의 절차·권한·측정 범위를 설명. 실제 측정값 없는 성과 막대그래프는 만들지 않음.
- Cemex 사례 도해와 일반적인 구성 예시를 구분함.

## 배치

- 들어가며: `thumbnail.webp`
- HR AI에게 어떤 일을 맡길까요?: `diagram-hr-task-connections.svg`
- 안경 지원비를 물었더니, 신청서까지 받았습니다: `diagram-cemex-benefits-request.svg`
- 같은 질문에도 직원마다 답이 달라집니다: `diagram-policy-and-live-data.svg`
- 신청 버튼을 누른 뒤에도 할 일이 남습니다: `diagram-request-state.svg`
- 인사팀 계정을 빌려주면 편할 것 같지만: `diagram-user-authorization.svg`
- 사람에게 넘길 때, 처음부터 다시 묻게 하지 않으려면: `illustration-contextual-handoff.webp`
- 챗봇의 답변 수보다, 다시 걸려온 전화를 보겠습니다: `diagram-completion-metrics.svg`
- 나가며: `illustration-hr-workflow-workshop.webp`

## 일러스트 생성 프롬프트

### thumbnail

Use case: illustration-story. Wide landscape 16:9 editorial illustration for Korean business tech blog HR AI. Clear visual argument: chatbot has answered, but employee still has to call HR for the actual employment certificate. In a bright modern office, young adult Korean employee at left holding a phone with tired puzzled expression, open laptop with BACK facing viewer blank. Beside him a large detached chat UI inset with exact Korean '인사팀에 문의하세요'. On right a middle-aged Korean HR professional on telephone starting a document issuance task, document icon in a tray and a clock nearby. The two communicate by phone, separated workstations, no physical touching. Large short editorial labels above zones exactly '답변 완료' on left and '발급은 아직' on right. Warm ivory, muted teal and terracotta, painted gouache magazine illustration, restrained charcoal outlines, adult proportions, not chibi or infographic only. Minimal props, correct hands and phone grip, no text on laptop backs, no gibberish additional lettering, no numbers, no logos, no watermark. Meaningful concept immediately understandable at800px width.

### illustration-contextual-handoff

Use case: illustration-story. Wide landscape16:9 warm gouache editorial illustration for Korean HR AI blog, adult realistic simplified proportions and charcoal outlines, ivory daylight, muted teal and terracotta. Two Korean adult people in a private HR consultation, employee at left, HR advisor at right. Employee has relaxed attentive expression rather than repeating an entire story. Advisor consults an upright monitor visibly angled toward BOTH advisor and viewer displaying a simple summary card with only Korean three labels '요청 내용', '확인한 기록', '남은 질문'. Three abstract gray lines below labels, no personal details. Advisor gently points to summary and listens. Physically plausible screen viewpoint, no writing on monitor backs. No unnecessary paper, no floating arms, no extra fingers, no medical or salary details. Human handoff with context is main action, not generic handshake. No other text, captions, logos or watermarks.

### illustration-hr-workflow-workshop

Use case: illustration-story. Landscape16:9 editorial gouache illustration for final section Korean HR AI blog. HR practitioner and AI engineer jointly examine a real employee request workflow at whiteboard. One Korean woman HR specialist with bob hair and cream blouse holds a plain folder; Korean man engineer in muted teal shirt points to one step on board. Distinct natural poses, hands simple anatomically sound. Board shows FOUR readable Korean labels in sequence '본인 확인' → '신청' → '승인' → '결과 확인'. Paper-like note under approval reads '예외는 담당자에게'. Show thoughtful cooperative working session, not a celebratory deal or generic meeting. Warm bright office, terracotta accents, charcoal linework, restrained painterly texture, non-chibi adult figures, matching professional magazine illustration, no additional labels, numbers, logos, captions or watermark. Board text physically faces audience and people stand beside it.
