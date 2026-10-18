# Dawn Pet 提示词模板

## 数量与选题

遵守 SKILL.md 的“场景与数量”：未指定数量时基础三张，关键流程在其上额外配图；重大里程碑、重要事件与强调内容按独立表达价值追加。先列总数、每张用途及“基础/追加”来源，再为每张图片分别填写下方模板。用户指定总数时在其数量内覆盖重点；不要将三张独立图片压成一张三联画。

## 主模板

```text
Use case: illustration-story
Asset type: {avatar / pose sheet / 16:9 editorial scene / flow diagram}
Input images:
- Image 1 is the exact Dawn Pet identity AND style anchor. Preserve this same
  gray-and-cream miniature schnauzer in every pose. Other images only supply
  pose, prop or composition references ONLY when explicitly needed.
- Image 1 fixes appearance and drawing style, not its sitting pose, raised paw,
  gaze, camera angle or centered composition. Create the new scene below from
  scratch. Do not copy a previous scene's book, prop or arrangement.
Meaning to communicate: {specific relationship or event from the user content}.
Primary request: Show Dawn Pet {concrete physical action serving that meaning}.
Body pose: {canine posture and weight/contact with the prop}.
Camera/view: {front / side / three-quarter / overhead, chosen for the action}.
Spatial composition: {dog and prop placement, direction and relative scale}.
Character invariants:
- Compact puppy body, large recognizable schnauzer head, two folded triangular
  ears, short sturdy legs, rounded dog paws, short upturned tail.
- Gray crown, ears and back; cream eyebrows, cheeks, beard, chest and paws,
  matching the anchor's coat patches.
- Two warm brown eyes with black pupils and small highlights, black nose,
  small natural mouth. Keep distinctive cream eyebrows and fluffy beard.
- Muted sage-green collar with a small brass buckle in every pose.
Personality: attentive, friendly, curious, earnest and slightly clumsy.
Style: simplified hand-drawn editorial illustration, slightly wobbly black
contours, gray and cream color blocks, sparse short fur strokes. Match Image 1.
Composition: {layout}; generous whitespace. One main prop per scene, drawn
with sparse thin black lines and white interior. Pure white background.
Constraints: no breed change, no human hands, fingers, long arms, clothing,
extra accessories, old black blob body, white dot eyes or orange belly mark.
No photorealistic fur, 3D, glossy vector rendering, gradient, busy background,
text, border or watermark. Dog remains a dog even when using its front paws.
```

## 场景推导与差异

先根据内容设计，以下只是推导示例，不是每次轮换的固定素材库：

| 内容含义 | 动作与构图示例 |
|---|---|
| 将成果交到下一环节 | 四足侧身行走，嘴叼文件袋，向画面右侧移动 |
| 发现隐藏的问题 | 三分之四俯视，前腿弯曲、鼻子靠近打开的盒子 |
| 推动困难任务 | 侧视，四足撑地向前倾，用鼻子推过大的文件夹 |
| 等待响应 | 趴在沙漏旁，下巴靠前爪，低视角、宽留白 |
| 在候选方向间选择 | 背面三分之四视角，站在岔路前回头观察 |

书只在具体内容需要阅读行为或用户点名时使用，不能作为所有知识类主题的通用道具。多张独立图分别填写主模板；保持同一角色，但在语义允许时至少改变动作、身体姿态、视角、空间关系中的两项。不要仅更换书中符号。

## 流程图解模板

在主模板后追加，保留全部 Character invariants 和 Constraints：

```text
Draw a {N}-node {linear / loop / branch} process illustration. Every node shows
this SAME schnauzer doing one physical action. Use generous whitespace and
sparse thin black arrows, clear direction, no crossings.
Nodes:
{label: action with one thin-line prop, repeated for each node}
Place one short handwritten black label directly UNDER each node, outside the
dog and prop. No other text, title, legend, border or numbered circles.
Keep coat patches, ears, eyebrows, beard, eye color, collar and proportions
identical at every node. No human hands or humanoid standing posture.
```

## 局部迭代

- `Keep everything else unchanged. Restore the anchor's folded ears, cream eyebrows and beard, brown eyes and sage-green collar.`
- `Keep the pose and layout unchanged. Simplify fur details to sparse short strokes and flat gray/cream color blocks.`
- `Keep the character unchanged. Replace human-like fingers with short rounded dog paws.`
- `Keep every node unchanged except node 3. Move its label below the prop and fix the arrow direction.`
