# AI 승인 워크플로 포스트 이미지 생성 기록

- 대상: `content/posts/geoff-12-ai-approval-workflow/index.md`
- 생성 방식: 내장 imagegen 도구. 최종 WebP는 파일 자체 폭 800px 이하로 변환.
- 배치: H2 섹션 8개에 이미지 8장. 썸네일은 들어가며에도 사용.
- 그림 설명은 alt에만 기록하며 본문 캡션은 추가하지 않는다.
- 장면은 가상·개념 일러스트이며 실제 회사 화면이나 현장을 재현하지 않는다.

## 최종 보정·내보내기

- 실행 검사 도해만 1회 국소 수정: 투명 배경을 밝은 불투명 배경으로 바꾸고 본문에 없는 거래 금액을 제거했다. 흐름과 상태 표시는 유지했다.
- 생성 원본을 보존하고 `cwebp -q 90 -m 6 -resize 800 0`으로 최종 WebP를 내보냈다. CSS나 테마 코드는 바꾸지 않았다.
- 최종 8장 모두 실제 크기 800×451px. 이미지와 썸네일 frontmatter 외에 본문 문장은 변경하지 않았다.

### 실행 검사 도해 국소 수정 프롬프트

```text
Change only the transparent/black background to solid opaque warm ivory #FAF7EF and remove the arbitrary ledger amounts -50,000, -30,000, -20,000, replacing them with neutral gray bars. Remove cutout fringes. Preserve all Korean labels, objects, branch arrows and aspect ratio. Pending and denied branches must not reach execution. Do not add any text or numbers.
```

## thumbnail.webp

- 섹션: 들어가며
- 유형: editorial illustration
- Alt: AI가 12만 원 환불을 완료했다고 알리지만 고객지원 팀장은 승인한 적이 없어 당황하는 가상의 업무 장면

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: illustration-story.
Create an editorial thumbnail that immediately conveys unauthorized AI execution, not a generic office mood. Single visually unified scene: an adult customer-support team leader in a navy cardigan looks surprised and troubled at a refund notification, with one hand naturally at the desk and the other holding a pen lowered in disbelief. Nearby a simple abstract AI application motif (small teal sparkle/application icon, NOT a humanoid robot) accompanies a large clean notification inset "12만 원 환불 완료". The manager's reaction is conveyed in a single clearly attached short speech balloon "저는 승인한 적 없는데요?"
A small ledger-like approval card next to the notification reads "팀장 승인 없음" in coral. The refund notification is completed; there must be NO approved green signature or approval stamp on the manager's card. Let the juxtaposition of completed action and missing human authorization be the main image. Sparse bright office setting, not walls of data. No extra title text. Keep the reaction and 12만 원 readable even as a thumbnail. Illustration, clearly hypothetical, no real brand logos.
```

## figure-identity-permission-approval.webp

- 섹션: 일을 잘한다고 전결권까지 주지는 않습니다
- 유형: concept comparison
- Alt: 인증은 신원 확인, 권한은 담당 주문 조회 범위, 승인은 이번 12만 원 환불의 결정을 뜻하는 개념 비교

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: infographic-diagram.
A minimal illustrated comparison of THREE distinct concepts, not a timeline. Three equal open columns with generous gaps and NO connecting arrows. Each column has one memorable big object illustration, one big heading and one short line.
Column 1: badge with a generic human portrait and verification tick, heading "인증", line "누구인가?"
Column 2: a key next to a bounded folder of order cards, with only one assigned folder accessible, heading "권한", line "무엇을 할 수 있나?"
Column 3: a specific refund request card showing the large amount "12만 원", a human approver's signed approval mark, heading "승인", line "이번 건을 허용했나?"
Below the objects within each column, only if needed use these exact short examples: "사원증 확인", "담당 주문 조회", "환불 한 건 결재". The three headings and questions dominate, no long description. Do not imply authentication automatically gives permission or approval. All columns are separate explanations, balanced visual weight.
```

## illustration-advisor-email-review.webp

