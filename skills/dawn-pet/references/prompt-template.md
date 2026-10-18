# Dawn Pet 提示词模板

## 主模板

```text
Use case: illustration-story
Asset type: {avatar / pose sheet / 16:9 editorial scene / flow diagram}
Input images:
- Image 1 is the exact Dawn Pet identity AND style anchor. Preserve this same
  gray-and-cream miniature schnauzer in every pose. Other images only supply
  pose, prop or composition references.
Primary request: Show Dawn Pet {action}.
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

## 动作示例

- 坐姿歪头：`Sitting naturally, gently tilting its head, all paws readable.`
- 打招呼：`Sitting on its haunches and lifting one short front paw.`
- 搬箱子：`Seated on its haunches, hugging one oversized box with both front paws; the box tilts slightly as if slipping. Keep paws canine, not hands.`
- 推文件：`On all four paws, leaning forward to push a large folder with its nose.`

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
