# 🌌 Antigravity 2.0 — Aileron Protocol (Thai)

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity Version" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Primary Model" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="License" /></a>

</div>


> [!NOTE]
> **"โมเดลไม่ได้ทำงานแย่ แต่เป็นเพราะ Default Harness ที่ปล่อยให้มันทำงานสะเปะสะปะ ถึงเวลาติดปีก (Ailerons) เพื่อคุมทิศทางให้มันแล้ว"**
>
> *— Aileron Protocol: ระบบนำร่องที่แม่นยำสำหรับ AI Agents บน Antigravity 2.0*

---

## 🚀 Why Aileron Protocol?

ปัญหาคลาสสิกของการใช้ AI Agent เขียนโค้ดใน **Google Antigravity 2.0** คือภาวะข้อมูลท่วมท้น **(System-Induced Cognitive Dilution)** เมื่อตัวเอเจนต์ต้องแบกรับคำสั่งขนาดใหญ่จากระบบตัวควบคุม **(Harness Directives)** ไม่ว่าจะเป็น System Prompt, คำแนะนำการใช้เครื่องมือ หรือแนวทางการพัฒนาทั่วไปที่ถูกป้อนเข้าระบบตั้งแต่เริ่มต้น ส่งผลให้สมาธิและความจำของโมเดลหลุดโฟกัส **(Cognitive Drift)** นำไปสู่ปัญหาเหล่านี้:

*   **Infinite Debugging Loops:** AI วนแก้โค้ดที่เดิมซ้ำไปซ้ำมาแบบมืดแปดด้าน แทนที่จะตั้งสมมติฐานใหม่
*   **Context & Token Bloat:** โหลดประวัติแชทหรืออ่านไฟล์ที่ไม่เกี่ยวกับงาน ทำให้เปลือง Token และตอบสนองช้า
*   **Visual & UI Slop:** เขียน UI ออกมาดูราคาถูก สาดสีฉูดฉาด (Raw Saturation) ใช้ Gradient พร่ำเพรื่อ หรือวาง Layout โดยไม่มีช่องไฟ (Breathing Room)
*   **Boundary & Scope Drift:** แอบไปแก้โครงสร้างโปรเจกต์ หรือรื้อ Dependency/Routing โดยไม่ได้สั่ง

**Aileron Protocol** ถูกออกแบบมาเพื่อแก้ปัญหาเหล่านี้ โดยแยก Rules ออกเป็น **5 โปรไฟล์ตามลักษณะงาน** การจำกัด Scope การทำงานให้แคบและตรงจุด จะช่วยลดภาระการประมวลผลของ AI ทำให้ตอบสนองไวขึ้น ประหยัด Token และยกระดับคุณภาพโค้ดหรือ UI ที่ได้

> [!TIP]
> **Model Compatibility & Sweet Spot:**
> Aileron Protocol ออกแบบมาสำหรับ Antigravity 2.0 และจูนกับพฤติกรรมของ Gemini-style coding agent เป็นหลัก โดยควรใช้ได้กับโมเดลเขียนโค้ดที่มีความสามารถสูงตัวอื่นด้วย แต่อาจต้องเลือกโปรไฟล์และระดับความเข้มให้เหมาะกับโมเดลนั้นๆ จุดที่เหมาะที่สุดคือการใช้งานรายวันแบบเร็วและคุ้มค่ากับโมเดลสาย Gemini Flash

---

## 💡 What You Gain: Aileron vs Default Harness

การเปลี่ยนมาใช้ Aileron Protocol จะยกระดับพฤติกรรมการเขียนโค้ดและแก้บั๊กของ AI ได้อย่างชัดเจน:

