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
    <td width="33%" align="center" nowrap>
      <a href="#-why-aileron">
        <strong>🚀 Why Aileron</strong>
      </a>
    </td>
    <td width="33%" align="center" nowrap>
      <a href="#-repository-structure">
        <strong>📂 Structure</strong>
      </a>
    </td>
    <td width="34%" align="center" nowrap>
      <a href="#%EF%B8%8F-installation--setup">
        <strong>🛠️ Installation</strong>
      </a>
    </td>
  </tr>
</table>

---

## 🚀 Why Aileron?

When vibe coding on Antigravity, the default harness can easily get in the way. Agents end up over-reading context, over-planning simple edits, or stuck in endless loops repeating the same failed fixes.

**Aileron Protocol** solves this by enforcing codebase-first execution, strict debugging safeties, command discipline, and rigorous anti-slop styling rules directly in your system/workspace configuration (**GEMINI.md**).

| Feature / Metric | Default Harness | Aileron Protocol | Developer Benefit |
| :--- | :---: | :---: | :--- |
| **Latency** | 🐌 Slow (process overhead) | ⚡ **Lean** (compact ruleset) | Faster dev loops |
| **Token Use** | 💸 Heavy (over-reads context) | 📉 **Smart** (slims instruction size) | Clean context, lower cost |
| **UI Quality** | 🧪 AI Slop (arbitrary design) | 🎨 **Premium** (restrained UI defaults) | Polished design out-of-the-box |
| **Debugging** | 🔄 Endless loops | 🛑 **Protected** (max 2 failures before prompt) | Saves wasted runs |
| **System Safety** | ⚠️ Speculative changes | 🏗️ **Risk-Aware** (caller checks first) | Fewer breaking changes |

> [!NOTE]
> **Model Compatibility:** Aileron is tuned for all models on Antigravity 2.0. We highly recommend Gemini 3.5 Flash for the absolute best performance across all of your tasks.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📂 Repository Structure

The configuration file is packaged inside the `Aileron/` folder:

```text
aileron-protocol/
├── Aileron/
│   └── GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## 🛠️ Installation & Setup

Aileron can be deployed **globally** (system-wide baseline) or **locally** (project-level override).

### 🌍 Global Setup (System-wide default)
Copy `GEMINI.md` to:
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
> [Rules start here...]
> ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📄 License

Distributed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License**. See [LICENSE](LICENSE) for more details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
