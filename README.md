<a id="readme-top"></a>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:121826,100:2B3A54&height=220&section=header&text=Aileron%20Protocol&fontSize=70&fontAlignY=35&fontColor=F0EEEE" width="100%" alt="Aileron Protocol Banner" />
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&size=20&pause=1000&color=94E2D5&center=true&vCenter=true&width=700&lines=Precision+flight+control+for+AI+agents;Minimize+wasteful+token+usage;Complete+small+tasks+in+a+flash;Execute+large+tasks+with+razor-sharp+precision" alt="Typing SVG" />
  </a>
</p>

<div align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/Language-English_🇺🇸-89dceb?style=for-the-badge&logo=translate&logoColor=black" alt="English"/></a>
  <a href="README.th.md"><img src="https://img.shields.io/badge/Language-ภาษาไทย_🇹🇭-f2cdcd?style=for-the-badge&logo=translate&logoColor=black" alt="Thai"/></a>
</div>

<br />

<div align="center">
  <img src="https://img.shields.io/badge/-Antigravity_2.0-cba6f7?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity 2.0" />
  <a href="LICENSE"><img src="https://img.shields.io/badge/-CC_BY--NC--SA_4.0-f5c2e7?style=for-the-badge&logo=creative-commons&logoColor=white" alt="CC BY-NC-SA 4.0" /></a>
</div>

<br />

---

<table align="center" width="100%">
  <tr>
    <td width="20%" align="center" nowrap>
      <a href="#-why-aileron">
        <strong>🚀 Why Aileron</strong>
      </a>
    </td>
    <td width="20%" align="center" nowrap>
      <a href="#-task-optimized-profiles">
        <strong>⚡ Profiles</strong>
      </a>
    </td>
    <td width="20%" align="center" nowrap>
      <a href="#-repository-structure">
        <strong>📂 Structure</strong>
      </a>
    </td>
    <td width="20%" align="center" nowrap>
      <a href="#%EF%B8%8F-installation--setup">
        <strong>🛠️ Installation</strong>
      </a>
    </td>
    <td width="20%" align="center" nowrap>
      <a href="#-license">
        <strong>📄 License</strong>
      </a>
    </td>
  </tr>
</table>

---

## 🚀 Why Aileron?

When vibe coding on Antigravity, the default harness can easily get in the way. Agents end up over-reading context, over-planning simple edits, or stuck in endless loops repeating the same failed fixes.

**Aileron Protocol** solves this by splitting rules into **two specialized profiles**: **Core** (system logic, safety, execution discipline) and **Design** (aesthetics, styling, anti-slop guidelines).

| Feature / Metric | Default Harness | Aileron Protocol | Developer Benefit |
| :--- | :---: | :---: | :--- |
| **Latency** | 🐌 Slow (process overhead) | ⚡ **Lean** (loads only target rules) | Faster dev loops |
| **Token Use** | 💸 Heavy (over-reads context) | 📉 **Smart** (slims system files) | Clean context, lower cost |
| **UI Quality** | 🧪 AI Slop (arbitrary design) | 🎨 **Premium** (OKLCH, strict hierarchy) | Polished design out-of-the-box |
| **Debugging** | 🔄 Endless loops | 🛑 **Protected** (max 2 failures before prompt) | Saves wasted runs |
| **System Safety** | ⚠️ Speculative changes | 🏗️ **Risk-Aware** (caller checks first) | Fewer breaking changes |

> [!NOTE]
> **Model Compatibility:** Aileron is tuned for all models on Antigravity 2.0. We highly recommend Gemini 3.5 Flash for the absolute best performance across all of your tasks.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## ⚡ Specialized Profiles

Select the behavior profile your agent needs for the task:

<table width="100%">
  <tr>
    <td width="50%" valign="top" align="center">
      <a href="Aileron/Core/GEMINI.md">
        <img src="https://img.shields.io/badge/-⚙️_Core_Profile-a6e3a1?style=for-the-badge&logoColor=white" alt="Core Profile" />
      </a>
      <br /><br />
      <p align="left"><b>Core Logic & Safety:</b> Codebase-first execution, strict planning restraints, debugging discipline, and command optimization. Restricts question trees and prevents Windows terminal/permission exhaustion by prioritizing native tools. Allows minor pre-existing lint/type fixes in modified files to ensure verification stability.</p>
    </td>
    <td width="50%" valign="top" align="center">
      <a href="Aileron/Design/GEMINI.md">
        <img src="https://img.shields.io/badge/-🎨_Design_Profile-cba6f7?style=for-the-badge&logoColor=white" alt="Design Profile" />
      </a>
      <br /><br />
      <p align="left"><b>Frontend & Aesthetics:</b> Overrides the platform's rich-aesthetics defaults. Enforces clean spacing, Pantone 2026 Cloud Dancer palettes, and strict anti-slop rules (bans gradient text, ghost cards, raw saturation). Ensures high contrast and accessibility. Allows minor pre-existing lint/type fixes in modified files to ensure verification stability.</p>
    </td>
  </tr>
</table>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📂 Repository Structure

Each profile is packaged as a standalone `GEMINI.md` file:

```text
aileron-protocol/
├── Aileron/
│   ├── Core/      └── GEMINI.md
│   └── Design/    └── GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## 🛠️ Installation & Setup

Aileron profiles can be deployed **globally** (system-wide baseline) or **locally** (project-level override).

### 🌍 Global Setup (System-wide default)
Copy your preferred profile's `GEMINI.md` to:
*   **Windows:** `%USERPROFILE%\.gemini\GEMINI.md`
*   **macOS / Linux:** `~/.gemini/GEMINI.md`

### 📁 Workspace Setup (Project override)
Place the rules inside your active project workspace using either option:

*   **Option A (Root):** Copy `GEMINI.md` directly to the project root.
*   **Option B (Rules Dir):** Save the file as `.agents/rules/project-rules.md` (or any custom filename).

> [!IMPORTANT]
> If using **Option B**, you must prepend the following trigger header to the file (leaving a blank line after the closing `---`):
> ```markdown
> ---
> trigger: always_on
> ---
> 
> [Profile rules start here...]
> ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📄 License

Distributed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License**. See [LICENSE](LICENSE) for more details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
