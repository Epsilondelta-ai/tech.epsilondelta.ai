# Agentic Commerce 포스트 이미지 제작 기록

- 제작일: 2026-09-11
- 대상: content/posts/geoff-11-agentic-commerce/index.md
- 방식: imagegen 스킬과 내장 이미지 생성 도구. 별도 API·CLI 이미지 생성은 사용하지 않음.
- 요청: 썸네일과 섹션별 설명 이미지, 실제 파일 폭 최대 800px, 캡션 없음.
- 구성: 썸네일 1장, 본문 인포그래픽 3장, 상황 일러스트·실사풍 개념 이미지 4장. 총 8장.
- 저장 형식: 모든 파일 WebP, 800×451px. cwebp 품질 86으로 비율 유지 축소.
- 총 용량: 409,466바이트(약 400KiB).
- 이미지 생성 전 원고: _workspace/2026-09-11-agentic-commerce-images/index-before-images.md
- 본문과 표, 기존 출처, 사용자가 수정한 문의 문장, draft=true를 그대로 유지. 이미지·alt와 썸네일 메타데이터만 추가.
- 그림 아래 캡션·그림 번호는 없음. 그림 내부의 제목·라벨은 설명 요소.
- 실제 기업의 화면·촬영 사진으로 제시하지 않고 해당 장면의 alt에 가상·개념 이미지임을 명시.

## 배치와 설명 목적

| 섹션 | 파일 | 설명 목적 |
|---|---|---|
| 들어가며 | [thumbnail.webp](../content/posts/geoff-11-agentic-commerce/thumbnail.webp) | 정보가 부족한 상품과 비교 가능한 상품의 차이, 고객 확인 후 주문 |
| 고객이 쓰는 AI가 새로운 구매 창구가 됩니다 | [illustration-customer-shopping.webp](../content/posts/geoff-11-agentic-commerce/illustration-customer-shopping.webp) | 고객이 여러 판매자의 상품을 AI의 후보 목록으로 보는 구매 접점 |
| 이미 식단을 짜고 장바구니를 채웁니다 | [illustration-recipe-to-cart.webp](../content/posts/geoff-11-agentic-commerce/illustration-recipe-to-cart.webp) | 레시피에 필요한 재료를 실제 구매할 식료품으로 연결 |
| AI는 우리 상품이 고객 조건에 맞는지 알 수 있을까? | [figure-product-comparison.webp](../content/posts/geoff-11-agentic-commerce/figure-product-comparison.webp) | 같은 예산·무게·수령일 조건으로 A·B·C 후보 비교 |
| 추천은 받았는데 주문할 수 없다면 | [figure-order-confirmation.webp](../content/posts/geoff-11-agentic-commerce/figure-order-confirmation.webp) | 최종 조건, 고객 승인, 실제 주문 접수와 배송 확인을 구분 |
| GEO와 쇼핑 프로토콜은 어떻게 맞물릴까? | [figure-geo-shopping-paths.webp](../content/posts/geoff-11-agentic-commerce/figure-geo-shopping-paths.webp) | 웹 검색과 카탈로그 조회가 같은 비교·추천에 함께 쓰이는 관계 |
| 전 상품을 한꺼번에 연결할 필요는 없습니다 | [illustration-limited-catalog.webp](../content/posts/geoff-11-agentic-commerce/illustration-limited-catalog.webp) | 전체 상품군 중 일부부터 상품 데이터와 판매를 연결 |
| 나가며 | [illustration-ready-to-sell.webp](../content/posts/geoff-11-agentic-commerce/illustration-ready-to-sell.webp) | 실제 상품·상품 정보·주문 이행을 일치시키는 운영 준비 |

## 검수와 보정

- 썸네일 초안의 임의 예산·무게·금액·배송일을 본문과 맞춰 수정했다. 고객 조건은 배송비 포함 150만 원 이하, 1.3kg 이하, 9월 15일까지 도착. 비교 가능한 후보는 1.28kg·149만 원·9월 14일이다.
- 식료품 이미지의 재료를 잘못 연결할 소지가 있는 점선·화살표를 제거했다. 화면과 장바구니에 같은 파스타·토마토·시금치·두부를 배치해 대응 관계를 전달한다.
- 상품 비교의 A는 1.20kg·151만 원·9월 14일, B는 1.25kg·141만 원·9월 18일, C는 1.28kg·149만 원·9월 14일. C는 최고 상품·구매 확정이 아니라 조건 충족 후보다.
- 주문 그림에서 고객 구매 승인과 판매자 주문 접수를 구분했다.
- GEO 그림에서 두 정보 경로가 같은 비교·추천에 연결된다. 서로 배타적인 GEO 전용·프로토콜 전용 단계로 표시하지 않았다.
- 인물은 고객 한 명의 뒷모습 또는 단순 아바타로 표현해 부자연스러운 손·팔 동작을 피했다.
- 생성 원본과 축소본의 구도·사물 대응·문구·수치를 확인했다. 인포그래픽 3장은 별도 검토자도 800px 파일로 확인했다.
- 최종 8개 H2에 각각 이미지 1장. 파일 폭 모두 800px, 캡션 0개.
- 이미지 링크와 썸네일 필드만 제거한 원고가 작업 전 스냅샷과 동일함을 검사했다.
- 원본 PNG는 생성 디렉토리에 보존했다. 프로젝트에서는 해당 포스트 디렉토리의 축소본을 사용한다.