- 섹션: 실제 회사들은 어디서 사람을 부를까?
- 유형: scenario illustration
- Alt: 담당자가 AI가 작성한 고객 메일 초안을 읽고 수신자와 첨부파일을 확인하는 가상의 자산관리 업무 장면

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: illustration-story.
A mature editorial illustration of a financial advisor personally reviewing an AI-generated client email BEFORE sending. Clearly hypothetical office, no actual company branding. An adult advisor in a simple jacket sits at desk, viewed from a plausible over-the-shoulder three-quarter angle so the monitor faces the advisor and is visible to viewer from same side. One hand naturally rests on mouse and other on desk next to an open folder with pages oriented toward advisor. Monitor shows a clean email composition window with generous abstract gray text lines; visible short labels "초안", "수신자", "첨부파일", and a muted inactive-looking "보내기" button. No 'sent', no outbound envelope in flight, no completed-send checkmark. Advisor attentively compares the recipient field and attached document before acting; a subtle desk note with a document icon conveys actual supporting material. Warm daylight, simplified but sophisticated illustration, relatable professional attention rather than broad generic smile. No separate caption, no giant headline or process arrows.
```

## figure-cumulative-refund.webp

- 섹션: 금액만으로 승인 대상을 정하면 빠지는 일이 있습니다
- 유형: numeric explanatory diagram
- Alt: 같은 주문에서 처리한 6만 원과 추가 환불 요청 6만 원의 누적액이 12만 원이 되어 팀장 승인이 필요한 가상 예시

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: infographic-diagram.
Draw a visually precise refund cumulative-limit example, landscape and very legible. Small top label "같은 주문의 환불". Two illustrated receipt cards on the left/middle joined by a plus sign, leading to a cumulative amount card on right.
First receipt: heading "처리 완료", amount "6만 원", teal completed tick.
Second receipt: heading "추가 요청", amount "6만 원", coral small clock icon and label "승인 대기". This second payment has NOT executed. Do not mark it completed.
Result: heading "처리하면 누적", amount "12만 원". Beneath result a clear coral callout "팀장 승인 필요".
A discreet but readable bottom rule line: "예시 규정: 10만 원 초과 시 승인".
Do not show two completed payments followed by late approval. Show the proposed cumulative total if the pending request were executed. No percentages, no charts, no additional numbers.
```

## figure-execution-approval-gate.webp

- 섹션: 승인 버튼 뒤에는 실행을 막는 코드가 있어야 합니다
- 유형: execution flow diagram
- Alt: 승인이 필요한 환불 요청을 권한·조건·승인 검사에 통과시킨 뒤 실행하고 승인 대기는 보류하며 거절된 요청은 중단하는 구조

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: infographic-diagram.
Create a clear technical concept diagram titled "승인이 필요한 환불". Three main large illustrated stages from left to right:
1 a proposed-action document labeled "AI의 실행 요청";
2 a central guarded gateway/server gate labeled "권한·조건·승인 확인";
3 a business-system ledger labeled "환불 실행".
Only one right-pointing arrow from gate to execution, labeled "검사 통과". It is not enough to simply receive approval; all checks pass.
Above the central gate show a small human reviewer icon with approval record card labeled "담당자 승인 기록", connected DOWN to the gate, NOT directly to execution.
Below the central gate TWO distinct small status branches: amber clock labeled "승인 대기: 보류"; coral stop icon labeled "거절: 중단". Neither branch reaches execution. Make branch lines unambiguous and non-crossing. No background server rooms, no invented company logos, no bypass arrow, no loops, no decorative tiny text. Important labels are large and schematic readable at 800px.
```

## figure-approved-versus-changed-refund.webp

- 섹션: 12만 원을 승인했는데 15만 원이 나가면 안 되겠죠
- 유형: transaction integrity comparison
- Alt: R-204 주문의 12만 원 환불 승인과 금액을 15만 원으로 변경해 재승인이 필요한 요청을 비교한 가상 예시

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: infographic-diagram.
Two big transaction cards side by side connected by one horizontal change arrow. Big heading at top "승인한 내용이 바뀌었다면?"
LEFT card with teal accent: "주문 R-204", large "12만 원", a greenish approval stamp "승인 완료".
Arrow between the cards labeled briefly "금액 변경".
RIGHT card with coral accent: exact same "주문 R-204", large "15만 원", a coral closed-padlock icon and status "재승인 필요". This card is NOT approved and has NOT executed. No outgoing money or success mark.
Bottom concise rule "이전 승인으로 실행 불가".
Keep original approved12 vs changed15 visually distinct. Do not show that all12만원 approved payments auto-execute. No additional dates, refund IDs, tiny footnotes, fake signatures or per-person names. Minimal vector-like editorial shapes with very subtle grain.
```

