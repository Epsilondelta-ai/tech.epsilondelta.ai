# FDE 포스트 이미지 제작 기록

- 작성일: 2026-09-07
- 대상: `content/posts/geoff-7-forward-deployed-engineer/index.md`
- 생성 방식: 기본 내장 image_gen 도구로 서사형 일러스트 3종 생성. 설명 도해 3종은 기존 블로그의 SVG 방식으로 작성.
- 목적: FDE의 현업 공동개발, 업무와 시스템의 차이, 구현 뒤 운영 지식이 남는다는 내용을 설명한다.
- 표현: 밝은 아이보리 바탕, 잉크 선과 과슈·종이 질감, 네이비·블루·틸·테라코타. 실제 고객 현장 사진이나 실제 제품 화면을 재현한 것으로 표현하지 않는다.

## 이미지 구성

| 파일 | 배치 | 설명 역할 |
|---|---|---|
| thumbnail.jpg | 대표 이미지·본문 첫머리 | 품질검사 현장의 조건을 현업·엔지니어·고객 운영자가 함께 소프트웨어로 옮기는 장면 |
| figure-fde-cycle.svg | FDE 정의 뒤 | 현업 관찰부터 구현·검증·운영 인계와 피드백의 순환 |
| illustration-kitchen.webp | 주방 비유 뒤 | 정상인 장비와 실제 업무 동선의 차이를 관찰하는 장면 |
| illustration-field-diagnostics.webp | Jabil 사례 뒤 | 제품을 확인하는 기술자와 소프트웨어를 함께 고치는 엔지니어 |
| figure-workflow.svg | 현업의 말이 코드가 되는 과정 | Tool·Skill·Memory와 사람 승인·실행 검증의 관계 |
| figure-handover.svg | 엔지니어가 떠난 뒤 남길 것 | 고객의 업무 기록과 구축팀의 재사용 지식, 고객 운영 역량을 구분 |

## 생성 프롬프트

### thumbnail

```text
Use case: illustration-story
Asset type: 3:2 landscape editorial thumbnail for a Korean enterprise AI blog article, "What is an FDE? Why AI engineers work inside the customer's operations."
Primary request: Create a thoughtful, visually concrete editorial illustration that communicates an engineer working alongside frontline staff to turn their real operational rules into working AI software, leaving the customer able to operate it.
Scene: A bright, unbranded manufacturing workshop with a shared workbench physically inside the operational space. Three people collaborate as peers: a frontline quality specialist points from an inspection clipboard toward a crate of components bearing an amber pause/quality-hold symbol; a software engineer at the same table translates that observation into a simple branching workflow on a laptop; a customer operations colleague tests the workflow on a desktop screen showing a small approved checklist. An open, well-organized operating manual beside the colleague suggests the know-how stays with the customer. All three look at the work, not the viewer.
Composition: One unified scene, not a triptych or diagram. Medium-wide cutaway view with the shared table and people as the strong center. The quality-hold crate, the small workflow screen, and the customer-owned operating manual must all remain identifiable at thumbnail size. Keep background machinery minimal and subordinate. Generous clear margins.
Style: Premium magazine editorial illustration with precise ink outlines, simplified human anatomy, subtle gouache and paper texture, warm ivory background, deep navy, muted blue, teal and terracotta accents. Bright natural daylight. Tactile and humane, not glossy 3D.
Constraints: No text, no letters, no numbers, no logos, no watermark. No robot, brain, holographic panels, neural-network ball, handshake, floating cloud, generic office mood, or photorealistic claim about an actual customer site. Avoid clutter and tiny UI details. Show a practical shared problem being solved.
```

### kitchen

