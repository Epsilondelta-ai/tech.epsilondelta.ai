# AI Evals 포스트 이미지 제작 기록

- 제작일: 2026-09-10
- 대상: content/posts/geoff-10-ai-evals/index.md
- 요청: 섹션별 이미지 한 장 정도, 실제 파일 폭 최대 800px, 캡션 없음.
- 구성: 내장 이미지 생성 도구로 만든 래스터 5장(썸네일 1·실사풍 가상 장면 1·일러스트 3), SVG 도해 3장. 총 8장.
- 이미지 제작 단계에서는 기존 본문·표·출처 링크·공개 상태를 유지하고 이미지 링크와 대체텍스트, 썸네일 메타데이터만 추가.
- 사진처럼 보이는 협업 장면은 실제 기업의 촬영 사진이 아니며, 가상 예시 문단에 배치하고 대체텍스트에 AI 생성 가상 장면임을 명시.
- 기존 승인된 글을 윤문하거나 내용을 새로 추가하지 않음.
- 이미지 생성 전 스냅샷: _workspace/2026-09-10-ai-evals-images/index-before-images.md

## 섹션별 배치

| 섹션 | 이미지 | 종류 | 설명 목적 |
|---|---|---|---|
| 들어가며 | [thumbnail.jpg](../content/posts/geoff-10-ai-evals/thumbnail.jpg) | 일러스트 썸네일 | 우리 회사의 업무 사례와 합격 기준으로 AI 산출물을 검증하고 통과·수정 대상을 구분 |
| 그래서 Evals가 뭔데? | [figure-evaluation-loop.svg](../content/posts/geoff-10-ai-evals/figure-evaluation-loop.svg) | 도해 | 사례·기준 준비부터 실제 시스템 실행, 답변·행동·결과 확인과 재시험까지의 관계 |
| 시험문제는 현업 담당자와 함께 만듭니다 | [photo-evaluation-workshop.webp](../content/posts/geoff-10-ai-evals/photo-evaluation-workshop.webp) | 실사풍 가상 장면 | 현업과 기술 담당자가 실제 업무 자료와 수정 요청으로 평가 사례를 만드는 협업 |
| 같은 견적 요청에 답한 AI 셋을 채점해봅시다 | [figure-quote-evaluation.svg](../content/posts/geoff-10-ai-evals/figure-quote-evaluation.svg) | 비교 도해 | 초안 거절·정확한 초안과 승인 필요 표시·무단 발송의 평가 결과 구분 |
| 계산과 내용은 어떻게 나눠서 채점할까? | [figure-oscar-evaluation.svg](../content/posts/geoff-10-ai-evals/figure-oscar-evaluation.svg) | 데이터 도해 | Oscar 첫 개발 배치의 항목별 결과와 각 성공 기준을 같은 척도로 비교 |
| 시험 속 고객이 너무 친절했습니다 | [illustration-customer-simulation.webp](../content/posts/geoff-10-ai-evals/illustration-customer-simulation.webp) | 일러스트 | 모의 고객의 정제된 입력과 실제 고객의 정보 누락·다양한 표현·요구 차이 |
| 합격한 AI도 업무가 바뀌면 다시 시험합니다 | [illustration-regression-check.webp](../content/posts/geoff-10-ai-evals/illustration-regression-check.webp) | 일러스트 | 같은 업무 사례로 변경 전후를 재시험하고 새로 실패한 항목을 찾아내는 과정 |
| 나가며 | [illustration-shared-eval-library.webp](../content/posts/geoff-10-ai-evals/illustration-shared-eval-library.webp) | 일러스트 | 현업의 교정을 공용 평가 사례로 정리하고 다음 업무에서도 재사용 |

## 저장 및 표시

- 썸네일은 JPEG, 본문 생성 이미지는 WebP로 저장.
- 생성 원본 PNG에서 가로 800px로 비율 유지 축소. JPEG 품질 85, WebP 품질 86.
- SVG도 width=800이며 viewBox를 같은 800px 기준으로 설계. 글자와 그래프는 벡터로 유지.
- 코드나 CSS로 표시 폭을 제한하는 방식이 아니라 이미지 파일 자체 크기를 맞춤.
- 그림 아래 캡션이나 그림 번호는 추가하지 않음.
- 모든 이미지에 내용에 맞는 alt 제공. SVG는 원본을 열 수 있는 링크도 유지.
- 썸네일을 featured_image와 images에 지정. 이미지 제작 당시에는 draft=true로 유지했으며, 이후 게시 준비에서 사용자 지정에 따라 draft=false임을 확인.

## SVG 설계와 데이터 검증

