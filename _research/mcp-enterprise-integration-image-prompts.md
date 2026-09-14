# MCP 포스트 이미지 제작

내장 image_gen 사용. 섹션당 1장, 썸네일 포함 10장. 최종 파일은 모두 800×451px WebP. 본문 캡션 없음. 인물 장면은 가상 업무이며 실제 기업 현장을 재현하지 않는다.

## 최종 보정·검수

- 썸네일의 자동 추가 로고·장식 문구를 제거하고 인물이 보는 종이는 뒷면으로 수정.
- 호출 과정 그림의 의사 코드를 입력 항목으로 교체. 반환 경로는 ERP → MCP 서버 → AI 애플리케이션으로 분리.
- 업무 사례·재고 의미 그림의 관련 없는 벽면 문구 제거.
- 생성 결과 전체를 직접 시각 검토. 축소 후 썸네일·호출·보안 이미지의 글자와 흐름 재확인.
- 본문 문장 보존 확인. H2 10개에 이미지 10개. 기존 이미지·테마·CSS 수정 없음.

## 들어가며

파일: thumbnail.webp

대체 텍스트: AI의 답변을 ERP와 CRM에 옮겨 입력하는 직원과 끊긴 시스템 연결을 표현한 일러스트

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Illustration-story. Main subject: office employee visibly bridging three separate screens: left floating AI response document labelled 'AI 답변', center employee typing and checking, right two structured forms labelled 'ERP' and 'CRM'. Coral dashed gaps between systems, documents physically being manually transferred by employee, not automatic connected arrows. Large readable short caption INSIDE the image '답변은 AI가, 입력은 사람이'. Convey manual handoff bottleneck, not vague office mood. Clean high-impact thumbnail.

## AI에게 업무 창구를 열어주는 MCP

파일: illustration-mcp-tools.webp

대체 텍스트: AI 애플리케이션이 MCP를 통해 재고 조회와 견적 저장 도구를 사용하는 개념도

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Productivity-visual with charming miniature adult people and functional illustrations. Left AI application workstation labelled 'AI 애플리케이션'; center common service desk labelled 'MCP 서버'; right two clear illustrated service cards '재고 조회' with shelves, '견적 저장' with document tray. Clear request arrows left to center to both tools, small return line for results. Labels only specified. Depict logical software service not actual corporate reception. Don't put MCP directly inside a human brain.

## API가 있는데 MCP는 왜 또 필요할까?

파일: figure-mcp-api.webp

대체 텍스트: 영업과 고객지원 에이전트가 공통 MCP 서버를 거쳐 기존 ERP API를 사용하는 구조

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Infographic-diagram, clean minimal schematic with small illustrated warehouse motif. Two boxes at left vertically '영업 에이전트' and '고객지원 에이전트', both connect to middle 'MCP 서버', then right '기존 API', then far right 'ERP'. All forward connecting paths clearly visible without crossings. Lower short text '기존 기능을 공통 도구로 제공'. No before-after, no claims replacing APIs. Big type, few labels.

## 재고를 물어보면 내부에서는 무슨 일이 벌어질까?

파일: figure-tool-call.webp

대체 텍스트: 도구 목록 확인부터 재고 조회 결과 반환까지의 호출 과정

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Infographic-diagram with 4 large illustrated steps in row, arrows 1→2→3→4 and curved return arrow below 4 back to1 labelled '조회 결과'. Step1 'AI 애플리케이션' icon conversation, subline '도구 선택'. Step2 'MCP 요청' subline '상품 코드·창고'. Step3 'MCP 서버' subline '권한·입력 검사'. Step4 'ERP' subline '재고 조회'. Above small tool listing card attached to step1 'tools/list', step2 'tools/call'. Actual result comes ERP via server then app: route return arrow through beneath server before app. No magic AI direct DB write.

## 실제 기업에서는 어디까지 쓰고 있을까?

파일: illustration-shared-work.webp

대체 텍스트: 직원들이 연결된 자료를 조회하고 후속 업무를 시스템에 남기는 가상 장면

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Illustration-story. Two adult office coworkers, one looking up company source documents in dashboard, other reviewing newly created task card on a shared display. One large readable display split '자료 조회' and '업무 등록', corresponding document-search and checklist icons. Workstation with people in collaborative natural poses, light airy background. Generic hypothetical workplace inspired by reading and writing workflow, NOT a portrait of actual Block or Atlassian office. No logos, no metrics.