## illustration-focused-approval-review.webp

- 섹션: 결재선이 생겼는데 팀장은 더 바빠졌습니다
- 유형: scenario illustration
- Alt: 일상 요청은 자동 처리하고 예외 건의 문의·반품 상태·금액을 모아 검토하는 담당자의 가상 업무 장면

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: illustration-story.
Create a coherent editorial scene about protecting a human reviewer's attention by routing routine cases automatically and bringing them only well-prepared exceptions. Adult team leader at desk carefully reviewing ONE exception with an attentive calm expression, NOT overwhelmed by dozens of dialogs. View from three-quarter rear so monitor is correctly oriented toward reviewer, with natural hands resting on keyboard and a supporting folder (no reverse-oriented writing).
In the left side of composition a clearly stylized digital tray of small routine-order cards with teal ticks is labeled "일상 요청: 자동 처리". These cards flow to a closed processed tray, not toward the person.
Near the reviewer, one large highlighted coral-bordered request card labeled "예외 건 검토". It contains exactly three large compact visible fields: "고객 문의", "반품 상태", "요청 금액". The fields have small abstract illustration icons rather than tiny unreadable prose. The reviewer sees the same card on the monitor; detach the large card as a clear explanatory inset rather than an impossible physical screen floating in their face. No numeric savings, no brand UI, no explicit approval yet. The important story is focused review with evidence, not a generic office portrait. Warm bright palette and mature hand-drawn editorial finish.
```

## illustration-team-approval-rules.webp

- 섹션: 나가며
- 유형: scenario illustration
- Alt: 현업 담당자와 엔지니어가 승인·반려 사례를 함께 검토하며 자동 처리·승인 필요·금지 조건을 정하는 가상 협업 장면

```text
Asset type: explanatory image for a Korean enterprise AI tech blog read by executives. Landscape 16:9, aim for 1600x900. Final image will be resized to 800px wide, so all important visible text must be very large, concise, and readable at that width. Use exact Korean text supplied, do not add extra labels, watermarks, slogans, logos, page numbers or captions. Cohesive professional editorial style: warm ivory background, deep navy typography and outlines, muted teal for allowed or verified states, coral for attention or blocked states, a little ochre emphasis. Restrained flat color shapes with subtle tactile editorial texture, clean composition and generous whitespace. Not a dark futuristic control room, not neon, not a corporate stock handshake, not a comic page, not chibi. Human figures if used should have plausible adult proportions, natural shoulder/elbow/wrist connections, two arms each, coherent fingers and gaze; readable document or monitor content must face the person using it, or be in a clearly detached explanatory inset.
Use case: illustration-story.
A meaningful bright editorial illustration of a domain operations lead and software engineer standing SIDE BY SIDE facing the same whiteboard, collaborating to translate actual exception cases into operational rules. The viewer sees them three-quarter from behind, with their faces slightly in profile so gaze and board orientation are coherent. One person holds a thin folder of case documents at their side; the other points naturally with one hand at a relevant board card. No tangled arms, no handshake, no writing notebooks toward the viewer.
On the board exactly THREE clear large columns labeled "자동 처리", "승인 필요", "금지". Under the columns simple icon cards: routine valid order/teal tick; exceptional request/human approval clock; disallowed change/coral stop. A small group of source case cards at bottom-left of board is labeled "승인·반려 사례", and two unobtrusive connectors lead from these cases into the human-curated columns. Make both people visibly engaged with the specific rule cards, not an AI robot inventing its own policy. No invented brand logo, no corporate slogan, no other text or statistics. The image communicates people turning operational judgment into reusable rules and working with an engineer, not generic team building.
```
