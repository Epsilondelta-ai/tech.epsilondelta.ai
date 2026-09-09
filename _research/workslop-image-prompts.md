# Workslop 포스트 이미지 제작 기록

- 제작일: 2026-09-09
- 대상: `content/posts/geoff-9-workslop/index.md`
- 범위: 썸네일 메타데이터, 섹션별 이미지, 대체 텍스트와 그림 설명 추가. 기존 본문·표·출처 링크는 유지.
- H2·H3 13개 섹션에 각각 이미지 1장, 총 13장.
- 구성: 썸네일 1장, 실사풍 2장, 일러스트 5장, SVG 도해 5장.
- 생성 방식: 내장 이미지 생성 도구로 래스터 이미지 8장 생성. 정확한 한글·수치·연결 관계가 필요한 도해 5장은 SVG로 제작.
- 게시 상태: `draft = true` 유지. 이번 이미지 작업에서는 커밋·푸시하지 않음.
- 본문 보존 확인용 스냅샷: `_workspace/2026-09-09-workslop-images/index-before-images.md`

## 섹션별 배치와 설명 목적

아래 파일은 모두 포스트와 같은 디렉토리에 저장했습니다. 사진처럼 보이는 두 장은 실제 사건·기업의 촬영 사진이 아니라 AI로 생성한 가상 업무 장면이며, 본문 캡션에도 이를 표시했습니다.

| 섹션 | 파일 | 설명 목적 |
|---|---|---|
| 들어가며 | [thumbnail.jpg](../content/posts/geoff-9-workslop/thumbnail.jpg) | 작성 속도 향상 뒤에 남은 수신자의 확인·수정 업무 |
| 그럴듯한 결과물에 동료의 할 일이 들어 있습니다 | [illustration-unfinished-package.webp](../content/posts/geoff-9-workslop/illustration-unfinished-package.webp) | 바로 쓸 줄 알았지만 조립부터 해야 하는 결과물의 비유 |
| 실제 업무에서는 누가 뒤처리를 했을까? | [figure-rework-spread.svg](../content/posts/geoff-9-workslop/figure-rework-spread.svg) | 두 실제 사례에서 추가 업무가 넘어간 사람과 기관 |
| 검토 보고서를 다시 검토한 호주 정부 | [photo-report-audit.webp](../content/posts/geoff-9-workslop/photo-report-audit.webp) | 인용과 원자료를 대조하며 다시 검토하는 업무 |
| 동료 변호사가 넘긴 판례를 법원이 다시 찾았습니다 | [illustration-legal-recheck.webp](../content/posts/geoff-9-workslop/illustration-legal-recheck.webp) | 서면에 기재된 판례를 찾기 위한 추가 조사 |
| 왜 AI를 쓰면서 이런 일이 생길까요? | [figure-missing-context.svg](../content/posts/geoff-9-workslop/figure-missing-context.svg) | 업무 목적·현업 기준의 누락과 재작업, 측정에서 빠지는 시간 |
| 회사의 시간은 어디에서 계산해야 할까? | [figure-team-time.svg](../content/posts/geoff-9-workslop/figure-team-time.svg) | 작성자와 팀 전체 투입시간의 차이 |
| 해결은 받는 사람의 업무에서 시작합니다 | [photo-cross-team-review.webp](../content/posts/geoff-9-workslop/photo-cross-team-review.webp) | 작성자와 수신자가 목적과 필수 정보를 맞추는 협업 |
| 넘겨도 되는 기준을 함께 정합니다 | [figure-handoff.svg](../content/posts/geoff-9-workslop/figure-handoff.svg) | 업무 기준 합의부터 근거·검사·보완·인계까지의 흐름 |
| 확인할 근거를 결과물 옆에 둡니다 | [illustration-source-trace.webp](../content/posts/geoff-9-workslop/illustration-source-trace.webp) | 주장과 숫자를 원자료의 해당 위치와 대조하는 방법 |
| 검토를 맡길 사람에게 자료와 시간도 줍니다 | [illustration-review-capacity.webp](../content/posts/geoff-9-workslop/illustration-review-capacity.webp) | 검토에 필요한 자료와 일정 확보 |
| 바빠졌다고 모두 Workslop은 아닙니다 | [figure-two-kinds-of-work.svg](../content/posts/geoff-9-workslop/figure-two-kinds-of-work.svg) | 가짜 문제의 확인과 진짜 문제의 해결에 드는 업무 구분 |
| 나가며 | [illustration-reusable-knowledge.webp](../content/posts/geoff-9-workslop/illustration-reusable-knowledge.webp) | 현업의 교정을 공용 지침으로 남겨 다음 업무에서 활용 |

