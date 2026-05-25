# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity Version" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Target Model" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="License" /></a>

</div>


> [!NOTE]
> **"The model isn't underperforming; your agent harness is just letting it drift. It's time to add the ailerons."**
>
> *— Aileron Protocol: Precision Flight Control for AI Agents in Antigravity 2.0*

---

## 🚀 Why Aileron Protocol?

Operating autonomous coding agents in developer environments like **Google Antigravity 2.0** exposes a critical challenge: **system-induced cognitive dilution**. When agents are burdened by monolithic harness directives—such as extensive system prompts, tool instructions, and general developer guidelines injected at startup—their attention drifts, leading to high latency and suboptimal execution patterns:

*   **Infinite Debugging Loops:** AI repeating identical, failing test patches instead of forming new hypotheses.
*   **Context & Token Bloat:** Recursive, expensive reads of logs and unrelated workspace directories.
*   **Visual & UI Slop:** Generating cheap visual components that lack proper typographic breathing room, alignment, or accessibility contrast.
*   **Boundary & Scope Drift:** Speculatively modifying global routing, dependencies, or infrastructure files without explicit approval.

The **Aileron Protocol** mitigates these behaviors by decomposing system directives into **five task-optimized control profiles**. By matching the rule constraints to the immediate task scale, developers can eliminate cognitive overhead, minimize execution latency, and secure premium codebase quality.

> [!TIP]
> **Model Compatibility & Optimizations:**
> Aileron Protocol is designed for Antigravity 2.0 and tuned around Gemini-style coding-agent behavior. It should also work with other capable coding models, but profile choice and strictness may need adjustment. The practical sweet spot is fast, low-cost daily work on Gemini Flash-style models.

---

## 💡 What You Gain: Aileron vs. Default Harness

Operating under the Aileron Protocol yields immediate, measurable improvements in agent behavior compared to a default, unsegmented global rule configuration:

| Scenario / Metric | Without Aileron (Default Harness) | With Aileron Protocol | Direct Developer Benefit |
| :--- | :--- | :--- | :--- |
| **Response Latency** | 🐌 High. Minor edits can still inherit broad harness behavior. | ⚡ Lean. **Lite** profile reads only the essentials. | Faster small/medium execution loops. |
| **Token Footprint** | 💸 Heavy. Default behavior can over-plan or over-read for simple fixes. | 📉 Smart. Skips plans for minor work; keeps context clean. | Lower token usage and less context bloat. |
| **Visual Quality** | 🧪 Sterile or generic. Saturated gradients, poor layouts, no standard scales. | 🎨 Premium UI. Restrained colors, OKLCH, accessibility guidelines. | More polished UI without obvious AI visual slop. |
| **Debugging Integrity** | 🔄 Infinite loop. Repeats edits on failing tests until timeout. | 🛑 Safer. Stops after 2 failures and asks for new evidence or direction. | Cuts repeated failed-loop waste. |
| **Architectural Safety** | ⚠️ Risky. Modifies dependencies or system routes without risk analysis. | 🏗️ Risk-aware. Checks callers, contracts, migration risk, and external impact first. | Reduces regression and deploy-break risk. |

---

## ⚡ The 5 Flavors of Alignment

Select the profile that fits your immediate task to optimize for execution flow and token consumption:

| Profile | Execution Flow | Token Cost | Best Suited For |
| :--- | :--- | :---: | :--- |
| **⚡ Lite** | **Frictionless Velocity** <br>*(Direct execution; bypasses plans)* | 📉 Minimal | Hotfixes, minor bug fixes, single-file edits. |
| **⚖️ Balanced** | **Dynamic Velocity** <br>*(Standard daily driver; light chat planning)* | 📊 Moderate | Everyday development, routine features, standard tasks. |
| **🎨 Studio** | **Accelerated UI** <br>*(Rapid local render and preview loops)* | 📈 High | Landing pages, high-fidelity styling, UX and motion details. |
| **🏗️ Architect** | **Structured Velocity** <br>*(Risk-checked; evidence trail)* | 📈 High | Major refactoring, API upgrades, schema design. |
| **👑 Ultimate** | **Rigorous Velocity** <br>*(Full guardrails; multi-layer checks)* | 👑 Maximum | Critical path tasks, sensitive configurations, high-assurance goals. |

---

## 🎯 Quick Selector

Choose your active profile based on the development mode and risk tolerance of your task:

*   **⚡ Lite (Direct & High-Speed Development)**
    👉 Choose when you want the agent to start coding immediately. It skips process files such as `implementation_plan.md` by default, optimizing for direct, iterative edits. Ideal when the task requirements are already clear.
*   **⚖️ Balanced (Standard Feature Development)**
    👉 The default daily driver. It uses quick chat-based alignment instead of heavy planning files, offering a balanced mix of development speed, token efficiency, and basic guardrails.
*   **🎨 Studio (Premium Frontend & UI Crafting)**
    👉 Choose when styling, layout, or animations are the priority. It enforces strict design systems, color theories (OKLCH, contrast $\ge$ 4.5:1), and motion physics while preventing low-quality "AI slop" interfaces.
*   **🏗️ Architect (Core Backend & Systems Engineering)**
    👉 Choose for complex database schema changes, API design, or major refactoring. It enforces step-by-step risk assessment (Tree-Chain Questioning) and detailed debugging records (Evidence Trail) before executing.
*   **👑 Ultimate (Mission-Critical Full-Stack Alignment)**
    👉 The strongest guardrail mode. It merges the premium UI craft of *Studio* with the structural discipline of *Architect*, using planning alignment for complex full-stack changes where correctness matters more than speed.

