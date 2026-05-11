# AGENTS.md

This file provides guidance to Codex (Codex.ai/code) when working with code in this repository.

## Repository Purpose

This is a **monorepo of AI agents**. Each top-level directory is an independent agent for a different task. Today there is one (`agent_roteirista`), but more will be added over time. There is no shared build, lint, or test pipeline — agents are self-contained and the artifacts are mostly Markdown definitions (Agent Skills spec) plus any helper scripts each agent needs.

## Layout

- `<agent_name>/` — one directory per agent at the repo root. Treat each as its own project; don't cross-link skills, workflows, or scripts between agents unless the user asks for it.
- `.Codex/settings.local.json` — repo-wide Codex permissions (shared across agents).

When the user asks to work on an agent, scope your edits and exploration to that agent's directory.

## Adding a new agent

Default to the [Agent Skills](https://agentskills.io/specification) layout used by `agent_roteirista`:

```
<new_agent>/.agent/
  workflows/<workflow>.md   # entry point describing the pipeline
  skills/<skill_name>/SKILL.md   # one directory per skill, with YAML frontmatter (name, description)
  spec/                     # optional pointers to specs
```

Only deviate from this layout if the agent has fundamentally different needs (e.g., it's a runnable service rather than a skill-based agent). In that case, document the layout in the agent's own README or `AGENTS.md`.

## Existing agents

### `agent_roteirista` — YouTube scriptwriter

Workflow `agent_roteirista/.agent/workflows/roteirista-youtube.md` orchestrates a 10-step pipeline (theme → web research → synthesis → script → references → scientific validation → titles/thumbnails/description → short-form derivation → teleprompter formatting → PDF export). The tone directives at the top of the workflow (70% narrative / 30% science, "bar conversation" register, no production markings like `[B-ROLL]`) are load-bearing.

Skills under `agent_roteirista/.agent/skills/`:
- `cacador_de_retencao` — retention techniques (Open Loops, Re-hooks).
- `validador_cientifico` — tags claims as `[FATO VERIFICADO]` / `[FATO PARCIAL / NECESSITA CUIDADO]` / `[MITO / REMOVER]`.
- `metadados_youtube` — 5 titles, 2 thumbnail directions per title, description with 3 hashtags.
- `derivacao_de_conteudo` — 3 short-form scripts (TikTok/Reels/Shorts) via "Gold Nuggets".
- `formatador_de_roteiro` — teleprompter spacing/legibility.
- `gerador_de_teleprompter`, `pdf`, `docx`, `skill-creator` — utilities (export, skill authoring/eval).

Final deliverable: PDF with two sections in this exact order — `# [Roteiro Longo]` (script + references + validation + metadata) and `# [Shorts]` (3 short-form scripts).

Conventions specific to this agent:
- Content is in **Portuguese (pt-BR)** — preserve language and register.
- Do **not** add production markings (`[B-ROLL]`, cuts, visual cues, dramatic pauses) to scripts.
- Cap statistics at 2–3 per long-form script.
- References must include exact source URLs for any cited statistic, study, or chart.

## Permissions

`.Codex/settings.local.json` pre-allows `WebSearch` and `python3` invocations (markdown, weasyprint, reportlab, fpdf, headless Chrome PDF printing) currently used by `agent_roteirista`'s `pdf` skill. New agents that need additional commands should extend this file.