## 실제 생성 프롬프트

### thumbnail.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-28d12309-48eb-41d8-8f2c-34dbc7ed2723.png

~~~text
Create one polished wide 16:9 raster image for a Korean executive-facing technology blog about Agentic Commerce. It will be displayed at only 800 pixels wide, so use generous spacing, simple legible shapes, and very large typography wherever text is requested. Neutral warm-white background, dark ink outlines, restrained blue-green accents, subtle tactile editorial print texture, no neon sci-fi mood. No watermarks, real company logos, invented statistics, or tiny unreadable interface text. The illustration must explain the stated concept, not decorate empty space.
Use case: illustration-story. Asset type: article cover. Show a clear left-to-right visual story: a customer's speech bubble with icons for budget, laptop weight, and a delivery calendar; in the center an AI chat/search interface compares two DISTINCT laptop product cards: the first is subdued and shows visibly empty weight, total-cost and delivery-date fields with question marks; the second clearly shows completed attribute rows with weight, budget and calendar icons and is outlined as an eligible candidate; to the right the selected laptop is shown in a HUMAN purchase-confirmation screen, then a parcel ready for shipping. Draw one small human customer head icon immediately above the purchase-confirmation screen to show the person approves before purchase, no human arms or hands. Keep the laptop and box recognizably related. Main headline at top in large precise Korean: "고객의 AI가 고르는 상품". Other text, as large short labels beneath the three main regions: "고객 조건", "상품 비교", "구매 확인". The two compared cards carry the short labels "정보 부족" and "비교 가능". Use these exact labels only. Highlight preparation of usable product information, not the claim that any connected product is guaranteed to win. Subtle directional connectors serve the explanation. This is a conceptual illustration, not a real product UI. Do not imply autonomous purchase without confirmation. No robot mascot.
~~~

수정 프롬프트:

~~~text
Edit only the numerical details and request text in this existing thumbnail so it matches the article's fictional laptop example. Preserve the exact current illustration, arrangement, people, laptop drawings, colors, icons and all main labels. In the customer speech bubble replace the budget with "배송비 포함 150만 원 이하", replace the light-laptop request with "무게 1.3kg 이하", replace the delivery request with "9월 15일까지 도착". On BOTH the green comparison card and the purchase-confirmation card change weight to "1.28kg", total cost to "149만 원", and delivery date to "9월 14일". The information-missing card must KEEP its three question marks. Keep the main title "고객의 AI가 고르는 상품", and labels "고객 조건", "상품 비교", "구매 확인", "정보 부족", "비교 가능". Do not change any other visual elements. Text must be readable, exact and aligned. Do not add any new values or claims.
~~~

### illustration-customer-shopping.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-ffe57624-ed40-462c-b6f8-ced4be9cfa41.png

~~~text
Create one polished wide 16:9 raster image for a Korean executive-facing technology blog about Agentic Commerce. It will be displayed at only 800 pixels wide, so use generous spacing, simple legible shapes, and very large typography wherever text is requested. Neutral warm-white background, dark ink outlines, restrained blue-green accents, subtle tactile editorial print texture, no neon sci-fi mood. No watermarks, real company logos, invented statistics, or tiny unreadable interface text. The illustration must explain the stated concept, not decorate empty space.
Use case: illustration-story. Asset type: explanatory editorial scene. A single customer at home planning a trip: three-quarter rear view of an adult seated comfortably looking at an upright tablet on a stand. Both hands rest separately and naturally in their lap, mostly hidden below the desk; do not draw any pointing hands. The tablet screen, facing the person and seen obliquely by the viewer, shows a speech bubble above three small laptop comparison cards with a single selected candidate. A small travel suitcase is near the chair. Behind and beyond the tablet, an editorial cutaway of three distinct generic online shop windows with laptop products suggests the agent compares multiple sellers before the customer visits a store. No arrows crossing the person, no shopping cart full of unrelated goods. No lettering anywhere. Bright calm daylight, sophisticated hand-drawn gouache illustration, believable object perspective. Message: the customer begins with an AI request and sees a shortlist instead of browsing each store separately.
~~~

### illustration-recipe-to-cart.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-b017c971-54ce-46af-b813-616402c280b4.png