---

## 📂 Profiles Breakdown

<details>
<summary><b>⚡ Lite Profile details</b></summary>

*   **Objective:** Maximize execution speed and eliminate process overhead.
*   **Key Strategies:**
    *   Bypasses the creation of formal planning files such as `implementation_plan.md` unless explicitly ordered.
    *   Enforces the use of existing system styles; strictly prohibits generating speculative visual assets.
    *   Inspects minimal context and applies changes directly, preventing multi-file verification loops.
</details>

<details>
<summary><b>⚖️ Balanced Profile details</b></summary>

*   **Objective:** The sweet spot between developer speed, token consumption, and code validation.
*   **Key Strategies:**
    *   Utilizes quick chat-based planning for multi-file updates, saving context space.
    *   Blocks styling slop (prohibits cheap gradients, raw saturation, and excessive glassmorphism).
    *   Forks into direct execution for minor edits, and safety-checked validation for intermediate features.
</details>

<details>
<summary><b>🎨 Studio Profile details</b></summary>

*   **Objective:** High-end, premium visual designs with buttery-smooth interactions.
*   **Key Strategies:**
    *   Enforces strict anti-AI slop visual guidelines (prefers restrained palettes, OKLCH, proper typographic breathing room, and alignment).
    *   Configures rigorous rules for custom cursors and physics-based motion (gated JS initialization, no `transition: all` layout reflows).
    *   Maintains a minimum WCAG AA contrast ratio ($\ge$ 4.5:1) for normal text and interactive states.
</details>

<details>
<summary><b>🏗️ Architect Profile details</b></summary>

*   **Objective:** Risk-aware backend refactoring, API integration, and database operations.
*   **Key Strategies:**
    *   Integrates **Adaptive Tree-Chain Questioning** to align on database schemas and API designs before execution.
    *   Enforces a strict **Evidence Trail** for diagnostics (Symptom $\rightarrow$ Hypothesis $\rightarrow$ Check $\rightarrow$ Result).
    *   Strips decorative elements, designing interfaces prioritizing functional density and semantic markup.
</details>

<details>
<summary><b>👑 Ultimate Profile details</b></summary>

*   **Objective:** Full monolithic safety for complex codebases.
*   **Key Strategies:**
    *   Combines all constraint profiles (Studio, Architect, Balanced) into a single, comprehensive instruction set.
    *   Enforces rigorous planning alignment and comprehensive multi-layer verification for complex or high-risk work.
    *   Optimizes for correctness and fewer debugging cycles at the cost of higher upfront token overhead.
</details>

---

## 📂 Repository Structure

The repository organizes profiles by directory so that each file is named `GEMINI.md` as required by the agent platform during execution:

```text
aileron-protocol/
├── Aileron/
│   ├── lite/
│   │   └── GEMINI.md
│   ├── balanced/
│   │   └── GEMINI.md
│   ├── studio/
│   │   └── GEMINI.md
│   ├── architect/
│   │   └── GEMINI.md
│   └── ultimate/
│       └── GEMINI.md
├── README.md
└── LICENSE
```

---

## 🛠️ Installation & Setup

Aileron Protocol rules can be deployed either **globally** (for universal agent alignment) or **locally** (for project-specific overrides).

### 🌍 1. Global Setup (Highly Recommended)
Deploying rules globally ensures the central agent engine utilizes the profile as its universal default behavior baseline. This establishes platform-wide discipline without cluttering individual directories.

Copy the `GEMINI.md` file from your desired profile folder (e.g., `Aileron/ultimate/GEMINI.md` or `Aileron/balanced/GEMINI.md`), and save it to the following location depending on your Operating System:

*   **Windows**:
    ```bash
    %USERPROFILE%\.gemini\GEMINI.md
    # Resolves to: C:\Users\<YourUsername>\.gemini\GEMINI.md
    ```
*   **macOS / Linux**:
    ```bash
    ~/.gemini/GEMINI.md
    # Resolves to: /Users/<YourUsername>/.gemini/GEMINI.md or /home/<YourUsername>/.gemini/GEMINI.md
    ```

---

### 📁 2. Workspace Setup (Optional Overrides)
For project-specific requirements, you can define workspace-level rules. **Workspace configuration takes priority and will automatically override the global baseline.**

Choose one of the following directory structures inside your active project workspace:

#### Option A: Root-Level Configuration
Copy the `GEMINI.md` file of your chosen profile directly to the root of your project directory:
```text
your-project-workspace/
├── GEMINI.md  <-- Place here
├── src/
└── package.json
```

#### Option B: Rules Directory (`.agents/rules`)
Copy the profile rule file into the `.agents/rules/` directory at the root of your project:
```text
your-project-workspace/
├── .agents/
│   └── rules/
│       └── project-rules.md  <-- Place here (custom name allowed)
├── src/
└── package.json
```
*   **Filename Flexibility:** When placed inside `.agents/rules/`, the file does not have to be named `GEMINI.md`. You can rename it descriptively (e.g., `aileron-architect.md` or `project-rules.md`).
*   **Trigger Header Requirement:** To ensure the orchestration harness registers and applies this rule, you **must** prepend the following frontmatter header at the absolute top of the file (lines 1 to 3), followed by a **blank line** on line 4:

```markdown
---
trigger: always_on
---

[Your Aileron profile rules text starts here...]
```

> [!WARNING]
> Ensure that line 4 remains completely blank immediately after the closing `---` metadata marker before starting the markdown body. Failing to do so may prevent the agent harness from recognizing the trigger header.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.
