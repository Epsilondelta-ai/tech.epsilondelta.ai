# Thumbnail design record — Five scopes of agent engineering

- 작성일: 2026-09-04
- 최종 제작 방식: 정확한 제목과 용어를 보장하기 위해 SVG로 직접 제작한 뒤 `rsvg-convert`로 PNG 렌더링
- 최종 파일: `content/posts/geoff-5-five-scopes-of-agent-engineering/thumbnail-v2.png`
- 편집 원본: `content/posts/geoff-5-five-scopes-of-agent-engineering/thumbnail-v2.svg`
- 비고: 생성형 이미지 시안은 글의 주제가 바로 드러나지 않아 사용하지 않음

## Final design spec

```text
Use case: infographic-diagram
Asset type: 3:2 landscape technology blog thumbnail
Audience: 기술에 관심은 있지만 깊은 이해가 없는 경영진
Primary request: Prompt, Context, Loop, Graph, Harness가 AI 모델을 움직이는 서로 다른 다섯 통제 범위라는 점을 한눈에 보여준다.
Composition: 왼쪽에는 글 제목과 독자가 얻을 답, 오른쪽에는 중앙 AI MODEL과 방사형으로 연결된 다섯 개의 큰 카드.
Text (verbatim): "프롬프트만 잘 쓰면 끝인 줄 알았다", "PROMPT", "CONTEXT", "LOOP", "GRAPH", "HARNESS".
Style: 밝은 아이보리 배경, 에디토리얼 인포그래픽, 큰 글자, 작은 카드에서도 읽히는 대비.
Color palette: graphite, emerald, cobalt, muted coral, amber, purple.
Constraints: 다섯 개념을 선형 성숙도나 포함 관계로 오해하게 하지 말 것. 중앙 모델과 각 범위를 동등하게 연결할 것. 정확한 텍스트, no watermark.
```

## Discarded image-generation prompt

```text
Edit/reimagine the previously generated blog thumbnail while preserving only its core idea: a central AI model surrounded by five distinct engineered scopes. Remove the dark office, night skyline, desk lamp, pens, notebook, and all moody black scenery.

Use case: stylized-concept
Asset type: 3:2 landscape technology blog thumbnail / header image
Primary request: turn the concept into a bright, clean, optimistic editorial still life for nontechnical business leaders.
Scene/backdrop: seamless warm off-white studio background with a faint paper texture and soft daylight.
Subject: a simplified elegant kinetic sculpture. One small luminous faceted core in the center; around it exactly five visually distinct layers: a precise instruction frame, a few translucent context cards, a circular feedback track, a sparse branching node network, and a protective outer supporting frame. Make the hierarchy easy to read at thumbnail size.
Style/medium: premium contemporary editorial 3D illustration, tactile paper, frosted glass, matte ceramic, and anodized metal; clean rather than futuristic.
Composition/framing: wide 3:2 composition, centered object, generous breathing room, strong silhouette, slightly elevated three-quarter view.
Lighting/mood: soft natural daylight, subtle grounded shadows, calm and intelligent.
Color palette: warm ivory, graphite, emerald green, cobalt blue, muted coral, and a small amber accent.
Constraints: exactly five surrounding structures; no words, letters, numbers, labels, logos, trademarks, people, faces, robots, brains, watermark, or dark office background.
Avoid: neon cyberpunk, black-dominant palette, tangled cables, dense circuitry, glossy sci-fi control panels, generic stock AI imagery.
```