~~~text
Create one polished wide 16:9 raster image for a Korean executive-facing technology blog about Agentic Commerce. It will be displayed at only 800 pixels wide, so use generous spacing, simple legible shapes, and very large typography wherever text is requested. Neutral warm-white background, dark ink outlines, restrained blue-green accents, subtle tactile editorial print texture, no neon sci-fi mood. No watermarks, real company logos, invented statistics, or tiny unreadable interface text. The illustration must explain the stated concept, not decorate empty space.
Use case: illustration-story. Asset type: concrete shopping example. A large smartphone standing at an angle on a kitchen counter shows an illustrated recipe card: a bowl of tomato, spinach and tofu pasta, with small clear ingredient pictures directly below it. Nearby, a real open grocery paper bag contains the SAME ingredients in purchasable forms: a pasta packet, tomatoes, a bunch of spinach, and a plain tofu box. In the background a small simple store shelf with these same groceries makes the link to available retail products clear. A short clean curved dotted path connects the recipe ingredients on screen to the corresponding grocery products, without stray strokes. No people, hands or logos. No English labels and no tiny text. One short large Korean title at top: "레시피에서 실제 장바구니로". Warm daylight, refined editorial gouache, material texture, not a sterile flowchart. Conceptual depiction, not a screenshot of Instacart or an assertion of completed payment.
~~~

수정 프롬프트:

~~~text
Remove ALL teal dotted connector lines and their arrowheads from this image, leaving clean background in their place. Preserve the phone, all four ingredient pictures, the recipe image, grocery bag, pasta packet, tomatoes, spinach, tofu package, shelves, lighting, composition and Korean title exactly. Do not alter ingredients, remove objects or add any arrows. This image should communicate the recipe-to-groceries relationship purely by the corresponding ingredients visible on the phone and in the bag. Keep everything else unchanged.
~~~

### figure-product-comparison.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-bb63dc7e-2e64-4b49-b3d2-35c12dba537e.png

~~~text
Create ONE finished raster illustration for a Korean executive-facing technology blog about Agentic Commerce, wide 16:9. Final display is only 800px wide. Use large, highly legible Korean sans-serif labels, clean spacing and very simple explanatory composition. Light warm-white background, dark ink, muted blue-green and small terracotta accents, subtle editorial print texture. No real logos, watermark, fake brand names, tiny text, extra invented facts or numbers. Every arrow, label and object must serve the explanation.
Use case: infographic-diagram. A polished illustrated comparison with THREE equally sized laptop candidate cards A, B, C. At top title: "같은 조건으로 비교하면?". A clear common requirements banner on two readable lines: "1.3kg 이하 · 배송비 포함 150만 원 이하" and "9월 15일까지 도착". Each card includes a small simple drawing of a laptop and exactly three facts followed by an outcome badge. Card A facts: "1.20kg", "총액 151만 원", "9월 14일 도착"; outcome "예산 초과" with a small orange cross next to TOTAL COST ONLY. Card B facts: "1.25kg", "총액 141만 원", "9월 18일 도착"; outcome "도착 지연" with a small orange cross next to DELIVERY ONLY. Card C facts: "1.28kg", "총액 149만 원", "9월 14일 도착"; outcome "조건 충족 후보" with a calm teal outline, not a winner trophy. C is an eligible candidate, NOT a completed purchase or best laptop. Spell all numbers and Korean verbatim. Do not add any data, ratings, percentages, payment button or caption strip. No people or hands. Keep the visual closer to a well-designed editorial comparison than a spreadsheet.
~~~

### figure-order-confirmation.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-1fd24d97-be60-427a-9307-a8e3e5bc8ac6.png

~~~text
Create ONE finished raster illustration for a Korean executive-facing technology blog about Agentic Commerce, wide 16:9. Final display is only 800px wide. Use large, highly legible Korean sans-serif labels, clean spacing and very simple explanatory composition. Light warm-white background, dark ink, muted blue-green and small terracotta accents, subtle editorial print texture. No real logos, watermark, fake brand names, tiny text, extra invented facts or numbers. Every arrow, label and object must serve the explanation.
Use case: infographic-diagram. Title at top: "추천 다음에는 실제 주문 확인". Four large illustrated checkpoints arranged clearly left to right with exactly three one-way arrows joining them. Checkpoint 1 shows a price tag, warehouse stock box and delivery calendar; label "최종 조건 확인". Checkpoint 2 shows a simple human head icon beside a purchase approval screen; label "고객 구매 승인". Checkpoint 3 shows a merchant order-record screen with a single order row and confirmation check; label "주문 접수 확인". Checkpoint 4 shows a parcel and delivery-status timeline; label "배송 상태 확인". All checkpoints are conceptual, not a particular product UI. Emphasize that customer approval precedes order placement and the merchant system must actually contain the order. No fictional order numbers, prices, dates, cards, percentages or extra text. No hands. Do not put an arrow that skips approval. Labels are large and readable at 800px; put them on two lines if needed.
~~~

