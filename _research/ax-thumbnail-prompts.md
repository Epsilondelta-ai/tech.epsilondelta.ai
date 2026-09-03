# 썸네일 이미지 프롬프트 (gpt-image-2)

포스트: AX와 암묵지 자산화 (geoff-4-ax-tacit-knowledge)

## 가이드 요약 (OpenAI Cookbook 기준)

- 순서: **배경/장면 → 주체 → 핵심 디테일 → 제약조건**. 긴 문단 대신 짧은 라벨 세그먼트로.
- 매체·재질·질감·시점·조명을 구체적으로. 사진이면 "photorealistic" 명시.
- 이미지 안 텍스트는 **따옴표 또는 ALL CAPS**로 감싸고, 폰트·크기·색·위치를 제약조건으로 명시. 텍스트가 있으면 `quality="high"`.
- 처음엔 깔끔한 기본 프롬프트로 시작하고, 한 번에 한 가지씩만 바꿔가며 수정("change only X, keep everything else the same").
- 불변 조건은 매번 반복 명시: "no watermark", "no logos" 등.
- 권장 사이즈: 1024×1024 / 1536×1024 / 1024×1536. 양변 16의 배수, 장단비 3:1 이내. 블로그 썸네일은 **1536×1024**(3:2) 또는 **1792×1008**(16:9 근사) 권장.
- 주의: 한글 텍스트 렌더링은 영문보다 불안정. 텍스트 없이 생성한 뒤 한글은 후편집으로 얹는 것이 안전. 텍스트를 넣을 경우 짧게(4~6자), quality high, 여러 장 생성해 고르기.

API 파라미터 예시: `model="gpt-image-2"`, `size="1536x1024"`, `quality="high"`, `n=3`

---

## 프롬프트 A (추천) — 빈 의자와 에이전트

```
Use case: editorial thumbnail for a Korean tech blog post about capturing senior employees' tacit knowledge into AI agents.

Scene: a quiet corporate office desk at a Korean bank or investment firm, late evening, cool blue-grey ambient light with one warm desk lamp. Photorealistic, shot like a 35mm documentary photograph, eye-level, shallow depth of field.

Subject: an empty ergonomic office chair pushed slightly back from the desk, as if someone left for good. On the desk, a personal mug, a stack of dog-eared credit review files, and reading glasses folded on top.

Key details: the desk monitor is on and shows a clean dark-mode interface — a list of short decision rules with checkboxes, some already checked, one being typed with a blinking cursor. Rules are rendered as abstract text lines, not legible words. A small, friendly abstract AI-agent indicator (a soft glowing geometric shape, not a robot, not a humanoid) sits at the corner of the screen.

Mood: honest, slightly melancholic but hopeful. Real skin-of-the-office texture: worn desk edge, cable clutter, fingerprints on the monitor.

Constraints: no people, no faces, no humanoid robots, no legible text anywhere in the image, no company logos, no watermark. Wide 3:2 composition with the chair on the left third and the monitor on the right third, leaving calm negative space at the top for a title overlay later.
```

후편집용 한글 카피 후보: "내규에는 없는 것" / "그 사람이 나가면 판단도 나간다"

---

## 프롬프트 B — 머릿속에서 빠져나오는 판단 기준 (개념형)

```
Use case: editorial illustration thumbnail for a tech blog post on turning tacit knowledge into AI agent rules.

Scene: flat, minimal editorial illustration on a solid off-white background. Limited palette: charcoal, one deep navy, one accent of warm amber. Clean vector-like shapes, strong silhouette, generous negative space. No gradients, no 3D.

Subject: side profile silhouette of a middle-aged professional in a suit, facing right, occupying the left half of the frame.

Key details: from the back of the head, instead of data streams or circuit lines, a loose trail of small paper cards drifts to the right. Each card is a tiny abstract rule: a checkbox, a short bar of text, an arrow, an "if/then" fork shape. The cards land in neat stacked rows inside a simple rounded rectangle on the right — a plain terminal-like panel, with one card still mid-air. The panel has a small amber cursor block.

Mood: calm, precise, editorial — like a business magazine feature, not a sci-fi poster.

Constraints: no legible words, no glowing brains, no circuit patterns, no binary digits, no robots, no logos, no watermark. 3:2 composition. Keep the top 20% of the frame empty for a title overlay.
```

---

## 프롬프트 C — 인터뷰 장면 (방법론 강조)

```
Use case: thumbnail for a tech blog post explaining how an AI agent interviews a senior expert to extract decision criteria.

Scene: a small meeting room in a Korean office, daytime, soft diffuse window light from the left. Photorealistic, natural documentary style, eye-level, medium shot.

Subject: a senior Korean professional in her 50s, sleeves rolled up, sitting at a table and gesturing mid-explanation, seen in three-quarter view from behind and to the side so her face is mostly turned away. Across the table, no person — instead a laptop open toward her.

Key details: the laptop screen shows a simple chat interface. On the left side of the screen, a speech bubble; on the right side, a growing structured checklist being filled in, with a few items already checked. All on-screen text is rendered as abstract lines, not readable words. A notepad with hand-drawn arrows and a coffee cup on the table.

Mood: attentive, respectful, ordinary workday. Real textures: paper grain, laminate table, slight lens softness.

Constraints: no readable text, no robots or humanoid figures, no holograms, no logos, no watermark. 3:2 composition with the laptop screen in the right third and the person in the left two-thirds; keep the upper area uncluttered for a title overlay.
```

---

## 수정 반복 시 문구 예

- "Change only the monitor content to show three stacked cards instead of a list; keep everything else the same."
- "Make the lighting slightly warmer; keep composition, objects, and framing identical."
- 텍스트를 넣고 싶을 때: `Add the Korean text "내규에는 없는 것" in a clean bold sans-serif, white, centered in the top negative space, about 8% of image height. Change nothing else.` (quality high, 3~4장 생성 후 선택)

## 출처

- [OpenAI Cookbook – GPT Image Generation Models Prompting Guide](https://developers.openai.com/cookbook/examples/multimodal/image-gen-models-prompting-guide)
- [i-SCOOP – Prompting gpt-image-2 like a pro](https://www.i-scoop.eu/prompting-gpt-image-2-like-a-pro-guide/)
