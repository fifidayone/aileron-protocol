<a id="readme-top"></a>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:121826,100:2B3A54&height=220&section=header&text=Aileron%20Protocol&fontSize=70&fontAlignY=35&fontColor=F0EEEE" width="100%" alt="Aileron Protocol Banner" />
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&size=20&pause=1000&color=F0EEEE&center=true&vCenter=true&width=700&lines=Precision+flight+control+for+AI+agents;Slim+token+waste;Eliminate+diagnostic+loops;Deploy+premium+UI+instantly" alt="Typing SVG" />
  </a>
</p>

<div align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/Language-English_🇺🇸-89dceb?style=for-the-badge&logo=translate&logoColor=black" alt="English"/></a>
  <a href="README.th.md"><img src="https://img.shields.io/badge/Language-ภาษาไทย_🇹🇭-f2cdcd?style=for-the-badge&logo=translate&logoColor=black" alt="Thai"/></a>
</div>

<br />

<div align="center">
  <img src="https://img.shields.io/badge/-Antigravity_2.0-cba6f7?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity 2.0" />
  <img src="https://img.shields.io/badge/-Gemini_3.5_Flash-f9e2af?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Gemini 3.5 Flash" />
  <img src="https://img.shields.io/badge/-Gemini_3.1_Pro-fab387?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Gemini 3.1 Pro" />
  <img src="https://img.shields.io/badge/-Claude_Sonnet_4.6-94e2d5?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Sonnet 4.6" />
  <img src="https://img.shields.io/badge/-Claude_Opus_4.6-b4befe?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Opus 4.6" />
  <img src="https://img.shields.io/badge/-GPT--OSS-a6e3a1?style=for-the-badge&logo=openai&logoColor=white" alt="GPT-OSS" />
  <a href="LICENSE"><img src="https://img.shields.io/badge/-CC_BY--NC--SA_4.0-f5c2e7?style=for-the-badge&logo=creative-commons&logoColor=white" alt="CC BY-NC-SA 4.0" /></a>
</div>

<br />

---

<table align="center" width="100%">
  <tr>
    <td width="20%" align="center">
      <a href="#-why-aileron">
        <strong>💡 Why Aileron</strong>
      </a>
    </td>
    <td width="20%" align="center">
      <a href="#-task-optimized-profiles">
        <strong>⚡ Profiles</strong>
      </a>
    </td>
    <td width="20%" align="center">
      <a href="#-repository-structure">
        <strong>📂 Structure</strong>
      </a>
    </td>
    <td width="20%" align="center">
      <a href="#%EF%B8%8F-installation--setup">
        <strong>🛠️ Installation</strong>
      </a>
    </td>
    <td width="20%" align="center">
      <a href="#-license">
        <strong>📄 License</strong>
      </a>
    </td>
  </tr>
</table>

---

## 🚀 Why Aileron?

When vibe coding on Antigravity, the default harness can easily get in the way. Agents end up over-reading context, over-planning simple edits, or stuck in endless loops repeating the same failed fixes.

**Aileron Protocol** solves this by splitting rules into **five task-optimized profiles**. Choose the exact strictness you need, keep your context clean, and save tokens:

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



## ⚡ Task-Optimized Profiles

Select the exact strictness and behavior profile your agent needs for the task:

<table width="100%">
  <tr>
    <td width="33%" valign="top" align="center">
      <a href="Aileron/lite/GEMINI.md">
        <img src="https://img.shields.io/badge/-⚡_Lite_Profile-a6e3a1?style=for-the-badge&logoColor=white" alt="Lite Profile" />
      </a>
      <br /><br />
      <p align="left"><b>Speed & Agility:</b> Bypasses planning. Allows fast, direct code modifications with minimal harness friction. Best for quick bug fixes and exploratory coding.</p>
    </td>
    <td width="33%" valign="top" align="center">
      <a href="Aileron/balanced/GEMINI.md">
        <img src="https://img.shields.io/badge/-⚖️_Balanced_Profile-cbd8f7?style=for-the-badge&logoColor=white" alt="Balanced Profile" />
      </a>
      <br /><br />
      <p align="left"><b>Standard Development:</b> Sensible compromise. Inspects caller/callee context to prevent shallow fixes, planning only when multi-file risk is detected.</p>
    </td>
    <td width="33%" valign="top" align="center">
      <a href="Aileron/studio/GEMINI.md">
        <img src="https://img.shields.io/badge/-🎨_Studio_Profile-cba6f7?style=for-the-badge&logoColor=white" alt="Studio Profile" />
      </a>
      <br /><br />
      <p align="left"><b>Frontend & Design:</b> Visual craft. Enforces clean spacing, typography scales, OKLCH colors, interactive states, and rendering checks. Minimizes AI slop.</p>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top" align="center">
      <a href="Aileron/architect/GEMINI.md">
        <img src="https://img.shields.io/badge/-🏗️_Architect_Profile-94e2d5?style=for-the-badge&logoColor=white" alt="Architect Profile" />
      </a>
      <br /><br />
      <p align="left"><b>System Integrity:</b> Forces deep caller analysis, contract validation, and database migration risk assessment before editing shared systems.</p>
    </td>
    <td width="67%" valign="top" align="center" colspan="2">
      <a href="Aileron/ultimate/GEMINI.md">
        <img src="https://img.shields.io/badge/-👑_Ultimate_Profile-f9e2af?style=for-the-badge&logoColor=white" alt="Ultimate Profile" />
      </a>
      <br /><br />
      <p align="left"><b>High-Stakes Production:</b> Maximum execution quality. Merges Architect-level risk checks, Studio-level premium UI aesthetics, and strict verification loops.</p>
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
│   ├── lite/       └── GEMINI.md
│   ├── balanced/   └── GEMINI.md
│   ├── studio/     └── GEMINI.md
│   ├── architect/  └── GEMINI.md
│   └── ultimate/   └── GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## 🛠️ Installation & Setup

Aileron profiles can be deployed **globally** (system-wide baseline) or **locally** (project-level override).

### 🌍 Global Setup (System-wide default)
Copy your preferred profile's `GEMINI.md` to:
*   **Windows:** `<samp>%USERPROFILE%\.gemini\GEMINI.md</samp>`
*   **macOS / Linux:** `<samp>~/.gemini/GEMINI.md</samp>`

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