| Metrics | Default Harness | Aileron Protocol | ประโยชน์สูงสุดที่จะได้รับ |
| :--- | :--- | :--- | :--- |
| **Latency** | 🐌 ช้า เพราะงานเล็กอาจยังโดนพฤติกรรมกว้างๆ ของ Harness เดิมลากไปด้วย | ⚡ เร็วขึ้น โปรไฟล์ **Lite** จะโหลดเฉพาะ Instruction เท่าที่จำเป็น | ลดรอบการทำงานที่ไม่จำเป็นในงานเล็กถึงกลาง |
| **Token Usage** | 💸 เปลือง เพราะ Default behavior อาจวางแผนหรืออ่าน Context เกินจำเป็น | 📉 ประหยัดขึ้น ตัดขั้นตอน Plan ที่ไม่จำเป็นออก และจำกัดขอบเขต Context | ลด Token และลด Context Bloat |
| **UI Quality** | 🧪 จืดชืด หรือไม่ก็สาดสี UI แบบ AI Slop ทั่วไป | 🎨 พรีเมียม บังคับใช้สไตล์ที่ดูแพง คุมโทนสี ทรานซิชัน และช่องไฟให้เป๊ะ | **ได้ UI ที่ดูหรูหรา น่าใช้งาน** |
| **Debugging** | 🔄 วนแก้บั๊กมั่วซั่วจนกว่า API จะ Timeout | 🛑 หยุดเมื่อหลงทาง ถ้าแก้พลาดติดกัน 2 ครั้ง ระบบจะหยุดเพื่อขอหลักฐานหรือทิศทางใหม่ | ลดการเผา Token ซ้ำกับลูปที่ล้มเหลว |
| **System Safety** | ⚠️ เสี่ยง แอบอัปเดตไลบรารี หรือแก้ Config เองโดยพละการ | 🏗️ รัดกุมขึ้น ตรวจ callers, contracts, migration risk และ external impact ก่อน | ลดโอกาสเกิด Regression และ Deploy Break |

---

## ⚡ The 5 Profiles

เลือกโปรไฟล์ที่เหมาะกับ Task ของคุณ เพื่อคุม Token และบังคับพฤติกรรมของ Agent:

| Profile | Velocity & Loop | Token Usage | เหมาะสำหรับ |
| :--- | :--- | :---: | :--- |
| **⚡ Lite** | **Frictionless Velocity** <br>*(ไม่ต้องมีพิธีรีตอง ไม่เขียน Plan ลุยแก้เลย)* | 📉 ต่ำสุด | งานแก้บั๊กจุดเล็กๆ, สั่งแก้ไฟล์เดียว, Quick Fixes |
| **⚖️ Balanced** | **Dynamic Velocity** <br>*(มาตรฐานสำหรับใช้งานทั่วไป คุย Plan สั้นๆ ในแชท)* | 📊 ปานกลาง | เขียนฟีเจอร์ทั่วๆ ไป, งานโค้ดดิ้งแบบ Day-to-Day |
| **🎨 Studio** | **Accelerated UI** <br>*(เน้นคราฟต์ UI และพรีวิวผ่านเบราว์เซอร์)* | 📈 สูง | ออกแบบหน้าเว็บ, วาง Layout CSS, คราฟต์ Animations |
| **🏗️ Architect** | **Structured Velocity** <br>*(ประเมินความเสี่ยง มีหลักฐานก่อนลงมือทำ)* | 📈 สูง | รื้อโครงสร้างระบบ (Refactor), วางเส้น API, ปรับแก้ Database Schema |
| **👑 Ultimate** | **Rigorous Velocity** <br>*(คุมเข้ม หลายชั้น ตรวจละเอียด)* | 👑 สูงสุด | โปรเจกต์ความเสี่ยงสูง, งาน Full-Stack ที่ต้องการความรัดกุมสูง |

---

## 🎯 Quick Selector

เลือกโปรไฟล์ที่เหมาะสมกับรูปแบบการทำงานและความเสี่ยงของงานที่คุณกำลังทำอยู่:

*   **⚡ Lite (เน้นความเร็วสูงสุด - Direct Execution)**
    👉 เหมาะสำหรับงานที่คุณต้องการให้ Agent ลงมือแก้ไขโค้ดทันทีโดยไม่ต้องมีขั้นตอนยุ่งยาก โปรไฟล์นี้จะข้ามการเขียนไฟล์ Plan เช่น `implementation_plan.md` เป็นค่าเริ่มต้น เหมาะมากในกรณีที่บรีฟงานเคลียร์แล้วในแชทและต้องการเห็นผลลัพธ์ทันที
*   **⚖️ Balanced (งานพัฒนาฟีเจอร์ทั่วไป - Daily Driver)**
    👉 โปรไฟล์เริ่มต้นสำหรับใช้งานทั่วไปในทุกๆ วัน ใช้การตกลงแผนงานแบบย่อผ่านแชทแทนการสร้างไฟล์ Plan แยก ช่วยควบคุมปริมาณ Token และให้ความปลอดภัยที่พอดีกับงานทั่วไป
