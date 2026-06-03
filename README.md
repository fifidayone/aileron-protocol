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

**Aileron Protocol** is a ready-made `GEMINI.md` you drop into your project or global config. It enforces strict boundaries on how your agent plans, debugs, reads files, and writes code.

<br />

| Behavior | Default Harness | With Aileron |
| :--- | :--- | :--- |
| **Planning** | Plans minor edits, creating unnecessary planning overhead | Skips planning on simple edits; plans only for structural risk |
| **Context** | Scans broad directories, bloating context windows | Inspects target files first before searching |
| **Debugging** | Retries failed fixes blindly until timeout | Stops after 2 failed cycles for human feedback |
| **Safety** | Edits shared files speculatively, risking breakages | Checks caller files before editing shared APIs |
| **Styling** | Spams generic gradients and saturated glassmorphism | Blocks decorative styling; enforces minimal color strategies |

> [!NOTE]
> Aileron is fully compatible with all models on Antigravity 2.0. We recommend Gemini 3.5 Flash for the best balance of speed and reliability.

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

You can install Aileron **globally** for all projects or **locally** for a specific workspace.

### Global Setup

Copy `GEMINI.md` to your global configuration folder.
* **Windows:** `%USERPROFILE%\.gemini\GEMINI.md`
* **macOS / Linux:** `~/.gemini/GEMINI.md`

### Workspace Setup

Place `GEMINI.md` inside your active project directory. You have two options.
* **Option A:** Copy the file directly to the root of your project.
* **Option B:** Save the file in a custom directory like `.agents/rules/project-rules.md`.

> [!IMPORTANT]
> If you choose Option B, you must add the following trigger header to the very top of the file. Ensure there is a blank line after the closing `---`.
> ```markdown
> ---
> trigger: always_on
> ---
>
> [Rules start here...]
> ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

This project is distributed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License**. Please see [LICENSE](LICENSE) for more details.