## 웹용 저장

- 래스터 이미지 8장: 각각 1672 × 941px.
- 썸네일: JPEG, 품질 85.
- 본문 래스터 이미지: WebP, 품질 86.
- SVG: 글자를 확대해 읽을 수 있도록 본문에서 원본 파일도 연결.
- 생성 원본 PNG는 아래 로컬 경로에 보존. 포스트에서는 웹용 파일만 사용.
- 썸네일은 `featured_image`와 `images` 양쪽에 지정.

## 도해의 의미와 검수 기준

- `figure-rework-spread.svg`: 호주 보고서 사례의 재확인·정정·재공개와 법률 서면 사례의 추가 판례 조사를 구분. AI 사용 주체와 업무 수행 주체를 혼동하지 않도록 표시.
- `figure-missing-context.svg`: 업무 목적과 현업 기준이 빠지는 문제를 설명. 작성 시간만 측정하는 관행은 재작업 비용을 성과표에서 놓치는 문제로 연결.
- `figure-team-time.svg`: 본문의 가상 계산만 사용. 기존 방식 60 + 20 + 10 = 90분, AI 활용 후 15 + 45 + 35 = 95분. 두 막대에 같은 영점과 척도를 사용. 사람별 투입시간 합계이며 실측 성과나 경과시간이 아님을 표시.
- `figure-handoff.svg`: 기준 합의 → 초안·근거·미확인 항목 준비 → 업무에 맞는 검사와 검토 → 인계. 미흡한 경우 보완 단계로 돌아감. 승인이 필요한 업무의 실행 권한도 확인.
- `figure-two-kinds-of-work.svg`: 가짜 문제를 확인·반박하는 재작업과 진짜 문제를 우선순위에 따라 수정하는 후속 작업을 구분.
- SVG에는 `title`·`desc`를 제공. 모든 이미지에 내용에 맞는 대체 텍스트와 그림 설명을 작성.

## 래스터 이미지 생성 프롬프트

아래는 내장 생성 도구에 실제 전달한 프롬프트입니다. 법률 삽화는 아래 별도 수정 프롬프트까지 적용한 최종본을 사용합니다.

### 1. thumbnail.jpg

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-bb01b567-d980-4212-b2d5-1b5519087c5b.png`

```text
Use case: illustration-story. Asset: landscape editorial cover for a Korean executive-facing article about WORKSLOP, 16:9, approximately 2048x1152. Show the article's central idea: an AI-made report looks finished quickly, but the receiving colleague must reopen source material, verify and rework it. One coherent bright worktable scene: at the left a business author at a generic laptop with a small label "AI" hands over a neatly typeset report with a chart; at the right the receiving colleague has opened that same report beside source spreadsheets and reference pages, comparing a highlighted figure and making corrections with a pencil. The clean handoff document leads into a visibly larger spread of checking work on the receiving side. The author is working normally, not lazy or celebrating; do not portray blame or incompetence. Make this transfer of unfinished work visually clear even at thumbnail size. Premium business-magazine gouache and cut-paper illustration, warm ivory background, precise ink shapes, restrained teal/blue and coral marks, gentle paper grain. Large clearly legible title "WORKSLOP" at top; only other readable text is "AI". Keep title and main action within a safe central crop. No unrelated office mood, dark neon, robots, brains, holograms, logos, fake statistics, dense infographic boxes, or watermark.
```

### 2. illustration-unfinished-package.webp

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-5efabfb1-9f0e-4a06-ab7e-db14a448d7b8.png`

