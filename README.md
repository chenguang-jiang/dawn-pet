# dawn-pet

A Codex skill for consistent hand-drawn illustrations of **Dawn Pet**, DawnVibe’s gray-and-cream schnauzer. Create avatars, pose sheets, editorial scenes and illustrated process summaries from one identity anchor.

[简体中文](./README.zh-CN.md) · [MIT](./LICENSE)

<p align="center">
  <img src="./skills/dawn-pet/assets/identity/dawn-pet-anchor.png" width="360" alt="Dawn Pet: gray-and-cream schnauzer with folded ears, cream eyebrows and beard, brown eyes and a green collar, lifting one paw">
</p>

The default style uses simplified ink contours, gray and cream color blocks, sparse fur strokes and a white background. Folded ears, cream eyebrows and beard, brown eyes and a sage-green collar with a brass buckle stay consistent across poses.

## Install

The GitHub repository and skill are both named **`dawn-pet`**.

```bash
npx skills add chenguang-jiang/dawn-pet --skill dawn-pet
```

For a local Codex install from a clone:

```bash
git clone https://github.com/chenguang-jiang/dawn-pet.git
mkdir -p ~/.codex/skills
ln -s "$PWD/dawn-pet/skills/dawn-pet" ~/.codex/skills/dawn-pet
```

If migrating from `jcg-documentation-pet`, remove that old installation entry after installing `dawn-pet` so both versions are not discovered. The updated skill will be available on the next turn.

## Use

```text
Use $dawn-pet to draw a 16:9 white-background illustration of the schnauzer
seriously trying to hold a box that is slightly too big. Keep the box in
sparse black outlines and preserve the reference dog's identity.
```

<p align="center">
  <img src="./assets/readme/carrying-box.png" width="720" alt="Dawn Pet sitting on its haunches and trying to hold a large tilted box drawn in thin black lines">
</p>

The box illustration is a scene example. The paw-raising image is the **sole identity and default style anchor**; future scenes use its simpler rendering.

## What the skill does

| Request | Output |
|---|---|
| Avatar or hero | One recognizable dog on white |
| Pose sheet | Up to three separated poses of the same dog |
| Editorial scene | One action and one main prop, default 16:9 |
| Process or state summary | Usually 3–5 actions linked by thin arrows, with short labels underneath |
| Partial edit | Change the requested part while preserving the rest |

The anchor fixes appearance and drawing style; actions, props, camera views and layouts follow each request. Multiple independent images are generated as separate files, with meaningful scene differences rather than changes to symbols inside the same book.

The skill reads the anchor and identity rules, chooses an asset type from the request, builds an ImageGen prompt and checks the result. It uses built-in ImageGen; it does not install or train a model. Exact figures, fields, code and complex or concurrent flows belong in mermaid; the dog illustration can supply a short visual summary.

## Files and checks

The skill lives in [skills/dawn-pet](./skills/dawn-pet/SKILL.md). Identity, visual style, prompt templates, flow actions and QA guidance are in its `references/` directory. The bundled PNG anchor is required for each generation.

From the repository root:

```bash
python3 skills/dawn-pet/tests/test_skill_contract.py
```

[Changelog](./CHANGELOG.md) · [License](./LICENSE)