```text
Use case: illustration-story
Asset type: 3:2 landscape supporting illustration for a Korean business technology article
Primary request: Illustrate the article's kitchen analogy: equipment can work correctly while the actual workflow remains obstructed, and observing the work reveals what a blueprint misses.
Scene: A compact restaurant kitchen during lunch preparation, bright and clean. A refrigerator door opens across the narrow walking route and temporarily blocks a cook carrying a tray. A second cook needs the same small prep station, visibly waiting with a mixing bowl. At the edge of the kitchen, a planner in a plain navy shirt compares a simple kitchen floor plan with what the cooks are actually doing, taking a pencil note. This is a calm, recognizable operational bottleneck, not a disaster.
Composition: Slightly elevated three-quarter view makes the refrigerator door, obstructed aisle, shared prep station, two cooks, and observer clear in a single scene. Real objects and human gestures explain the story; no diagram arrows, no panels, no data cards. Comfortable negative space around the vignette.
Style: Premium editorial ink and gouache illustration on warm ivory textured paper; restrained navy, teal, muted blue, terracotta and natural steel colors. Bright diffuse daylight, natural proportions, subtle expressive body language. Match a polished enterprise blog, not a children's cartoon.
Constraints: No text, no letters, no numbers, no logos, no watermark, no floating symbols, no flames or accidents, no chaotic pile of props. Do not portray a real restaurant. The key is the mismatch between planned layout and actual movement.
```

### diagnostics

```text
Use case: illustration-story
Asset type: 3:2 landscape supporting illustration for the manufacturing example in an enterprise AI blog
Primary request: Show an experienced manufacturing technician and a software engineer co-developing a diagnostic assistant at the actual workbench. Make the technician's knowledge entering the software visible through concrete actions.
Scene: Unbranded electronics inspection bench in a clean factory. An experienced technician points to a specific component on a circuit-board assembly with a probe while explaining the issue; the software engineer sits beside the technician and revises a diagnostic checklist on a laptop. A handheld barcode scanner and the product's simple barcode label are visible near the assembly. A nearby tablet displays a minimal document page with a source-document icon and check marks. A short paper note with a hand-drawn component sketch sits next to the laptop, linking the explanation to the revised procedure. Tools and electronics are organized and plausible.
Composition: Medium-close view centered on the board, pointing hand, and shared laptop. The two people lean into the same problem as equal collaborators. No factory-wide dashboard, no big process chart. Their gaze and hands carry the story.
Style: Editorial magazine illustration, crisp ink outlines and lightly textured gouache, warm off-white backdrop, deep navy, teal, muted blue and restrained terracotta accents. Bright work lighting; humane and detailed enough to recognize the task, without photorealism.
Constraints: No words, letters, numbers, company logos, or watermark. No robot or futuristic hologram. Do not depict or claim an actual Jabil factory or its proprietary interface. This is explicitly a conceptual illustration of the published workflow. Avoid arbitrary metrics or growth charts.
```

## 선택된 원본

- thumbnail: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-c9aa3900-c1e7-4ad1-9f4c-fa1b6455c082.png`
- kitchen: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-4f27ccd7-7f2f-4961-a3fb-48131130c003.png`
- diagnostics: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-4468d991-e29e-4a9b-a932-cf5da59e27a5.png`

## 검수 항목

- 썸네일에서 현업 문제·공동 구현·고객 운영의 연결이 식별되는가?
- 주방 그림에 동선이 막히는 이유가 보이는가?
- 제조 그림이 실재 고객의 시설·인터페이스·성과를 임의로 주장하지 않는가?
- 도해에서 Tool·Skill·Memory·승인의 역할과 화살표가 글의 설명과 일치하는가?
- 고객의 업무 데이터를 다른 고객에게 자동으로 공유하는 인상을 주지 않는가?
- 한국어 글자 잘림, 잘못된 손·도구·시선이 없는가?
- 본문의 이미지 경로와 대표·OG 이미지가 실제 페이지 자산을 가리키는가?

내장 도구 원본은 기본 생성 디렉터리에 남고, 선택된 결과의 웹용 파일을 포스트 디렉터리에 저장했다. 본문 일러스트 2종은 1536×1024 크기를 유지한 채 WebP 품질 88로 변환했다. 썸네일은 같은 크기의 JPEG 품질 88로 변환해 목록과 OG 이미지에 사용한다.