```text
Use case: illustration-story. Asset: landscape 16:9 in-article illustration of the author's explicit analogy, not a real product. Explain: the recipient expected a finished item but discovers assembly work still to do. A person opens a plain delivery box on a bright table. On the box is a simple picture of a fully assembled wooden desktop document organizer. In front are its still-disassembled wooden side panels, shelves and a small bag of screws; the recipient holds two panels and studies how they fit. Show the finished-organizer picture and the unassembled parts clearly together so the expectation mismatch is obvious. No complex machinery or unsafe electrical assembly. Sophisticated ink and gouache editorial illustration, warm paper surface, restrained blue/teal and natural wood colors. Moderate close-up focused on hands, box and parts; calm mildly puzzled gesture, not slapstick. No chart or diagram panels, no arrows, no text or letters, no logos or watermark. This illustrates hidden remaining work after apparent completion; do not imply all legitimate flat-pack products are bad.
```

### 3. photo-report-audit.webp

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-be5011b3-971d-4d6e-851c-0d98ad67d5b8.png`

```text
Use case: photorealistic-natural. Asset: landscape 16:9 supporting image for the paragraph about additional source checking after a report is delivered. Fictional work scene, NOT actual Deloitte, government staff, or evidence of the historical event. Tight overhead three-quarter editorial photograph of two adult colleagues' hands comparing a professionally formatted printed report with reference materials on a laptop and a separate source-check sheet. One hand points at a highlighted footnote on the report, another marks a correction in pencil on the matching check sheet. A few source entries have small question marks, one has a check; an open reference book and a revised page with visible margin edits demonstrate verification and correction. Contents are generic linework and small plausible print, no readable personal names, official seals, company names, financial figures or real quotes. Bright window daylight, natural paper and desk texture, credible hands, understated realism. Focus on the actual cross-checking activity rather than a generic busy desk. No posed handshakes, robot, holograms, dramatic dark lighting, infographic overlays or watermark.
```

### 4. illustration-legal-recheck.webp

1차 수정 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-6549dc56-7088-4067-91c0-d40756f9fbff.png`. 이후 주황색 연결선을 제거한 최종 원본은 아래 사용자 검토 후 수정 기록에 명시했습니다.

```text
Use case: illustration-story. Asset: landscape 16:9 conceptual illustration explaining a legal citation that the receiving lawyer cannot locate. Fictional characters and materials, not a reenactment of named people or a real courtroom. An adult legal professional at a desk compares a submitted legal brief with an open case-law reference volume and a laptop search page. One citation in the brief is highlighted amber and connected by the person's gaze and pointing pencil to the search page showing exactly "NO MATCH"; the professional is writing a follow-up query on a small notepad. Another stack of unrelated pending files remains closed, suggesting extra investigation displaced scheduled work. Make the specific citation lookup, not legal symbolism, the focus. Refined editorial ink and gouache with paper grain, warm ivory, navy, muted teal and amber. No judge costume, gavel, scales of justice, courtroom grandeur, real company logos, recognizable people, fabricated readable cases or quotations. Only readable text "NO MATCH"; other text abstract fine lines. No diagram frames or watermark.
```

### 5. photo-cross-team-review.webp

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-64e73118-392e-4a46-9a6e-332f1e897228.png`

```text
Use case: photorealistic-natural. Asset: landscape 16:9 in-article photo-style image introducing solutions to workslop. Show the author of a business report and its recipient agreeing what the report must help them decide. Two adult Korean colleagues from different business functions meet at a small daylight table: a strategy analyst and a sales lead examine the same printed customer-analysis report. The recipient points to a highlighted row on a short required-information checklist, while the author adds a note next to the corresponding report section. A laptop holds the underlying source spreadsheet; both are engaged with the materials and each other, not posing. This is a fictional illustrative scene, not real customer evidence. Natural skin and fabric texture, candid medium-wide framing, quiet modern office with minimal background, document interaction clearly visible. No named companies, readable confidential data, random financial numbers, artificial charts overlaid on photo, smiling at camera, handshakes, robots or watermark. Keep the image about agreeing requirements and use, not merely holding a meeting.
```

### 6. illustration-source-trace.webp

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-4e9685a6-cc72-4fca-a4f5-9f0f7f377274.png`

