# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity Version" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Target Model" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="License" /></a>

</div>

<div align="right">
  <strong>Language:</strong>
  <span>English 🇺🇸</span>
  <span>•</span>
  <a href="README.th.md">ภาษาไทย 🇹🇭</a>
</div>

> [!NOTE]
> **"The model isn't underperforming; your agent harness is just letting it drift. It's time to add the ailerons."**
>
> *— Aileron Protocol: Precision Flight Control for AI Agents in Antigravity 2.0*

---

## 🚀 Why Aileron? (Aileron vs. Default Harness)

When vibe coding on Antigravity, the default harness can easily get in the way. Agents end up over-reading context, over-planning simple edits, or stuck in endless loops repeating the same failed fixes.

**Aileron Protocol** solves this by splitting rules into **five task-optimized profiles**. Choose the exact strictness you need, keep your context clean, and save tokens:

| Metric | Without Aileron (Default Harness) | With Aileron Protocol | Direct Developer Benefit |
| :--- | :--- | :--- | :--- |
| **Latency** | 🐌 Slow. Simple edits inherit massive process overhead. | ⚡ Lean. Only loads what's needed for the task. | Faster dev loops. |
| **Token Use** | 💸 Heavy. Over-plans and over-reads unrelated files. | 📉 Smart. Bypasses plans for minor edits; keeps context tight. | Lower bills & clean context. |
| **UI Quality** | 🧪 AI Slop. Saturated gradients, bad layouts, no standard scales. | 🎨 Premium UI. Restrained colors, OKLCH, and clean spacing. | Premium look out of the box. |
| **Debugging** | 🔄 Endless loops. Repeats the same failed fixes until timeout. | 🛑 Safe. Stops after 2 failures and asks for input. | Saves wasted runs. |
| **System Safety** | ⚠️ Risky. Speculatively changes configs, routes, or dependencies. | 🏗️ Risk-aware. Checks callers, API contracts, and database risks first. | Fewer breaking changes. |

> [!TIP]
> **Model Compatibility:** Aileron is tuned for all models on Antigravity 2.0, yet we highly recommend Gemini 3.5 Flash for the absolute best performance across all of your tasks.

---

## ⚡ Profiles

Five standalone profiles. Same base, different priorities:

| Profile | Best for | Priority |
| :--- | :--- | :--- |
| **⚡ Lite** | Quick fixes, exploration | Speed and staying out of the way — does what's asked, skips overplanning, lets the model move |
| **⚖️ Balanced** | Everyday feature work | Sensible balance — reads enough surrounding code to avoid shallow fixes, plans only when the work needs it |
| **🎨 Studio** | UI work and design polish | How the result looks and behaves on screen — composition, hierarchy, motion, viewing the rendered output |
| **🏗️ Architect** | System changes with real risk | Understanding the system before changing it — blast radius, callers, contracts, recovery paths |
| **👑 Ultimate** | High-stakes production work | Maximum coverage: polished UI, solid code, resilient systems |

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
└── LICENSE
```

---

## 🛠️ Installation & Setup

Aileron profiles can be deployed **globally** (system-wide baseline) or **locally** (project-level override).

### 🌍 1. Global Setup (System-wide default)
Copy your preferred profile's `GEMINI.md` to:
*   **Windows:** `%USERPROFILE%\.gemini\GEMINI.md` (Resolves to `C:\Users\<YourUsername>\.gemini\GEMINI.md`)
*   **macOS / Linux:** `~/.gemini/GEMINI.md`

### 📁 2. Workspace Setup (Project override)
Place the rules inside your active project workspace using either option:

*   **Option A (Root):** Copy `GEMINI.md` directly to the project root.
*   **Option B (Rules Dir):** Save as `.agents/rules/project-rules.md` (or any custom filename).

> [!IMPORTANT]
> If using **Option B**, you must prepend the following trigger header to the file (line 4 must be left completely blank):
> ```markdown
> ---
> trigger: always_on
> ---
> 
> [Profile rules start here...]
> ```

---

## 📄 License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for more details.
