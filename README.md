# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity 2.0" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Gemini Agent" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="MIT License" /></a>

</div>

> **Aileron Protocol** is a set of drop-in `GEMINI.md` baselines for Antigravity 2.0.
> It reduces harness ceremony, sharpens tool/verification thresholds, and gives the agent clearer behavior for different kinds of work.

[อ่านภาษาไทย](README.th.md)

---

## Why This Exists

Antigravity's default harness is broad. That is useful for generality, but it can also make an agent over-plan, over-read, over-call tools, chase generic UI effects, generate unnecessary artifacts, or keep debugging without new evidence.

Aileron adds a tighter baseline on top of the harness. It does not replace project rules. It gives you a global foundation that can still be overridden by workspace-specific `GEMINI.md` or `.agents/rules` files.

---

## Profiles

Each profile is standalone. Copy exactly one profile file and use it as your active `GEMINI.md`.

| Profile | Bias | UI Default | Verification | Best For |
| :--- | :--- | :--- | :--- | :--- |
| **Lite** | Fastest path, least ceremony | Production-acceptable, restrained product UI | Cheapest useful check | Small fixes, clear edits, fast iteration |
| **Balanced** | Daily-driver behavior | Polished minimal product UI | Real checks when they matter | Routine development, medium tasks |
| **Studio** | Strong UI/render/design control | Premium visible result, render-first mindset | Render checks for meaningful UI | Frontend, landing pages, visual polish |
| **Architect** | Risk-aware engineering | Functional product UI; aesthetic work still allowed | Broader checks for shared behavior | Refactors, contracts, migrations, systems work |
| **Ultimate** | Strongest all-around guardrails | Premium UI when UI is involved | Strongest evidence discipline | High-risk, critical, or ambiguous work |

The profiles may look similar structurally because they are standalone files. The difference is in threshold and pressure: Lite lets the agent move faster with fewer gates; Ultimate closes more of the default harness escape routes.

---

## Quick Selector

- Use **Lite** when the task is clear and speed matters more than exhaustive checking.
- Use **Balanced** as the normal global baseline.
- Use **Studio** when the visible UI is the product.
- Use **Architect** when shared behavior, schemas, APIs, migrations, or long-term maintainability matter most.
- Use **Ultimate** when correctness, UI quality, and risk control all matter more than speed.

---

## What It Overrides

Aileron is tuned to reduce common Antigravity harness side effects:

- planning/artifact ceremony for routine work
- unnecessary slash-command or subagent suggestions
- broad context scans and old transcript reads
- repeated debugging loops without new evidence
- default vanilla-CSS bias when a project already has a styling system
- generic "WOW" UI effects, excessive gradients/glass, and generated-asset drift
- broken placeholder image paths
- SEO/meta/id churn on every UI by default
- claims of verification without current evidence

---

## Repository Structure

```text
aileron-protocol/
├── Aileron/
│   ├── lite/GEMINI.md
│   ├── balanced/GEMINI.md
│   ├── studio/GEMINI.md
│   ├── architect/GEMINI.md
│   └── ultimate/GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

---

## Installation

### Global Baseline

Copy one profile file, then save it as your global Gemini rules file:

```text
Aileron/<profile>/GEMINI.md -> ~/.gemini/GEMINI.md
```

Windows:

```text
%USERPROFILE%\.gemini\GEMINI.md
```

macOS / Linux:

```text
~/.gemini/GEMINI.md
```

### Workspace Override

For a specific project, place a project-specific rules file in the workspace. Workspace rules should override the global baseline.

Root-level option:

```text
your-project/
├── GEMINI.md
├── src/
└── package.json
```

`.agents/rules` option:

```text
your-project/
├── .agents/
│   └── rules/
│       └── project-rules.md
├── src/
└── package.json
```

If using `.agents/rules`, add this frontmatter at the top:

```markdown
---
trigger: always_on
---

[rules start here]
```

Keep the blank line after the closing `---`.

---

## License

MIT. See [LICENSE](LICENSE).