```text
Use case: illustration-story. Asset: landscape 16:9 supporting illustration for placing evidence beside the result. Close editorial still-life of a report and the source pages laid side by side, reviewed by a person's hand with a pencil. The report has one highlighted numeric/table entry; the source page has its corresponding table row highlighted in the same amber color, with a page tab and a clearly visible source date field rendered as short line marks. A small note shows a question mark for an unresolved claim. Let the viewer trace the report claim to the specific source row visually through the shared highlighting and the reviewer's pointing gesture. This is a fictional conceptual example; do not invent actual data values, names or citations. Premium textured gouache and paper collage, warm ivory and restrained teal/ink/amber. Simple tangible papers rather than floating tech dashboards. No long text, no numbers, no labels, no decorative magnifying glass, logos, brains, robots, dense arrows or watermark. Show that evidence is available for checking, not that one matching highlight guarantees the whole report is correct.
```

### 7. illustration-review-capacity.webp

선택한 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-435a706c-cc32-4f5e-acfa-2879de3fce5a.png`

```text
Use case: illustration-story. Asset: landscape 16:9 image for allocating time and source material to a reviewer. A human reviewer at a practical worktable has a report, its open source binder and a compact checklist ready for a focused review. Beside them is a clearly visible paper weekly planner with a substantial reserved block labelled exactly "REVIEW". A small organized queue of three other report folders waits in an incoming tray outside the active workspace. The person is using the checklist and source binder, rather than blindly approving a document. Make the allocated review block and the supplied evidence distinguishable, so the image communicates that assigning a reviewer also requires time and material. Editorial magazine gouache illustration, natural adult proportions, warm ivory, teal and ink with a small coral accent, tactile paper grain. No generic overworked employee cliche, no giant clocks, chaotic paper avalanche, red alarms, robots, company logos or watermark. Only readable word "REVIEW"; calendar otherwise abstract lines without dates or numbers. Not a claim about a specific company.
```

### 8. illustration-reusable-knowledge.webp

최초 생성 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-657d33e3-8161-4772-8ec2-3306670154eb.png`. 이후 팔 자세를 수정한 최종 원본은 아래 사용자 검토 후 수정 기록에 명시했습니다.

```text
Use case: illustration-story. Asset: landscape 16:9 closing illustration for a corporate AI article, connecting real feedback to reusable organizational know-how. Show one experienced colleague reviewing an annotated report and carefully adding a verified correction as a short checklist page to a shared tabbed work binder. A second colleague uses that same binder beside a new report on a laptop, checking a matching item before passing the report onward. One shared table, collaborative focused gestures, clear relation between corrected report, maintained shared guidance and the next person's work. The improvement is reviewed and maintained by people; do not imply automatic permanent model learning. Premium hand-drawn ink and gouache, warm ivory paper texture, muted navy and teal with restrained amber highlights, bright practical atmosphere. The binder tab reads exactly "TEAM GUIDE"; all other writing is unobtrusive line marks. No victory pose, handshake, glowing brain, neural nets, anonymous cityscape, charts promising gains, company logos or watermark. This should show a concrete reusable work practice, not abstract teamwork mood.
```

## 법률 삽화 국소 수정

최초 생성본에 요청하지 않은 읽을 수 있는 가상 판례명이 들어가 있어 제거했습니다. 실제 판례처럼 오인할 수 있는 사례명을 넣지 않고, 검색에 실패하는 개념을 유지했습니다.

