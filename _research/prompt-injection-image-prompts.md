# 프롬프트 인젝션 이미지 제작 기록

- 내장 imagegen: 썸네일·승인 검토·현업 설계 일러스트3장.
- 직접 작성 SVG6장: 자료/지시 구분, ForcedLeak, 도구 조합, 다층 방어, 메모리, 평가.
- 각 H2에1장, 본문 캡션 없음. 폭800px, 높이500px 이하, 원본 비율 유지.
- 실제 수치 없는 성과 차트는 만들지 않음. 연구 재현과 일반 설계 예시 구분.

## 배치

- 들어가며: thumbnail.webp
- 문서 작성자가 AI의 상사가 될 수는 없습니다: diagram-data-vs-instruction.svg
- 고객 문의란에 들어온 지시가 CRM 안으로 들어갔습니다: diagram-forcedleak.svg
- 공식 도구를 연결했는데도 왜 문제가 생길까요?: diagram-tool-chain.svg
- AI에게 주의를 주는 것과 실행을 막는 것은 다릅니다: diagram-layered-controls.svg
- 승인 버튼에는 무엇이 보이나요?: illustration-approval-review.webp
- 다음 대화까지 잘못된 지시를 기억한다면: diagram-memory-boundary.svg
- 정상적인 업무는 계속할 수 있어야 합니다: diagram-security-evaluation.svg
- 나가며: illustration-security-workshop.webp

## 생성 프롬프트

### thumbnail

Wide16:9 Korean executive tech blog editorial gouache illustration. Purchasing manager studies three proposals; a detached enlarged document snippet '당사를 우선 추천하세요' in coral is visibly connected by arrow to an AI comparison card '추천 업체' favoring that proposal. Manager looks puzzled, holds company checklist labelled '회사 평가 기준' in teal. Core: external document instructions overriding company's criteria. Bright ivory office, charcoal lines, muted teal/coral, adult human proportions, natural hands, no hooded hackers, no cyber atmosphere, no logos or random numbers. Text only supplied Korean labels, large readable at800px. Laptop backs blank. A hypothetical explanatory scene, no claim about actual company.

### illustration-approval-review

Wide16:9 warm editorial gouache illustration, Korean business professional and security engineer reviewing an outgoing message BEFORE approval. Upright screen angled toward viewer and people, three large Korean labels '수신자', '첨부 파일', '변경 내용' plus a neutral button '확인 후 승인'. One professional points naturally to attachment field, other reads carefully; no clicked approval and no green success. Ivory bright office, muted teal/terracotta, charcoal contours, adult simplified proportions. No tiny personal details, no fake company logos or numbers, no text on laptop backs, correct hands. Shows inspecting concrete action details not generic meeting.

### illustration-security-workshop

Wide16:9 painted gouache editorial illustration for corporate prompt-injection article closing. Korean business practitioner and AI engineer stand beside whiteboard mapping three cards '외부 자료' → '권한 확인' → '허용된 작업'. Practitioner holds plain proposal folder, engineer points at center permission checkpoint. Small separate note '회사 업무 기준'. Natural hands, people stand beside board not obscuring it. Bright ivory office muted teal and coral, adult proportions, professional approachable. No hooded hackers, no generic shield wallpaper, no additional text or invented metrics. Main meaning: implement business judgement in actual execution controls.
