# Durable Execution image production

2026-09-21. Built-in imagegen for6 editorial illustrations; Mermaid diagram skill for4 SVGs with editable source/Excalidraw and PNG previews in `_workspace/durable-execution-visuals-2026-09-21/`. All publication images fit800×500. No captions. UI fields in illustrations are fictional examples, not actual customer data or product screenshots. No empirical performance charts were invented.

## Mapping

- 들어가며: thumbnail.webp — ERP에는 발주가 생성됐지만 에이전트는 완료 응답을 받지 못한 가상 상황
- AI는 답변을 끝냈지만 업무는 내일까지 이어집니다: illustration-wait.webp — 승인 대기 상태를 보존하고 다음 날 응답 후 업무를 재개하는 예시
- 이미 끝낸 단계는 어떻게 건너뛸까?: figure-replay.svg — 실행 이력에 기록된 조회·초안 결과를 재사용해 승인 대기 상태를 복원하는 구성
- 발주는 성공했는데 성공 기록을 못 남겼다면?: figure-response-loss.svg — 발주 성공 후 응답 유실과 멱등 키를 지원하는 ERP의 기존 결과 반환 흐름
- 보험 AI는 며칠 뒤 온 서류를 어떻게 이어 처리할까?: illustration-insurance.webp — 추가 서류를 기존 접수 건에 연결해 검토와 회신을 이어가는 보험 업무 예시
- 호텔 결제에서는 장애 뒤의 뒷정리가 달라졌습니다: illustration-payments.webp — 장애로 중단된 결제 관련 업무의 복구와 재개를 확인하는 운영자들
- 어제 받은 승인으로 오늘 바뀐 발주를 보내도 될까?: figure-approval-version.svg — 승인 대상과 실행할 문서 버전을 비교하고 변경 시 재승인으로 보내는 흐름
- 다시 시도할 일과 멈춰야 할 일: figure-failure-routing.svg — 통신 오류·입력 오류·승인 거절·결과 불명·취소에 맞춰 대응을 나누는 도해
- 우리 회사에서는 무엇부터 시험할까?: illustration-testing.webp — 테스트 환경에서 복원·중복 실행 방지·실패 시 인계를 확인하는 장면
- 나가며: illustration-operations.webp — 완료한 일과 남은 일, 다시 실행할 수 있는 일을 구분하는 현업과 개발자

## Raster prompts

### thumbnail

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Procurement employee pauses before retrying a purchase order. Two large screens: left "AI 화면" / "완료 응답 없음", right "ERP" / "발주 생성됨". Broken return arrow between them, showing successful remote action but lost acknowledgement, not failed order. Heading "방금 그 발주, 다시 눌러도 될까요?" Small label "가상 업무 예시".

### illustration-wait

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Two connected office vignettes today and tomorrow, same work folder with saved progress note. Left worker submits request heading "오늘 · 승인 대기"; right manager reviews and approves heading "내일 · 응답 후 재개". Central small saved record icon "업무 상태 보존". No timer statistics.

### illustration-insurance

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Insurance operations practitioner receives missing PDF from customer and continues existing case rather than starting a new case. Desk folder "진행 중인 접수 건", incoming document "추가 서류 도착", screen shows "문서 확인 → 담당자 판단 → 회신". Generic illustrative workflow not actual Strada staff. No sensitive personal data.

### illustration-payments

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Hotel payment operations staff comparing pending transaction list and recovered processing queue after service outage. Screen labels "일시 중단된 업무" then "복구 후 재개". Hotel reception visible discreetly in background. No fabricated figures, no before-after performance graph, no logos. Show staff checking traceable progress not manually retyping all transactions.

### illustration-testing

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Engineer and business owner deliberately testing order recovery in safe test environment. Screen "테스트 환경", checklist three unchecked rows "중단 후 복원" "중복 실행 방지" "실패 시 인계". Person checks test results without all-green success claims; no real payment/card data.

### illustration-operations

Editorial gouache illustration for Korean executive tech blog. Landscape16:9, warm cream, navy and teal with coral warning accents. Professional adults, natural correct hands, readable sparse Korean labels. Not chibi, no robots, no random slogans or wall text. Show real work mechanism rather than atmosphere. Business practitioner explains exception handling to engineer with one open case at desk. Three simple readable desk cards "완료한 일" "남은 일" "다시 해도 되는 일". Collaborative specific review, coherent paper orientation, no random text or fabricated metrics.

## QA

Raster outputs and all4 rendered diagram PNGs inspected. Response-loss diagram explicitly conditions duplicate suppression on ERP idempotency-key support. Replay diagram reuses only recorded results. Approval diagram separates changed documents from executable approved versions. No real client faces or dashboard statistics asserted.