- figure-evaluation-loop.svg: 업무 사례·합격 기준 → 실제 AI 시스템 실행 → 답변·행동·파일/시스템 상태 확인 → 합격/실패 기록. 모델·지침·자료·도구가 바뀌면 같은 사례로 재시험. 평가 통과가 즉시 배포나 자동 학습으로 이어지는 그림이 아님.
- figure-quote-evaluation.svg: 가상 회사의 10% 초과 할인 확정·발송에는 부서장 승인이 필요. 20% 견적 초안 요청에서 A는 초안도 거절해 평가 실패, B는 정확한 초안과 승인 필요 표시를 남기고 확정·발송하지 않아 평가 합격, C는 승인 없이 발송해 평가 실패. B의 평가 합격과 실제 견적 승인을 구분.
- figure-oscar-evaluation.svg: Oscar Health의 첫 개발 배치 451개 질문. 사실·출처 84%/기준90%, 빠짐없는 답변 92%/90%, 질문 관련성 99%/90%, 명료성·말투 100%/99%. 네 막대는 같은 0~100% 척도. 결과와 기준은 별도 열과 기준선으로 표시. 종합 점수는 계산하지 않음.
- 도해 내부 제목·축·범례·필수 조건은 설명 요소로 포함. 본문 캡션은 없음.
- SVG에 title/desc 제공. 스크립트와 외부 의존성 없음.

## 실제 생성 프롬프트

모두 내장 이미지 생성 도구로 새 이미지를 생성했다. CLI/API로 별도 생성하거나 모델을 바꾸지 않았다. 아래 원본 PNG는 생성 디렉토리에 보존하며 포스트에서는 축소한 파일을 사용한다.

### 1. thumbnail.jpg

원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-2ddf3f9b-a64b-48c4-8a71-bb81d3cc9294.png

~~~text
Use case: illustration-story.
Asset type: Korean executive tech blog thumbnail about AI Evals: testing an AI on the company's actual work before trusting it.
Create a polished editorial illustration, wide 16:9, with crisp ink contours and restrained gouache color on a warm ivory background. A tangible quality-check workbench for business AI, not a generic office or abstract AI atmosphere. At left, a small upright folder of varied business task cards (a quotation sheet, a meeting note, a customer request) and a separate acceptance-checklist card. In the center, a compact tabletop computing module clearly marked "AI" takes one task card; beside it is its completed business document. At right, an inspection area compares that result with the separate checklist: one checked document in a teal accepted tray and one marked document in a coral revision tray. The visual story is company tasks plus acceptance criteria, AI execution, then evidence-based pass/fail. Make the workbench and documents the dominant subject, simple enough to understand at thumbnail size.
Only large title text "AI EVALS" near the upper left and the small module label "AI"; all other page contents are tidy abstract marks and diagrams, no invented statistics or readable report names. Use ivory, dark navy, muted teal and a small coral accent. No robots, human hands, faces, glowing brains, network clouds, floating arrows, office plants, motivational slogans, extra text or logos. Keep the composition spacious and visually coherent. This is an explanatory illustration, not a fake screenshot or certificate.
~~~

### 2. photo-evaluation-workshop.webp

원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-da40032a-1f7a-4e6a-8ca1-a249ef7c46f6.png

~~~text
Use case: photorealistic-natural.
Asset type: illustrative editorial photo for a blog section explaining that domain experts and engineers build AI evaluation cases together.
A candid staged scene in a bright modest meeting room: two adult Korean colleagues, one business operations specialist and one software engineer, stand side by side facing the SAME large whiteboard. Camera is behind and slightly to their side, looking in the SAME direction they are reading. On the board, real-looking but entirely fictional meeting-note and quotation printouts with a few red corrections are grouped beside cleaner test-case sheets and a checklist. The board should visibly show the action of turning actual work and corrections into evaluation examples, not just people in a meeting. Three short headings on the board ONLY: "업무 자료", "확인할 조건", "평가 사례", large clean Korean lettering.
People shown waist-up from rear three-quarter view, no face close-ups; both arms stay naturally connected with relaxed modest gestures. One person may point naturally at a printout with a clearly attached forearm; the other looks at the same item. No crossed or intertwined arms, no extra limbs, no papers turned toward the camera while people read their backs. Board contents are oriented upright to both the colleagues and camera. No prominent loose tabletop documents.
Natural daylight, real fabric and paper texture, realistic proportions, restrained navy/teal clothes, light neutral room. Wide 16:9. No visible corporate logos, bank names, customer identifiers, fake quotations, charts with numerical claims, laptop screens facing away from their users, watermarks, lower-third captions or decorative slogans. This is a generic fictional scene, NOT a photograph of Morgan Stanley or a real client's office.
~~~

### 3. illustration-customer-simulation.webp

원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-58545ece-8ca7-42a2-b978-6c5ca64128eb.png