- 미사용 최초 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-f39fcff0-cd69-4e27-858f-0b1ff665dd93.png`
- 포스트에는 수정 후 선택한 원본에서 변환한 `illustration-legal-recheck.webp`만 사용.

```text
Use case: precise-object-edit. Edit this exact editorial legal-research illustration. Keep the person, hands, desk, open book, papers, laptop, composition, lighting and painting style unchanged. The highlighted citation and laptop search field currently contain an invented case name and numeric citation; remove ALL readable words and numbers from both of those fields and replace them with neutral short horizontal line marks. They must still be highlighted/matching and clearly being compared. Retain the exact large laptop result text "NO MATCH". Remove ALL other readable lettering from the decorative posters, notebook, folder label and book spines, replacing it with blank paper or unobtrusive abstract lines. In particular there must be no "Rivers v. Dalton", no invented legal citation, no numeric year and no motivational slogan. Do not add new text, objects, arrows or labels. The only readable words in the finished image should be "NO MATCH". The image is a generic conceptual illustration, not evidence or a reconstruction of any named legal case.
```

## 시각 검수

래스터 이미지 8장과 SVG 렌더링 5장을 확인했습니다. 법률 삽화의 가상 판례명 제거를 확인했고, 도해의 연결 방향·한글·수치·본문과의 의미 일치를 점검했습니다. 이후 사용자 검토에서 나가며 삽화의 팔 위치와 법률 삽화의 주황색 연결선 문제가 추가로 확인되어 별도 수정했습니다. SVG 렌더링 확인용 PNG는 `_workspace/2026-09-09-workslop-images/`에 저장했습니다.

## 빌드와 본문 보존 확인

- Hugo 초안 포함 빌드 성공. 기존 다른 포스트의 raw HTML 경고 1건은 이번 작업에서 변경하지 않음.
- 기존 본문·표·출처 17개 보존 확인. 이미지·캡션과 썸네일 메타데이터를 제외하면 변경 전 스냅샷과 동일.
- H2·H3 13개 각각 이미지 1장, 캡션 13개 확인.
- 렌더링된 표 4개와 연락처 CTA 보존.
- 본문 이미지 파일 13개와 공유용 OG 썸네일 경로 확인.
- SVG 5개 XML 검증 통과. 스크립트나 외부 리소스 의존성 없음.

## 사용자 검토 후 이미지 수정

두 이미지 모두 내장 이미지 생성 도구의 편집으로 수정한 뒤 원래 WebP 경로에 반영했습니다. 변경 전 PNG는 생성 원본 디렉토리에 보존했습니다. 본문과 캡션은 변경하지 않았습니다.

### 나가며 삽화의 팔·손 자세 수정

- 최종 파일: `content/posts/geoff-9-workslop/illustration-reusable-knowledge.webp`
- 팔 자세 수정 당시 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-b37b4ac1-a745-42eb-a726-5d1a0d65b8fb.png`. 현재 최종 원본은 아래 왼손 수정본 기록 참조.

```text
Use case: precise-object-edit.
Input image: edit target, the existing wide watercolor illustration of two colleagues updating a TEAM GUIDE.
Change only the anatomically confused arms and the document support needed to make their poses natural. Keep the same two faces, clothes, warm watercolor style, room, palette, TEAM GUIDE binder, laptop, desk and overall wide composition.
The woman must have exactly two clearly connected arms and two hands with a natural shoulder-to-elbow-to-wrist path. Simplify her pose: place the corrected loose report FLAT on the desk to the LEFT of the open binder, rather than floating upright in front of her chest. Her anatomical right arm (viewer-left side) descends naturally from her shoulder, with its hand resting on that flat report. Her anatomical left arm (viewer-right side, near the binder) bends naturally forward from her visible shoulder, its elbow beside her torso and its forearm extending a short distance to a hand holding a pen over the LEFT page of the binder. No crossed arms, no sleeve entering from outside the frame, no detached hand or arm, no third limb, no extremely long forearm. Both of her shoulders, sleeve paths and elbows must be understandable.
The man has exactly two connected arms: his right forearm naturally extends toward the guide and one finger indicates the RIGHT page; his left hand rests next to the laptop. Keep his body and arms separate from hers. All four hands belong visibly to their owners.
Preserve the meaning: a senior colleague turns reviewed corrections into a shared guide while another colleague uses the guide for subsequent work. No new arrows, lines, slogans or extra objects. Keep the 16:9 aspect ratio.
```

