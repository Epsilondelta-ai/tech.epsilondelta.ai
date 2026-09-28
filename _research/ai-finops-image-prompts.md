# AI FinOps 이미지 제작

- 도구: 내장 imagegen(일러스트), 직접 작성 SVG(차트·도해)
- 크기: SVG 800×450, 일러스트 폭 800px, 원본 비율 유지
- 캡션 없음. 본문 각 H2에 이미지 한 장씩 삽입.
- 숫자는 본문의 가상 계산. Notion 도해는 공개 구현 설명을 단순화.

## 배치

- 들어가며: `thumbnail.webp`
- 사용료는 반값인데, 한 건 처리 비용은 올라갔습니다: `chart-cost-per-completed-task.svg`
- Notion은 바뀌지 않은 문서를 다시 계산하고 있었습니다: `diagram-incremental-indexing.svg`
- 모든 일을 가장 싼 모델에 맡기면 절약할 수 있을까요?: `diagram-model-routing.svg`
- 같은 내용을 매번 읽히고, 모든 답을 즉시 받고 있지는 않나요?: `diagram-cache-and-batch.svg`
- 청구서는 한 장인데, 누가 무슨 일에 썼는지 모릅니다: `illustration-shared-cost-review.webp`
- “예산 초과 알림”만 켜두면 에이전트가 멈출까요?: `diagram-budget-control.svg`
- 우리 회사에서는 어떤 업무부터 계산해볼까요?: `diagram-controlled-pilot.svg`
- 나가며: `illustration-workflow-workshop.webp`

## 생성 프롬프트

### thumbnail

Use case: illustration-story. Create a wide 16:9 editorial illustration for a Korean executive tech blog about AI FinOps. Core message: cheap AI calls can create expensive human rework. Two adjacent areas of same bright contemporary office: an engineer on left pleasantly examines a small AI invoice and downward teal cost arrow; a procurement specialist on right has many comparison sheets marked for corrections and a large clock, visibly puzzled but professional. Hands anatomically natural, papers oriented toward their users. A visual connection of generated documents between them. Large Korean labels only above each area: 'AI 사용료 ↓' and '검토·수정 시간 ↑'. Warm ivory background, charcoal linework, restrained teal and terracotta, elegant hand-painted gouache editorial illustration, adult proportions, not cartoon robots. Clear central visual argument, minimal props, readable when downscaled to 800px wide. No extra text, no logos, no watermark. Landscape.

### illustration-shared-cost-review

Use case: illustration-story. Wide 16:9 Korean enterprise tech blog editorial illustration. Three Korean adult colleagues from engineering, purchasing operations and finance sit on three sides of a meeting table and jointly inspect a large cost ledger and a corrected quotation comparison, showing AI cost accountability across teams rather than isolated invoice tracking. One shared upright display visible front-on to viewer, turned so participants also see it, has simple three labeled categories '모델·도구', '검토 시간', '완료 업무', no fake numbers. Different ages and genders, professional collaborative expressions, natural arm positions, no crossed disembodied hands, paper print oriented toward person reading. Hand-painted gouache editorial aesthetic, ivory daylight, teal and terracotta accents, charcoal lines, minimal scene, no corporate logos, no caption, landscape.

### illustration-workflow-workshop

Use case: illustration-story. Create a wide 16:9 editorial illustration for closing of a Korean AI FinOps executive blog. A purchasing specialist and an AI engineer stand at a whiteboard planning ONE real quotation comparison workflow together. Board large readable Korean stages '견적서' → 'AI 비교' → '검토' → '완료', with two small sticky notes below '품질 기준' and '비용·시간'. Purchasing specialist holds a quotation folder and points naturally at '검토', engineer writes a check mark next to the final stage. Both adults, one man one woman, natural anatomy and hands, board physically faces viewer at mild angle, warm bright office. Hand-painted gouache, charcoal contours, muted teal/terracotta and ivory, matching professional editorial illustration, minimal props, no logos, no additional text, no watermark. Clear story of defining completion and checking costs jointly, not a generic handshake.