*   **🎨 Studio (งานดีไซน์และคราฟต์หน้าจอ - Frontend Specialist)**
    👉 เหมาะสำหรับงานแต่งหน้าตา UI, จัด CSS Layout หรือทำ Animation โปรไฟล์นี้จะบังคับใช้หลักดีไซน์ที่ประณีต คุมระบบสี OKLCH, คอนทราสต์ และทรานซิชันที่ลื่นไหล เพื่อไม่ให้หน้าเว็บออกมาดูราคาถูกแบบ AI Slop
*   **🏗️ Architect (งานระบบและโครงสร้างหลัก - Backend & Systems)**
    👉 เหมาะสำหรับงานปรับเปลี่ยน Database Schema, ออกแบบ API หรือรีแฟกเตอร์ระบบใหญ่ โปรไฟล์นี้จะบังคับให้ประเมินความเสี่ยงด้วยคำถามเจาะลึก (Tree-Chain) และบันทึกประวัติการดีบั๊ก (Evidence Trail) ก่อนลงมือเขียนโค้ดเสมอ
*   **👑 Ultimate (งาน Full-Stack ความเสี่ยงสูง - Mission-Critical)**
    👉 โปรไฟล์ขั้นสุดสำหรับระบบสำคัญ โดยจะดึงเอากฎความเนี้ยบของ *Studio* มารวมกับความรัดกุมระดับระบบของ *Architect* และใช้การจัดแนวทางล่วงหน้าสำหรับงาน Full-Stack ซับซ้อนที่ความถูกต้องสำคัญกว่าความเร็ว

---

## 📂 Detailed Breakdown

<details>
<summary><b>⚡ Lite Profile</b></summary>

*   **Goal:** ตัด Process ที่ไม่จำเป็นออกให้หมด มุ่งเน้นการแก้ปัญหาให้เร็วที่สุด
*   **Strategy:**
    *   ข้ามการสร้างไฟล์ Plan เช่น `implementation_plan.md` เป็นค่าเริ่มต้น นอกเสียจากผู้ใช้จะสั่ง
    *   ใช้ Styling เดิมที่มีอยู่ในโปรเจกต์ ห้ามเพิ่มดีไซน์ใหม่เอง
    *   โฟกัสที่จุดเกิดบั๊กและเขียนโค้ดทับทันที ลดการสแกน Context ข้ามไฟล์
</details>

<details>
<summary><b>⚖️ Balanced Profile</b></summary>

*   **Goal:** รักษาสมดุลระหว่าง Speed และโครงสร้างการทำงาน
*   **Strategy:**
    *   ใช้การอธิบายสั้นๆ ในแชทเพื่อ Align งานก่อนเขียนโค้ด ไม่ต้องสร้างไฟล์ Plan แยก
    *   เบรกพฤติกรรม AI Slop ของหน้าเว็บ (ห้ามใช้ Glassmorphism พร่ำเพรื่อ หรือพ่นเกรเดียนท์มั่ว)
    *   ปรับตัวตามสเกลงาน: งานเล็กสามารถข้าม Plan ได้ แต่งานสเกลกลางต้องผ่านการตรวจทานความถูกต้องเสมอ
</details>

<details>
<summary><b>🎨 Studio Profile</b></summary>

*   **Goal:** คราฟต์ UI ให้ดูโดดเด่น หรูหรา และเป็นงานระดับ Premium
*   **Strategy:**
    *   บังคับใช้หลัก Typography และ Color Theory (ระยะช่องไฟเป๊ะ, คอนทราสต์ $\ge$ 4.5:1, คุมโทนสีด้วย OKLCH)
    *   ตั้งกฎฟิสิกส์สำหรับ Animations และ Custom Cursors อย่างเข้มงวด (ห้ามใช้ `transition: all` เพื่อป้องกัน Layout Shift)
    *   กรองการทำงานของรูปภาพและ SVG เพื่อรักษาความคลีนของ DOM
</details>

<details>
<summary><b>🏗️ Architect Profile</b></summary>

*   **Goal:** ใช้รับมือกับงาน System Architecture, Migrations และ Backend Core
*   **Strategy:**
    *   ใช้ Adaptive Tree-Chain Questioning เพื่อ Align เรื่อง Schema ให้ชัดก่อนเริ่มโค้ด
    *   บังคับบันทึก Evidence Trail สำหรับการหาบั๊ก (อาการ $\rightarrow$ สมมติฐาน $\rightarrow$ ตรวจสอบ $\rightarrow$ ผลลัพธ์)
    *   เน้น UI ที่ตอบสนองไว ข้อมูลครบถ้วน ลด Animations ที่ไม่จำเป็นทิ้ง