### 법률 삽화의 주황색 연결선 제거

- 최종 파일: `content/posts/geoff-9-workslop/illustration-legal-recheck.webp`
- 최종 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-284455a0-bb2b-48ed-ba88-b203b9dce158.png`

```text
Use case: precise-object-edit.
Input image: edit target, the existing wide watercolor legal-research illustration with NO MATCH on the laptop.
Remove ONLY the thin orange diagonal connector line and its arrowhead floating from the highlighted paragraph on the left document, across the woman's torso, toward her pencil hand. It is an unwanted infographic overlay, not a physical object. Restore the underlying paper edge, clothing and background cleanly. There must be no floating orange line, arrow or connector anywhere between the paper and her hand.
Keep the real short pencil she holds, the yellow highlight ON the paper, and the yellow highlight INSIDE the laptop search field. Preserve her face, clothing, hands, pose, the entire office setting, books and folders, watercolor texture, palette, framing, 16:9 aspect ratio and all other details. Keep the exact text NO MATCH on the screen. Do not add any case names, new readable text, symbols or lines. This is a localized removal, not a redesign.
```

여성 인물의 종이를 책상 위에 놓고 두 팔의 어깨·팔꿈치·손 연결이 드러나도록 자세를 단순화했습니다. 남성 인물의 손은 안내서를 가리키는 손과 노트북 옆에 둔 손으로 분리했습니다. 법률 삽화는 종이에서 인물의 몸 앞으로 지나던 주황색 연결선을 제거하고 실제 연필과 문서·검색창의 강조 표시를 유지했습니다.


### 펜을 쥔 왼손 수정본 교체 이력

- 최종 파일: `content/posts/geoff-9-workslop/illustration-reusable-knowledge.webp`
- 왼손 수정 당시 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-f514c995-2b33-4c56-bb52-ca65395f8760.png`. 현재 최종 원본은 아래 노트 방향 수정 기록 참조.
- 내장 이미지 편집 도구로 생성한 왼손 그립 수정본을 WebP 품질 86으로 변환하여 실제 포스트 파일에 교체.
- 종이 위에 놓인 손도 수정해야 한다는 판단은 잘못이었으며, 사용자가 요청하지 않은 추가 수정 작업은 중단하고 그 결과는 사용하지 않음.
- 아래는 선택한 이미지 생성에 실제 사용된 프롬프트 기록. 당시 양손을 수정하려던 지시는 요청 범위를 넓힌 잘못된 판단이었음. 이 기록은 후속 수정 지침이 아님.

