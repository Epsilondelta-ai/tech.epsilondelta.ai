# Agent Skills 포스트 이미지 제작 기록

- 제작일: 2026-09-08
- 대상: `content/posts/geoff-8-agent-skills/index.md`
- 방식: 내장 `image_gen`으로 썸네일·실사풍 이미지·서사형 일러스트 3종 생성. 한글과 관계를 정확하게 표현할 설명 도해 3종은 기존 블로그의 SVG 형식을 따라 직접 작성.
- 실제 회사의 인물·시설·제품 화면을 재현하지 않았다. 실사풍 이미지는 본문 캡션에 AI로 제작한 가상 업무 장면임을 명시했다.
- 본문 문장은 보존하고 이미지·캡션·대표 이미지 메타데이터만 추가했다. `draft = true`를 유지했다.
- 이미지 추가 전 원고: `_workspace/2026-09-08-agent-skills-images/index-before-images.md`. 이전 윤문 산출물로 현재 index.md 전체를 덮어쓰면 이미지가 사라지므로 주의한다.

## 배치와 역할

| 파일 | 배치 | 설명 목적 |
|---|---|---|
| thumbnail.jpg | 목록·OG·본문 첫머리 | 숙련자의 업무 방법·자료·도구를 스킬로 묶고 에이전트가 활용한 결과를 사람이 검토한다는 전체 논지 |
| figure-skill-loading.svg | Skill 개념 설명 뒤 | 이름·설명으로 선택 → 지침 읽기 → 필요한 자료 사용. 설치·선택·성공을 구분 |
| photo-skill-workshop.webp | 업무 범위와 사례 관찰 설명 뒤 | 정상 처리·반려 견적 및 계약을 함께 보고 판단 기준을 꺼내는 가상 현업 장면 |
| figure-quote-workflow.svg | 스킬 안팎의 역할 설명 뒤 | Skill·조회 Tool·검사 코드·양식을 함께 구성하고 미확인 내용이 있으면 보류 |
| illustration-stale-policy.webp | 오래된 지침의 실패 예시 뒤 | 새 정책 v2가 있어도 계속 읽는 지침이 v1이면 잘못된 결과가 반복될 수 있음 |
| figure-approval-boundary.svg | 승인 통제 설명 뒤 | 자연어 지침과 업무 시스템의 실행 검사 차이. 승인 상태와 내용을 확인하고 발송·보류 분기 |

## 내장 도구에 전달한 최종 프롬프트

### thumbnail

```text
Use case: illustration-story.
Asset type: wide editorial cover for a Korean business technology article titled "Agent Skills: teaching a general-purpose agent how our company works". Create one finished landscape image, approximately 16:9, 2048x1152.
Primary request: Visually explain that verified human work procedures, examples, templates and small tools are packaged into a reusable Skill that an AI agent consults to prepare work for human review. This is NOT model training or uploading knowledge into a robot brain.
Scene and composition: A bright, refined tactile editorial illustration, with one large open document folder as the strong central focal point. Its front tab reads exactly "SKILL.md". Inside the folder are four clearly different oversize sheets: a procedural checklist, an annotated example quotation, a spreadsheet template, and a tiny code-bracket tool card. On one side a human business expert's hands organize and annotate these materials; on the other side a restrained desktop agent interface shows the same folder opened and a single quotation draft coming out, with another human hand reviewing the draft with a pencil. These three elements must read in one glance at thumbnail size. Use gentle paper trails to connect, not a dense flowchart. The desktop should be a clearly generic agent interface, not a branded screenshot. Human agency and review remain visible.
Style: premium hand-painted gouache and cut-paper editorial illustration, crisp bold shapes, subtle paper grain, intelligent restrained business-magazine art, warm ivory background, deep ink and muted teal with small amber accents, welcoming daylight. No dark office, neon, glowing brains, robot mascot, hologram, circuit maze, unrelated cityscape, logos or fake real company evidence.
Typography: large simple legible title "AGENT SKILLS" in the open upper region, and "SKILL.md" on the folder tab. No other readable text, no tiny fake paragraphs, no gibberish. Documents use lines, checkboxes and table marks. Keep all main objects and text within a generous safe margin for cropping. The cover must primarily communicate the work-package concept, not just atmosphere.
```

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-ec77ecee-e31d-4cbe-b2f1-c67f88be7a86.png`

### workshop

```text
Use case: photorealistic-natural.
Asset type: in-article supporting editorial image for a Korean executive audience; one landscape 16:9 image, approximately 2048x1152.
Primary request: Make the article's concrete method visible: a domain expert and a technical colleague learn what belongs in an Agent Skill by comparing a good quotation and a returned quotation, locating an exception in a contract, and translating that into a checklist. This is a fictional illustrative workplace scene, not a photograph of a named company.
Scene: bright real-feeling daylight at a modest shared worktable, viewed from a slightly elevated three-quarter angle. Two adult Korean colleagues, one experienced domain specialist in their fifties and one technical colleague in their thirties, are concentrating on the documents rather than looking at the camera. The specialist points with a pencil at one circled line in a quotation; the colleague is writing a short checklist on a pad beside an open laptop. On the table are exactly two quotation sheets side by side, one with a green check mark, one with a red circle and correction mark, plus a thin open contract with one highlighted clause. Show the meaningful document interaction and natural hands clearly. The laptop can show a simple checklist layout, no actual product logo or identifiable customer data.
Style: photorealistic candid business editorial photography, natural skin and fabric texture, ordinary office supplies, soft daylight, balanced warm neutral colors, 35mm perspective, realistic depth of field with documents and working hands sufficiently sharp. The activity, not generic office mood, should dominate.
Constraints: no handshakes, no posing, no smiling at camera, no floating icons, no holograms or robots, no ornamental arrows or infographic panels, no watermarks, no brand names, no fabricated readable financial figures or customer names. Represent document contents using realistic small lines and table structure without prominent invented words.
```

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-aa9779a6-548a-4650-a5eb-d662e27ebf01.png`