</details>

<details>
<summary><b>👑 Ultimate Profile</b></summary>

*   **Goal:** กฎเข้มสุดสำหรับคุมวินัย AI ในงาน Full-Stack ที่ต้องการความรัดกุมสูง
*   **Strategy:**
    *   ผสานข้อบังคับของทุกโปรไฟล์ (ความหรูหราของ UI + ความแข็งแกร่งของระบบหลังบ้าน)
    *   บังคับจัดแนวทางให้ชัดและเพิ่มชั้น Verification สำหรับงานซับซ้อนหรือเสี่ยงสูง
    *   ยอมแลกกับ Latency และ Token ที่มากขึ้น เพื่อลดรอบแก้ซ้ำในงานสำคัญ
</details>

---

## 📂 Repository Structure

โปรไฟล์ทั้งหมดจะถูกแบ่งแยกตามโฟลเดอร์ เพื่อให้ Agent นำไฟล์ `GEMINI.md` ไปใช้ได้อย่างถูกต้อง:

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

## 🛠️ Installation & Usage

สามารถติดตั้ง Aileron Protocol ได้ 2 ระดับ: **Global** (ครอบคลุมทั้งเครื่อง) หรือ **Workspace** (จำกัดเฉพาะโปรเจกต์)

### 🌍 1. Global Setup (Recommended)
ตั้งค่าให้ Antigravity Agent ใช้โปรไฟล์นี้เป็น Default ในทุกๆ โฟลเดอร์ที่ทำงาน เพื่อให้โค้ดเป็นมาตรฐานเดียวกันโดยไม่ต้องก็อปไฟล์ไปมา

คัดลอกไฟล์ `GEMINI.md` ของโปรไฟล์ที่คุณต้องการ (เช่น `Aileron/ultimate/GEMINI.md`) ไปวางที่ตำแหน่งต่อไปนี้ ตาม OS ของคุณ:

*   **Windows**:
    ```bash
    %USERPROFILE%\.gemini\GEMINI.md
    ```
*   **macOS / Linux**:
    ```bash
    ~/.gemini/GEMINI.md
    ```

---

### 📁 2. Workspace Setup (Project-specific)
สำหรับโปรเจกต์ที่ต้องการ Rule เฉพาะตัว **(กฎระดับ Workspace จะ Override กฎ Global เสมอ)**

สามารถตั้งค่าได้ 2 วิธี:

#### วิธีที่ 1: วางไว้ที่ Root ของโปรเจกต์
คัดลอก `GEMINI.md` ไปวางไว้ที่ Root directory ของโปรเจกต์นั้นๆ เลย:
```text
your-project-workspace/
├── GEMINI.md  <-- วางที่นี่
├── src/
└── package.json
```

#### วิธีที่ 2: ใช้โฟลเดอร์ `.agents/rules`
คัดลอกไฟล์โปรไฟล์ไปไว้ในไดเรกทอรี `.agents/rules/` ที่อยู่ตรง Root ของโปรเจกต์:
```text
your-project-workspace/
├── .agents/
│   └── rules/
│       └── project-rules.md  <-- วางที่นี่ (เปลี่ยนชื่อไฟล์ตามต้องการ)
├── src/
└── package.json
```
*   **Flexible Naming:** ในโฟลเดอร์นี้ไม่จำเป็นต้องใช้ชื่อ `GEMINI.md` (สามารถเปลี่ยนชื่อเป็น `aileron-architect.md` หรือ `project-rules.md` ได้เลย)
*   **Requirements:** เพื่อให้ Agent มองเห็นและทำงาน คุณ**ต้อง**เพิ่ม Frontmatter 3 บรรทัดนี้ไว้ด้านบนสุดของไฟล์ และเว้นบรรทัดที่ 4 ให้ว่างไว้เสมอ:

```markdown
---
trigger: always_on
---

[เนื้อหาของโปรไฟล์เริ่มตั้งแต่บรรทัดที่ 5 เป็นต้นไป...]
```

> [!WARNING]
> บรรทัดที่ 4 จะต้องว่างเปล่า (Empty Line) เสมอ เพื่อให้ตัว Parser ของ Agent อ่าน Rules ได้ถูกต้อง

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