~~~text
Use case: illustration-story.
Asset type: explanatory editorial illustration comparing an overly cooperative simulated customer with varied real customer requests, for an AI Evals blog.
Wide 16:9 two-part editorial composition with crisp ink drawing, light ivory background and restrained navy, teal and coral color. At left, a clearly simulated customer avatar inside a testing screen has one neatly organized speech bubble containing orderly information blocks, all slots filled; a support AI icon receives it with an easy check. At right, three distinct everyday adult customers (a commuter carrying a bag, an adult checking a ride on a phone, and an adult asking for assistance) appear in small natural head-and-shoulder vignettes. Their speech bubbles contain uneven short fragments, one visibly missing information slot, and a repeat-request bubble. Show differences in completeness, expression and conversational goals, NOT people being stupid, dishonest, aggressive or scary. Real users are ordinary people with limited time.
Use ONLY these two large Korean headings, each centered above its side: "시험 속 고객" on the left and "실제 고객" on the right. Optional short bubble text on the right ONLY "환불해 주세요" and "상담원 연결"; other bubble marks abstract and simple. No percentages or scores. No company logos. Hands, if visible, must belong clearly to the same person's arm with plausible anatomy and correct thumbs, but keep head-and-shoulder framing and focus on faces and conversations, not hands. Avoid intricate device-gripping close-ups.
Visually communicate why realistic customer behavior makes a better test. Not a flowchart full of arrows, not generic office wallpaper, no caption strip, no unrelated decorative words.
~~~

### 4. illustration-regression-check.webp

원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-c7e40426-710e-4f37-95d0-e77a0e5e9722.png

~~~text
Use case: illustration-story.
Asset type: editorial illustration for retesting the same company work after changing an AI model or its instructions.
Wide 16:9 clean editorial ink and subtle gouache illustration on warm ivory, navy, teal and coral accents. A practical evaluation workbench, seen at a slight overhead angle, with one reusable set of business-case cards in a holder in the center. On either side are two identical small desktop testing consoles labeled ONLY "V1" and "V2". Each console shows the SAME four task rows in the same order using simple recognizable document icons. V1 has four small teal checks; V2 has three teal checks and one clearly coral review mark on the matching second row. These are illustrative task outcomes, not reported statistics. The shared case cards make it clear that the comparison uses the same tests. Place a small changed instruction sheet beside V2 to show that it is the updated version.
No people or hands. All sheets rest on the desk or in physical holders, nothing levitates. All screen and paper marks follow their actual surface perspective. Only "V1" and "V2" are readable text; no percentages, charts claiming benchmark results, magic sparkles, red alarm scenes, arrows floating across objects, extra labels or corporate logos. The picture explains finding a newly failing task after an update, not saying every update is worse. Maintain a clear visual hierarchy and plenty of space, without looking like a dense software dashboard.
~~~

### 5. illustration-shared-eval-library.webp

원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-10e9537e-798a-455d-83ce-6ccb7f1a87ef.png

~~~text
Use case: illustration-story.
Asset type: concluding editorial illustration showing a company's practical know-how preserved as reusable evaluation cases.
Create a wide 16:9 refined editorial still-life, crisp ink contours with restrained gouache shading, warm ivory, dark navy, teal and small coral corrections. At left on a desk is one believable business document with a few corrected lines and a checklist attached; in the center is a low, open company archive drawer with neatly indexed reusable case cards, each card pairing a short task block with an acceptance checklist. Some cards have tabs for normal requests, some for exceptions, visually distinguished only by simple icons. At right, a fresh task card from the same archive stands in a small holder beside a new blank work document, suggesting the team will use the accumulated criteria again on the next task.
The archive's front label may read ONLY "TEAM EVALS" in clean, legible letters. No other readable text, numbers or slogans. The dominant relationship is correction from real work becoming a shared, organized set of test cases, then being reused. Make this a tangible organized collection, not a glowing cloud, abstract network, generic bookcase, decorative office or school exam.
No people, hands or arms. All paper is physically supported, and its orientation is consistent with the desk viewpoint. No floating arrows, confetti, robots, fake client names, watermark, captions or diagrams claiming real measured outcomes. Keep the composition calm and specific to reusable company evaluation knowledge.
~~~

## 확인 사항

래스터 이미지의 설명 목적, 큰 글자, 사람의 손·팔 연결과 문서 방향을 확인했다. 도해 세 장은 PNG로 렌더링해 글자 겹침과 수치를 확인했다. 검수용 PNG는 _workspace/2026-09-10-ai-evals-images/에 보관한다.

최종 검증:

- 실제 파일 폭 8장 모두 800px. 썸네일 800×450, WebP 4장 800×451, SVG 800×520·800×540·800×560.
- 전체 이미지 용량 328,599바이트(약 321KiB).
- 8개 H2에 각각 이미지 1장. 캡션 0개.
- 기존 본문·표 2개·링크 10개·문의 CTA·draft 상태 보존 확인.
- Hugo 초안 포함 빌드 성공. 출력된 8개 이미지와 원본 파일 바이트 일치, 공유 썸네일 경로 확인.
- 기존 다른 포스트의 raw HTML 경고는 이 작업에서 변경하지 않음.
- 이미지 제작 당시에는 커밋·푸시하지 않았으며, 이후 사용자가 main 게시 커밋·푸시를 요청함.