### stale-policy

```text
Use case: illustration-story.
Asset type: conceptual in-article illustration explaining failure from stale Agent Skill instructions; landscape approximately 16:9 2048x1152.
Primary request: Explain visually that an agent can diligently follow an old policy and generate repeated wrong quotation drafts even though a newer policy already exists. The problem is stale work guidance, not a broken or malicious model.
Scene: one coherent editorial desk scene with a generic agent desktop interface acting as a document workstation. An old open paper instruction folder in muted coral, clearly labeled exactly "v1", is visibly connected to the agent workstation by a single paper ribbon. From the workstation emerges a short orderly fan of three quotation draft sheets, each showing the SAME clearly visible red-circled mistaken table cell. Nearby, a fresh updated policy folder in teal, labeled exactly "v2", sits on a small raised shelf, conspicuously outside that paper connection. A human reviewer is reaching in with a pencil and noticing the repeated circled mistake. Make the contrast between available v2 and still-used v1 instantly understandable. Do not put a connection between v2 and the workstation. Do not imply every old version is always wrong; this is one hypothetical example of changed policy.
Style: sophisticated hand-painted gouache and cut-paper business editorial illustration on a warm ivory background, bold readable silhouettes, subtle grain, restrained ink/teal/coral colors. A little narrative wit from the perfectly organized wrong drafts, no slapstick. Close composition focused on the relationship of old instruction, ignored update and repeated mistake, with enough space between them.
Text: only "v1" and "v2", large and exact on the folder tabs. No other lettering, captions, numbers, logos, watermark, robot faces, or decorative background objects. Tables represented with line marks. No infographic frames or long explanatory labels.
```

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-6cd8635d-d47b-4bee-841a-0e1d71e6e8b9.png`


## 도해 제작 기준

- 공통: 폭 1200px, 높이 680/760/780px, 밝은 아이보리 바탕과 틸·코발트·코럴 강조, 본문 글씨 24px 이상과 보조 22px. SVG 내부 title·desc와 Markdown 대체 텍스트 제공.
- figure-skill-loading.svg: 모든 스킬의 본문과 모든 자료를 매번 읽는 것으로 표현하지 않는다. 이름·설명 목록에서 선택된 견적 스킬을 강조하고 세 자료 분기는 점선으로 표현한다.
- figure-quote-workflow.svg: 지침 파일이 최신 데이터·연결·인증을 자동 제공한다고 표현하지 않는다. Skill은 업무 방법, Tool은 조회, 검사 코드·양식은 검증·출력 구성으로 역할을 나눈다. 확인이 끝나도 가격 확정·발송은 별도 승인·권한 절차다.
- figure-approval-boundary.svg: 위쪽은 승인 상태를 검사하지 않는 도구라는 조건을 명시한 가상 위험 구성이다. 아래쪽은 실행 전 승인 상태 및 승인된 금액·수량·버전을 확인한다. 자연어가 시스템 차단을 보장한다고 표현하지 않는다.

## 파일·검수

- 생성 원본은 기본 생성 디렉터리에 보존했다. 웹용 선택본은 포스트 디렉터리에 저장했다.
- 래스터 3종은 원본 크기 1672×941를 유지하고 JPEG 또는 WebP 품질 88로 변환했다. 의미를 바꾸는 합성·수정은 하지 않았다.
- 썸네일의 AGENT SKILLS·SKILL.md 표기, 실사풍 이미지의 문서 비교 장면과 손, v1·v2 연결 관계와 반복 오류를 시각 확인했다.
- SVG 3종을 rsvg-convert로 PNG 렌더링해 한글, 텍스트 잘림과 화살표·분기를 확인했다. 검수용 PNG는 `_workspace/2026-09-08-agent-skills-images/`에 보관했다.
- 도해는 눌러 원본 크기로 볼 수 있도록 본문에 링크를 걸었다.
- Hugo 초안 포함 빌드 성공. 이미지 6개가 출력 디렉터리에 복사되고 원본과 바이트가 같은지 확인했다. OG 이미지가 `/posts/what-are-agent-skills/thumbnail.jpg`를 가리키는 것도 확인했다.
- 최종 이미지 파일 합계 1,109,138바이트(약 1.06MiB). 생성 원본 PNG 대신 웹용 JPEG·WebP와 SVG를 게시 자산으로 사용한다.
- 본문 대조 결과 이미지·캡션 외의 원고는 동일하며 CTA·출처·초안 상태를 보존했다. 기존 다른 포스트의 raw HTML 경고는 이번 작업과 무관하므로 수정하지 않았다.
- 이미지 제작 단계에서는 커밋·푸시·공개 전환을 하지 않았다.

## 발행 준비 (2026-09-08)

- 후속 커밋·푸시 요청에 따라 포스트를 `draft = false`로 전환했다.
- 초안 포함 옵션 없이 실행한 Hugo 프로덕션 빌드에서 게시 페이지, 이미지 6개, OG 썸네일, 홈 목록·사이트맵과 메일 CTA를 확인했다.
- 게시 전 검토에서 그림 1 캡션의 대상을 '스킬 목록'에서 '모든 스킬의 본문'으로 명확히 했다. 이름·설명 목록은 먼저 살펴본다는 본문·도해와 맞췄다.
- 포스트와 관련 리서치만 커밋 대상으로 삼고 `_workspace`·`.DS_Store`·이전 포스트의 이미지 변경은 제외했다.