### figure-geo-shopping-paths.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-ac5969fa-6a46-4a72-8ea3-aa9d76cccf96.png

~~~text
Create ONE finished raster illustration for a Korean executive-facing technology blog about Agentic Commerce, wide 16:9. Final display is only 800px wide. Use large, highly legible Korean sans-serif labels, clean spacing and very simple explanatory composition. Light warm-white background, dark ink, muted blue-green and small terracotta accents, subtle editorial print texture. No real logos, watermark, fake brand names, tiny text, extra invented facts or numbers. Every arrow, label and object must serve the explanation.
Use case: infographic-diagram. Explain two complementary information paths feeding the SAME AI product comparison. Main title "AI가 상품을 찾는 두 경로". On left upper row, a magnifying glass and web page icon labeled "웹 검색" leads to two readable document icons labeled "자료 확인". On left lower row, structured product cards labeled "상품 피드·카탈로그" lead to a specific laptop option card labeled "상품·옵션 조회". BOTH rows have arrows converging on ONE shared central result with three laptop candidate cards, labeled "비교·추천". From this shared result, ONE arrow leads to final transaction condition check icon labeled "최종 조건 확인", then to human-head approval plus shopping bag icon labeled "고객 확인·구매". Use spatial layout with the two paths stacked at left, merged comparison in middle, shared purchase sequence at right, clear non-crossing connectors. The paths may be combined; DO NOT label one as GEO-only and the other protocol-only. No ranking guarantees, no marks suggesting every product is recommended, no extra statistics. Large typography; simple enough to understand at 800px. This is an explanatory conceptual diagram, not a real service interface.
~~~

### illustration-limited-catalog.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-c847135e-2a99-43bf-b1a1-06fb8a87f43a.png

~~~text
Create ONE finished raster illustration for a Korean executive-facing technology blog about Agentic Commerce, wide 16:9. Final display is only 800px wide. Use large, highly legible Korean sans-serif labels, clean spacing and very simple explanatory composition. Light warm-white background, dark ink, muted blue-green and small terracotta accents, subtle editorial print texture. No real logos, watermark, fake brand names, tiny text, extra invented facts or numbers. Every arrow, label and object must serve the explanation.
Use case: illustration-story. A tangible clothing brand's product preparation space, refined editorial gouache, bright natural daylight. In the background a long apparel rack holds many different garments. In the foreground a SHORT separate rack clearly selects just ONE dress and ONE pair of jeans, with uncluttered space around them. Beside the short rack, a standing catalog screen shows exactly these same two selected clothing items as two product cards; a small open shipping box waits nearby. The long background rack should feel ordinary and intact, not rejected or discarded, making clear that the team starts with a limited assortment. One large Korean title only: "일부 상품부터 시작". No numerical sales claims, no arrows, logos, company name, analytics charts or unrelated furniture products. No people, body parts, mannequins or loose paperwork. This is a generic illustrative scene, not an actual photograph of URBN.
~~~

### illustration-ready-to-sell.webp

최종 선택 원본: /Users/epsilondelta/.codex/generated_images/01a06a28-88b9-7333-83e2-32ba5d507839/exec-1fc5fd48-c8b1-40c9-a0cf-0a1314982a87.png

~~~text
Create ONE finished raster illustration for a Korean executive-facing technology blog about Agentic Commerce, wide 16:9. Final display is only 800px wide. Use large, highly legible Korean sans-serif labels, clean spacing and very simple explanatory composition. Light warm-white background, dark ink, muted blue-green and small terracotta accents, subtle editorial print texture. No real logos, watermark, fake brand names, tiny text, extra invented facts or numbers. Every arrow, label and object must serve the explanation.
Use case: illustration-story. Make a specific, tactile still life inside a small brand's fulfillment workspace showing consistency between REAL PRODUCT, PRODUCT DATA, and FULFILLMENT. A slim plain silver laptop sits on a neat product inspection bench. Next to it a desktop monitor faces the viewer at a believable slight angle, showing the SAME silver laptop and three crisp attribute rows illustrated with weight, stock and delivery-calendar icons, no numeric values. On the other side, an open fitted cardboard shipping box has protective insert sized for that same laptop and a plain shipping-label block. A second closed parcel with a small laptop pictogram is ready on a short packing shelf. Connect the objects by physical proximity and matching product identity, NOT floating arrows or abstract networks. Main feeling: the brand has made accurate product information usable and can fulfill the resulting order. Warm daylight, refined hand-drawn gouache with convincing paper and metal texture. No people, hands, slogans, text, giant warehouse, fake logos or decorative office plants. No unrelated desk accessories.
~~~
