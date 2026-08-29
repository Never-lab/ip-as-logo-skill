# CLAUDE.md — IP as Logo

Agent Skill repo for extremely simple, cute, rounded IP mascot images. Fork/source: `Never-lab/ip-as-logo-skill`. Upstream format: open Agent Skills (`SKILL.md` at repo root).

Read [`README.md`](./README.md) and [`SKILL.md`](./SKILL.md) before changing skill behavior.

## Shared agent block (Never-lab)

- Chat: Italian. Code/PR/issue/skill prose that ships: English (match existing `SKILL.md` voice).
- Before posting PR bodies or issue comments: skill **`no-ai-slop`**.
- Never `Co-authored-by: Cursor`.
- Prefer `ponytail` + Karpathy; no default `docs/superpowers/specs|plans` MD — decisions in chat/claude-mem.

## This repo

- Canonical skill instructions: root [`SKILL.md`](./SKILL.md). Cursor project copy: `.cursor/skills/ip-as-logo/` (keep in sync with root when editing the skill).
- Showcase asset: `assets/ip-as-logo-wall.webp`. Generated outputs stay out of git (`generated_images/`, `results/`, `*.png` except `assets/`).
- Do not invent SVG fallbacks for the AI skill when image models are missing.
- Optional companion: [`generator/`](./generator/) — deterministic SVG (`renderAvatar`) for game assets / avatars when the user asks for it explicitly. Credit: otatechie/mascot-avatars (MIT). Keep `NOTICE` when copying.
- Skill edits: keep workflow, complexity budget, and prompt skeleton consistent; do not soften constraints without an explicit request.

## When generating IP images

Invoke skill **`ip-as-logo`** (read `.cursor/skills/ip-as-logo/SKILL.md` or root `SKILL.md`) and follow it exactly: three directions → six candidates after approval → one-pass deliver, no auto-retry filters.