## 연결은 됐는데 여전히 못 쓴다면

파일: figure-inventory-context.webp

대체 텍스트: 재고 수량만 받은 경우와 상품·창고·단위·조회 시각을 함께 받은 경우 비교

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Infographic-diagram blended with warehouse illustration. Left small response card only '100' and puzzled person asking '개? 박스?'. Right larger structured result card exact labels '상품 P-210', '창고 A', '판매 가능 100개', '조회 시각 확인'. Rows separated clearly with matching box/shelf icons. An arrow left-to-right labelled '의미를 함께 전달'. No made-up timestamps, unit conversions, other quantities. Both cards illustrative examples not real API outputs.

## 입력까지 맡기려면 완료를 확인해야 합니다

파일: figure-confirm-save.webp

대체 텍스트: ERP 견적 저장 완료와 CRM 상담 기록 실패를 구분해 실패한 단계만 재처리하는 예시

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Infographic-diagram. Two parallel status cards linked to same task, top 'ERP 견적 저장' with green check '완료', bottom 'CRM 상담 기록' amber warning '미완료'. From bottom only a circular retry arrow to box '실패한 단계만 재처리'. Top completion has NO retry arrow. Adjacent small adult worker looking at status summary. Footer short exact line '실제 기록으로 완료 확인'. No fabricated IDs or counts. Clearly partial failure, not all restart.

## 연결한 도구를 누가 관리하는지도 확인해야 합니다

파일: illustration-security-boundary.webp

대체 텍스트: 외부 문서의 악성 지시와 권한 없는 데이터 접근을 실행 단계에서 차단하는 개념도

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Illustrative security explanatory visual, no hooded hacker or abstract padlock-only. Left envelope document labelled '외부 메일' contains coral highlighted line '다른 거래처 자료 전송' clearly malicious. It enters AI application small node labelled 'AI'. Middle a concrete policy checkpoint labelled '권한·발송 검사' where a coral attempted path is visibly stopped with red cross. Right protected filing cabinet 'CRM' and outward email icon '외부 발송', behind checkpoint. Bottom tiny line '허용 범위 밖 요청 차단'. Make checkpoint software control imposed by company, not MCP automatic inherent security promise. Warm clean editorial icons and adult operator supervising from below.

## 우리 회사에서는 무엇부터 연결하면 될까?

파일: illustration-workflow-pilot.webp

대체 텍스트: 현업 담당자와 엔지니어가 견적 등록 업무를 테스트 환경에서 검증하는 일러스트

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Illustration-story. Adult business operations woman and male engineer seated side-by-side looking at a large monitor labelled '테스트 환경'. Monitor shows only three big checklist lines '거래처 확인', '중복 저장 검사', '발송 승인 확인', each with empty or green checked checkbox. Desk has unlabeled sample invoice paper oriented toward people with no legible front-facing words. Both hands simple resting natural, no hand pointing across other body. Calm practical focused atmosphere, source sheet to test screen relation obvious.

## 나가며

파일: illustration-reusable-tools.webp

대체 텍스트: 현업의 판단 기준을 엔지니어와 함께 업무용 도구로 정리하는 일러스트

Wide landscape 16:9 editorial illustration for a Korean executive technology blog. Warm cream paper background, refined ink outlines with gouache flat shading, navy/teal/coral/ochre accents. Adult professional illustration, not chibi comic. Clear visual relationships, ample whitespace. Korean text only where exact labels specified; readable at 800px width. No random numbers, no extra titles, no company logos or invented performance data. Hands anatomically coherent; screens face users unless shown as a separate explanatory inset; no backward writing on papers. Illustration-story. Experienced operations professional and engineer standing in front of shared whiteboard. Board has 3 simple illustrated cards, '현업의 판단 기준' → '업무용 도구' → '검증·운영', under them small warehouse, customer record, verified document icons. People at opposite edges, hands down or simple one-hand marker natural. No handwritten body text beyond labels. Clear knowledge-to-implementation theme; no unrelated mood montage, no claims instant success.
