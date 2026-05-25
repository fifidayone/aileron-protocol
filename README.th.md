# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity Version" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Primary Model" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="License" /></a>

</div>

<div align="right">
  <strong>ภาษา:</strong>
  <a href="README.md">English 🇺🇸</a>
  <span>•</span>
  <span>ภาษาไทย 🇹🇭</span>
</div>

> [!NOTE]
> **"โมเดลไม่ได้แย่ — Harness ต่างหากที่ปล่อยมันลอยไร้ทิศ ติด Aileron ซะ แล้วคุณจะฟินไปกับมัน"**
>
> *— Aileron Protocol: ระบบควบคุมพฤติกรรม AI Agent บน Antigravity 2.0*

---

## 🚀 ทำไมต้องมี Aileron? (Aileron vs. Default Harness)

หงุดหงิดกับการ vibe coding บน Antigravity อยู่ใช่ไหม
ก็เพราะว่า AI มันชอบทำเกินหน้าที่ อ่าน context ทั้งโปรเจกต์ทั้งที่แก้แค่บรรทัดเดียว
วางแผนยาวเหยียดสำหรับงานง่ายๆ หรือไม่ก็ติดลูปวนแก้บั๊กเดิมซ้ำแล้วซ้ำอีก

**Aileron** แก้เรื่องนี้ตรงจุด — แยกกฎเป็น **5 โปรไฟล์ตามขนาดงาน** เลือกใช้ในแบบที่ต้องการ context สะอาด token ไม่รั่ว:

| ตัวชี้วัด | ไม่ใช้ Aileron (Default Harness) | ใช้ Aileron | ได้อะไร |
| :--- | :--- | :--- | :--- |
| **ความเร็ว** | 🐌 ช้า — งานเล็กก็โดนยัดขั้นตอนเต็ม | ⚡ ไว — โหลดแค่กฎที่ใช้จริง | dev loop เร็วขึ้น |
| **Token** | 💸 เปลือง — อ่านไฟล์ไม่เกี่ยว วางแผนเกินจำเป็น | 📉 ประหยัด — ข้ามแผน ตัด context ที่ไม่ต้องใช้ | ค่าใช้จ่ายลด context สะอาด |
| **UI** | 🧪 AI Slop — gradient มั่ว layout พัง ไม่มี scale | 🎨 คุณภาพ — สี OKLCH คุมโทน spacing เป๊ะ | UI ดูดีตั้งแต่ gen แรก |
| **Debug** | 🔄 วนลูป — แก้จุดเดิมซ้ำจนหมดเวลา | 🛑 หยุดทัน — พลาด 2 ครั้งก็ถามก่อน ไม่ดันทุรัง | ไม่เสีย run ฟรี |
| **Safety** | ⚠️ เสี่ยง — แก้ config, route, deps เองโดยไม่ถาม | 🏗️ รอบคอบ — เช็ค caller, API contract, DB risk ก่อน | ระบบไม่พังเพราะ AI |

> [!TIP]
> **เข้ากับโมเดลไหนบ้าง:** Aileron จูนมาให้ใช้กับทุกโมเดลบน Antigravity 2.0 แต่ถ้าอยากได้ผลลัพธ์ดีที่สุดในทุกงาน แนะนำให้ใช้คู่กับ Gemini 3.5 Flash

---

## ⚡ Profiles

5 โปรไฟล์ ฐานเดียวกัน แต่เน้นคนละแบบ:

| โปรไฟล์ | เหมาะกับ | เน้น |
| :--- | :--- | :--- |
| **⚡ Lite** | งานแก้ไว สำรวจโค้ด | เร็วเป็นหลัก — ทำตามที่สั่ง ข้ามขั้นตอนที่ไม่จำเป็น |
| **⚖️ Balanced** | งานฟีเจอร์รายวัน | ใช้ได้ทุกวัน — อ่าน code รอบๆ ก่อนแก้, plan เท่าที่งานต้องใช้ |
| **🎨 Studio** | งาน UI ขัดเกลาดีไซน์ | UI ต้องโอเค — layout, hierarchy, motion เช็ค render ก่อนส่ง |
| **🏗️ Architect** | งานระบบที่เสี่ยงพัง | รู้จักระบบก่อนแตะ — impact, caller, API contract, rollback |
| **👑 Ultimate** | งานระดับ production | คุมรอบด้าน — UI สวย, code ดี, ระบบแน่น |
---

## 📂 โครงสร้างโฟลเดอร์

แต่ละโปรไฟล์มาเป็นไฟล์ `GEMINI.md` แยกกัน หยิบใช้ได้เลย:

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

## 🛠️ ติดตั้งและใช้งาน

ติดตั้งโปรไฟล์ของ Aileron ได้ทั้งแบบ **Global** (เป็น default ของทั้งเครื่อง) หรือแบบ **Workspace** (override เฉพาะโปรเจกต์)

### 🌍 1. ติดตั้งแบบ Global (ใช้เป็น default ทั้งเครื่อง)
ก๊อปไฟล์ `GEMINI.md` ของโปรไฟล์ที่อยากใช้ ไปวางที่:
*   **Windows:** `%USERPROFILE%\.gemini\GEMINI.md` (เทียบเท่า `C:\Users\<ชื่อผู้ใช้>\.gemini\GEMINI.md`)
*   **macOS / Linux:** `~/.gemini/GEMINI.md`

### 📁 2. ติดตั้งแบบ Workspace (override เฉพาะโปรเจกต์)
วางไฟล์กฎไว้ในโปรเจกต์ที่ทำงานอยู่ เลือกวิธีไหนก็ได้:

*   **วิธี A (Root):** ก๊อป `GEMINI.md` ไปไว้ที่ root ของโปรเจกต์ตรงๆ
*   **วิธี B (Rules Dir):** บันทึกเป็น `.agents/rules/project-rules.md` (หรือจะตั้งชื่อไฟล์เป็นอย่างอื่นก็ได้)

> [!IMPORTANT]
> ถ้าเลือก **วิธี B** ต้องใส่ trigger header ไว้บนสุดของไฟล์ด้วย (บรรทัดที่ 4 ต้องเว้นว่างเปล่า):
> ```markdown
> ---
> trigger: always_on
> ---
> 
> [เนื้อหาของโปรไฟล์เริ่มจากตรงนี้...]
> ```

---

## 📄 License

เผยแพร่ภายใต้ **MIT License** ดูรายละเอียดได้ที่ [LICENSE](LICENSE)
