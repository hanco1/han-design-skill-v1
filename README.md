# Han Design Skill v1

`han-design-skill-v1` is a personal Codex skill for creating Han-first editorial social card systems, Rednote/Xiaohongshu carousel images, WeChat Official Account cover pairs, README visuals, dashboard mockups, and warm-beige serif editorial UI visuals.

The skill is adapted from the user's optimized `guizang-social-card-skill` and uses a Guizang-inspired editorial / Swiss visual system as its source lineage. This repository adds the Han warm-beige serif house style, refined social-card workflow rules, templates, references, and validation tooling.

## What It Produces

- Rednote/Xiaohongshu 3:4 social card sets.
- WeChat Official Account `21:9` + `1:1` cover pairs.
- Article covers, product-note cards, tutorial cards, and screenshot-heavy editorial posts.
- Han-style warm-beige serif visuals for frontend/editorial design prompts.
- Editorial dashboard and README presentation visuals where Han's house style should override generic SaaS dashboard defaults.

## Install As A Codex Skill

Clone this repository, then copy the repo folder into your personal Codex skills directory:

```powershell
git clone https://github.com/hanco1/han-design-skill-v1.git
Copy-Item -Recurse -Force '.\han-design-skill-v1' "$env:USERPROFILE\.codex\skills\han-design-skill-v1"
```

Install dependencies and validate:

```powershell
cd "$env:USERPROFILE\.codex\skills\han-design-skill-v1"
npm install
$env:PYTHONUTF8 = '1'
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" .
```

Expected validation output:

```text
Skill is valid!
```

Open a new Codex session after installation so the skill list can be rediscovered.

## Usage

Example prompt:

```text
Use $han-design-skill-v1 with Han's warm-beige serif house style to turn this article into a 3:4 social card image set and a paired WeChat 21:9 + 1:1 cover.
```

For interface work, ask for the Han style explicitly:

```text
Use $han-design-skill-v1. Treat Han's warm-beige serif house style as the primary design authority and design a frontend dashboard mockup for this repo.
```

## Skill Structure

```text
han-design-skill-v1/
|-- SKILL.md
|-- agents/
|-- assets/
|   |-- template-editorial-card.html
|   |-- template-swiss-card.html
|   |-- magazine-bg-webgl.js
|   `-- screenshot-backgrounds/
|-- references/
|-- validate-social-deck.mjs
|-- package.json
|-- package-lock.json
|-- LICENSE
|-- NOTICE.md
`-- README.md
```

## Source Lineage

This repository is a modified personal skill derived from the user's optimized copy of `guizang-social-card-skill`. Its design language is inspired by the Guizang PPT style system and the original Guizang social-card workflow, then adapted into Han's own warm-beige serif house style and publication workflow.

No upstream repository URL was present in the local source folder used for this publication. See `NOTICE.md` for attribution details.

## License

This project preserves the upstream AGPL license and is distributed under `AGPL-3.0-or-later`. See `LICENSE`.
