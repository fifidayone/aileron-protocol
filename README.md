<a id="readme-top"></a>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&color=0:F87171,100:FCD34D&height=220&section=header&text=Aileron%20Protocol&fontSize=70&fontAlignY=50&fontColor=FFF7ED" width="100%" alt="Aileron Protocol Banner" />
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&size=20&pause=1000&color=e2c08a&center=true&vCenter=true&width=700&lines=Precision+flight+control+for+AI+agents;Stop+wasting+quota+on+debug+loops;Reduce+unnecessary+context+reading;Zero+planning+overhead+for+simple+tasks" alt="Typing SVG" />
  </a>
</p>

<div align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/Language-English_🇺🇸-f4b393?style=for-the-badge&logo=translate&logoColor=black" alt="English"/></a>
  <a href="README.th.md"><img src="https://img.shields.io/badge/Language-ภาษาไทย_🇹🇭-e8c5c8?style=for-the-badge&logo=translate&logoColor=black" alt="Thai"/></a>
</div>

<br />

<div align="center">
  <img src="https://img.shields.io/badge/-Antigravity_2.0-c3b1e1?style=for-the-badge&logo=google&logoColor=black" alt="Antigravity 2.0" />
  <a href="LICENSE"><img src="https://img.shields.io/badge/-CC_BY--NC--SA_4.0-e2c08a?style=for-the-badge&logo=creative-commons&logoColor=black" alt="CC BY-NC-SA 4.0" /></a>
</div>

<br />

## Why Aileron?

Vibe coding with Antigravity is powerful, but the default harness gets in the way more than you'd expect. Agents over-read context, create elaborate plans for minor edits, and get stuck retrying the same failing fix until they burn your quota.

<br />

**Aileron Protocol** is a ready-made `GEMINI.md` for Antigravity 2.0. Drop it into a project or global config to keep the native capabilities while adding sharper boundaries for planning, debugging, tool cost, code changes, verification, and frontend work.

<br />

| Behavior         | Default Antigravity Experience                                        | With Aileron                                                                             |
| :--------------- | :-------------------------------------------------------------------- | :--------------------------------------------------------------------------------------- |
| **Planning**     | Routine work can expand into unnecessary plans and artifacts          | Skips ceremony for simple work; reserves formal planning for structural risk             |
| **Context**      | Agents may inspect broadly before narrowing the task                  | Starts from target files, nearby code, config, and repository conventions                |
| **Debugging**    | Repeated attempts can drift into speculative patching                 | Stops after 2 failed cycles on the same symptom and reports back                         |
| **Safety**       | Shared behavior can change before its impact is fully traced          | Identifies callers and compatibility impact before changing shared APIs                  |
| **Cost**         | Subagents and image generation can run when direct work is enough     | Requires cost-bearing tools to be explained and approved unless already requested        |
| **Verification** | Tested results and reasonable assumptions can blur together           | Keeps verified, inferred, and unchecked claims strictly separate                         |
| **Styling**      | Strong decorative defaults can produce repetitive AI-style interfaces | Prioritizes project design systems, structure, typography, spacing, and controlled color |

> [!NOTE]
> Aileron is fully compatible with all models on Antigravity 2.0. We recommend Gemini 3.5 Flash for the best balance of speed and reliability.

### Built to steer, not replace

Aileron does not replace Antigravity's System Harness, Tool Schemas, or Security Permissions. It applies strong local preferences where the harness leaves room for judgment, and yields cleanly when a system constraint takes precedence.

The result is not a less capable agent. It is an agent that spends more of its capability on the task that was actually requested.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Repository Structure

```text
aileron-protocol/
├── Aileron/
│   └── GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

## Installation

Install Aileron **globally** for all projects or **locally** for a specific workspace.

### Global Setup

Copy `Aileron/GEMINI.md` to your global configuration folder:

- **Windows:** `%USERPROFILE%\.gemini\GEMINI.md`
- **macOS / Linux:** `~/.gemini/GEMINI.md`

### Workspace Setup

Install Aileron for a specific project using either method:

- **Method A (Project Root):** Copy the protocol to the project root and keep the filename `GEMINI.md`.
- **Method B (Rules Directory):** Save under `.agents/rules/` and change the filename as desired (e.g. `aileron.md`).

> [!IMPORTANT]
> Files stored under `.agents/rules/` must include the following trigger header at the very top. Leave one blank line after the closing `---`.
>
> ```markdown
> ---
> trigger: always_on
> ---
>
> [Rules start here...]
> ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

This project is distributed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License**. See [LICENSE](LICENSE) for details.