```text
Use case: precise-object-edit.
Input image: edit target, the watercolor office illustration of an older woman and a younger man working with a TEAM GUIDE binder.
Fix ONLY the HANDEDNESS of the older woman's TWO HANDS. Her hands were accidentally drawn as the opposite hands on their respective arms. This is not an arm-position change. Keep both wrists, forearms, elbows, shoulders, faces, bodies, clothing, props, room, lighting, framing, and watercolor style fixed.

1. WRITING HAND, centered at approximately x=580,y=505 in this 1672x941 image: it connects to the woman's anatomical LEFT arm, on the viewer-right side of her body. Redraw it as an anatomically correct LEFT HAND holding the pen in a natural left-handed tripod grip. The thumb emerges from the radial edge on the VIEWER-LEFT / LOWER-LEFT side of this hand, opposing the index finger around the pen. Do not put the thumb on the viewer-right edge as in a mirrored right hand. The index finger curves over the pen, middle finger supports it, ring finger and little finger curl on the opposite outer edge, consistent with a real left hand. Make thumb-to-wrist continuity unambiguous. Pen tip touches the same binder page. Do not move the pen to her other arm.
2. RESTING HAND, approximately x=280,y=540 on the corrected report, connects to her anatomical RIGHT arm, on the viewer-left of her body. Redraw as an anatomically correct RIGHT HAND, palm down and back of hand visible, with four fingers extending diagonally toward the lower-right. Its short opposing thumb must be on the UPPER-RIGHT / binder-facing side of that hand, not the outer viewer-left edge. The little finger belongs on the lower-left outer edge. Make the short thumb distinct from the four longer fingers.

Use actual left-hand and right-hand anatomy, not mirrored copies. Exactly one thumb and four fingers per hand, naturally separated or occluded. Do not swap hands' positions, do not swap the arms or their tasks, do not hide the error by hiding either hand. Do not flip the whole image. Leave the man's hands and all other image details unchanged. Preserve wide 16:9 composition. No annotations, arrows, circles, extra text, or new objects.
```


### 노트를 인물이 읽는 방향으로 수정

- 노트 방향 수정 당시 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-d1673ab3-3ddc-464f-846a-56281e5244fd.png`. 현재 최종 원본은 아래 노트 옆 문서 수정 기록 참조.
- 최종 파일: `content/posts/geoff-9-workslop/illustration-reusable-knowledge.webp`
- 내장 이미지 편집 도구 사용. 노트 제목과 페이지 내용을 인물 기준으로 읽히도록 180도 회전. 관찰자에게는 제목이 거꾸로 보이고 체크박스는 글의 오른쪽에 위치.
- 앞서 수정한 펜 그립과 종이 위 손, 나머지 인물·장면 유지. 본문·캡션 변경 없음.
- WebP 품질 86으로 변환해 포스트 이미지 파일 교체.

```text
Use case: precise-object-edit.
Input image: edit target, the existing watercolor office scene with two people and the open TEAM GUIDE ring binder.

Change ONLY the printed/written CONTENT on the TWO PAGES of the central open ring binder so the PEOPLE sitting behind the desk can read and write it. Currently the pages face the camera, which is incorrect. The people are on the TOP side of the image; the camera is on the BOTTOM side.

Rotate each page's entire content by 180 DEGREES WITHIN THE PLANE OF THE PAPER. The title "TEAM GUIDE" must be genuinely UPSIDE DOWN to the camera/viewer, located near the BOTTOM/FOREGROUND edge of its page, not at the edge nearest the man. The top of every letter points toward the bottom edge of the image. Do NOT mirror the letters left-to-right: rotate the lettering 180 degrees as a whole. A person sitting where the man and woman sit must see the title upright. The checkboxes, checkmarks, paragraph lines, indentation and all other marks on BOTH pages must follow that same reader orientation. On the checklist page, checkboxes will appear on the VIEWER-RIGHT of the text lines after rotation, because they are on the seated readers' left. Ensure the content fits the existing paper perspective. The pages remain lying flat on the table.

Keep the physical binder, ring spine, page shapes, tabs and their positions fixed. Keep BOTH PEOPLE AND ALL FOUR HANDS EXACTLY as in the input, especially the woman's corrected LEFT hand holding the pen and her RIGHT hand resting on the loose report. No hand edits or pose changes. Keep the loose reports, laptop, furniture, wall posters, room, faces, clothing, lighting, palette, watercolor texture and 16:9 framing unchanged. Do NOT rotate the whole scene or the people. Do NOT add any labels, annotations, arrows, objects or new text. Only reorient the ink on the two binder pages. It is essential that "TEAM GUIDE" is NOT readable upright to the camera.
```


### 노트 옆 문서들도 인물이 읽는 방향으로 수정

- 최종 원본: `/Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-597d9dbf-9b54-405c-ac4b-c4fb2a65522b.png`
- 최종 파일: `content/posts/geoff-9-workslop/illustration-reusable-knowledge.webp`
- 내장 이미지 편집 도구로 왼쪽 교정 문서, 오른쪽 체크리스트, 오른쪽 서류 더미 최상단 문서의 내용 방향 수정.
- 오른쪽 체크박스 열과 체크 표시, 서류 더미의 노란 메모 위치를 회전. 첫 결과에서 남아 있던 왼쪽 교정 표시를 추가 수정하여 원과 X가 종이 왼쪽으로 이동하고 X가 원보다 위에 오도록 반영.
- 중앙 노트의 방향과 인물·손·펜 그립은 유지. 본문·캡션 변경 없음.
- WebP 품질 86으로 저장하여 실제 포스트 파일 교체. 생성 원본은 보존.

첫 편집 프롬프트:

```text
Use case: precise-object-edit.
Input image: edit target, the watercolor office illustration whose central TEAM GUIDE binder is already correctly oriented upside down to the camera.

