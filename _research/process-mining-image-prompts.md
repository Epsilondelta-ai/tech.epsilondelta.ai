# Process mining visual production

2026-09-20. Built-in imagegen for five raster illustrations; WebP exports 800×451. Four SVGs fit within 800×500. No captions. Original generated PNGs remain in Codex generated_images. Diagram sources and editable Excalidraw files are in `_workspace/process-mining-visuals-2026-09-20/`.

## Asset mapping

- 들어가며: thumbnail.webp — 초안 작성은 3분이지만 검토와 승인 때문에 고객 전달은 늦어지는 가상 업무 장면
- 매뉴얼대로라면 벌써 끝났어야 하는데: illustration-real-workflow.webp — 매뉴얼의 순서와 검토·수정이 반복되는 실제 업무 경로를 비교하는 담당자
- 시스템에는 무엇이 남아 있어야 할까?: figure-case-timeline.svg — 가상 견적 Q-101의 초안 작성 3분과 요청부터 발송까지 7시간을 비교한 시간축
- 기록을 모으면 어떻게 업무 흐름이 나올까?: figure-object-relations.svg — 주문 A의 두 배송과 주문 A·B를 묶는 통합 청구서의 관계 예시
- Hexion은 출하까지 걸리는 시간을 줄였습니다: chart-hexion.svg — Celonis 공개 Hexion 사례: 신용 보류 해제부터 출하까지 약 11일에서 5일로 단축
- Cosentino는 발견한 병목에 AI를 투입했습니다: illustration-credit-review.webp — 주문·지급·신용 정보를 바탕으로 AI의 보류 해제 권고와 근거를 검토하는 업무 예시
- 오래 걸리는 곳마다 AI를 넣어야 할까요?: figure-match-intervention.svg — 조건 누락·자료 조회 지연·승인 대기에 따라 다른 개선 수단을 선택하는 도해
- 정말 빨라졌는지는 어디에서 확인할까?: illustration-measure-outcome.webp — 고객 전달 여부와 재작업·미완료 건을 함께 확인하는 담당자들
- 나가며: illustration-workflow-workshop.webp — 지연된 업무 한 건의 기록과 현업 판단을 검토하며 개선을 논의하는 실무자들

## Data provenance

- Thumbnail: fictional scenario in post, 3 minutes drafting versus three days customer wait. Not a measured customer result.
- Timeline: fictional Q-101; same day09:00–16:00, drafting09:02–09:05, next review14:00. Proportional scale96px/hour; 295-minute gap472px; 3-minute drafting4.8px.
- Hexion: credit hold release to shipment, approximately11 days to5 days. Source: https://www.celonis.com/solutions/stories/hexion-supply-chain-process-mining . Axis starts0; scale43px/day.
- Object relations and intervention mapping: explanatory constructions from post, not customer implementation diagrams.
- Credit review illustration is a generic representation, not a photograph of Cosentino staff or software.

## Raster prompts

### thumbnail

Create a polished editorial illustration for a Korean executive tech blog, landscape 16:9, warm cream paper texture, teal navy and muted coral accents, elegant hand-painted gouache with clean readable forms, professional adult people diverse ages, NOT chibi comic, bright business environment. No decorative robots or meaningless digital glow. Natural hand anatomy and coherent paper/screen orientation. Korean labels only as specified, no extra lettering or invented statistics. Concept: an office author quickly finishes a quotation draft at left, but a document queue awaits review/approval in the middle and a customer at right waits checking a phone. Show one coherent business handoff story, not disconnected mood art. Large exact headline "작성은 3분, 고객은 사흘째 대기". Small label "가상 업무 예시". Left sign "초안 완료" middle "검토 · 승인 대기" right "고객 전달은 아직".

### illustration-real-workflow

Create a polished editorial illustration for a Korean executive tech blog, landscape 16:9, warm cream paper texture, teal navy and muted coral accents, elegant hand-painted gouache with clean readable forms, professional adult people diverse ages, NOT chibi comic, bright business environment. No decorative robots or meaningless digital glow. Natural hand anatomy and coherent paper/screen orientation. Korean labels only as specified, no extra lettering or invented statistics. Two staff compare a neat simple printed manual with a real board of sticky-note workflow including a clear backward arrow from review to revision. The actual office discussion is the focus. Only headings "매뉴얼의 순서" over simple linear diagram and "실제 처리 경로" over board with loop. A woman practitioner points to a returned document and older male colleague studies it. No numerical data.

### illustration-credit-review

Create a polished editorial illustration for a Korean executive tech blog, landscape 16:9, warm cream paper texture, teal navy and muted coral accents, elegant hand-painted gouache with clean readable forms, professional adult people diverse ages, NOT chibi comic, bright business environment. No decorative robots or meaningless digital glow. Natural hand anatomy and coherent paper/screen orientation. Korean labels only as specified, no extra lettering or invented statistics. Illustrative—not an actual company photograph—credit manager reviewing an AI recommendation for a blocked building-material order. On desk a restrained sample stone tile, screen showing three source cards "주문 정보" "지급 이력" "신용 정보", below "AI 권고 · 근거", final human review two options "해제" "추가 조사". Main adult analyst thoughtfully checks evidence, coworker nearby holds record. No brand logos, no all-orders automatic approval, no numbers.

### illustration-measure-outcome

Create a polished editorial illustration for a Korean executive tech blog, landscape 16:9, warm cream paper texture, teal navy and muted coral accents, elegant hand-painted gouache with clean readable forms, professional adult people diverse ages, NOT chibi comic, bright business environment. No decorative robots or meaningless digital glow. Natural hand anatomy and coherent paper/screen orientation. Korean labels only as specified, no extra lettering or invented statistics. Operations manager and customer-facing colleague review whether a quotation actually reached customer. Visible board with three readable headings "고객 전달까지" "재작업" "미완료 건", symbolic clock, returned document, pending tray icons respectively, no invented dashboard statistics. Worker compares sent message confirmation to open case folder. Show meaningful verification rather than celebration. No random graph.

### illustration-workflow-workshop

Create a polished editorial illustration for a Korean executive tech blog, landscape 16:9, warm cream paper texture, teal navy and muted coral accents, elegant hand-painted gouache with clean readable forms, professional adult people diverse ages, NOT chibi comic, bright business environment. No decorative robots or meaningless digital glow. Natural hand anatomy and coherent paper/screen orientation. Korean labels only as specified, no extra lettering or invented statistics. Three professionals from operations and engineering gather around a desk, investigating ONE delayed quotation case. Big card "지연된 업무 한 건" and three connected table cards "기록 확인" "현업의 판단" "개선 후 검증". Person explaining a specific returned report, engineer taking notes on laptop, manager listening. Papers oriented toward users, hands simple and correct. No company logo, no numeric claims.

## Verification

All generated raster images and rendered SVG previews visually inspected. Timeline values and chart bar proportions checked against post. Body text and draft status retained.