Rotate the LOOSE PAPERS beside the binder 180 degrees in the plane of the desk so the two seated people can read them, not the camera. Apply this to all THREE visible paper surfaces:
1. The corrected report beneath the woman's resting hand at viewer-left: rotate its entire printed layout AND red correction marks together by 180 degrees within the page.
2. The loose checklist between the binder and laptop at viewer-right: rotate the entire checklist layout, including the teal checkmark and boxes, by 180 degrees. The boxes must end up on the VIEWER-RIGHT side of the text rows, and the checkmark must be upside down to the camera, upright to the seated man.
3. The top sheet on the foreground-right document stack: rotate that page's full printed layout and the attached yellow sticky note together by 180 degrees, keeping the stack itself in place.

The people are seated at the TOP side of the image. The top of the content on every paper therefore points toward the BOTTOM/FOREGROUND edge, consistent with the already-correct upside-down TEAM GUIDE title. Rotate, do not mirror. Preserve realistic perspective of the paper surfaces. No need to add any readable text.

Keep the loose sheets' footprints, position and paper contours fixed; reorient their contents as if the sheets were turned around in their current positions. Keep the central binder and its already-correct pages EXACTLY UNCHANGED. Keep all FOUR HANDS, pen grip, arms, faces, bodies, laptop, table, document tray and its NEXT label, plants, wall posters and every other element EXACTLY UNCHANGED. Do not modify any hand, arm or anatomy. No new annotations, arrows or objects. Preserve the watercolor texture, lighting, palette and full wide 16:9 framing. This is only a paper-orientation correction.
```

왼쪽 문서 추가 수정 프롬프트:

```text
Use case: precise-object-edit.
Edit target: supplied watercolor illustration with correctly oriented central binder and right-side papers.

Correct ONLY the loose report under the woman's resting hand on the LEFT. Its ink layout did NOT rotate in the last edit. Rotate the ENTIRE CONTENT OF THAT ONE SHEET 180 degrees in its own plane, including every gray text line, all red underlining, the red ellipse and the red X.

Concrete required visible result: the red ellipse that is currently on the RIGHT-HAND side of the left sheet MUST move to the LEFT-HAND side of that sheet. The red X currently BELOW that ellipse must move ABOVE the ellipse after the 180-degree rotation. The left sheet's red circle and red X should therefore both be in the LEFT half of the sheet, with the X closer to the woman and the circle closer to the camera. Rotate the paragraph spacing and underline positions consistently; do not leave any duplicate circle or X in their old right-side positions. This is rotation, not mirroring or moving just a single symbol.

Keep the woman's resting hand EXACTLY unchanged and in front of the page; allow it to occlude whatever rotated ink falls behind it. Keep that sheet's outline and location unchanged. Do not move, resize or redraw hands, pen, people, central TEAM GUIDE binder, right checklist, yellow sticky note, stack or any other object. All other surfaces already have their correct orientation. Preserve the input watercolor style, faces, gestures, room, palette and full wide 16:9 composition. No new marks or readable text. Edit only the left loose paper's ink.
```
