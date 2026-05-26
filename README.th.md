# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

[![Antigravity Version](https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white)](https://github.com/)
[![Primary Model](https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white)](https://gemini.google.com/)
[![License MIT](https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge)](https://opensource.org/licenses/MIT)

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

หงุดหงิดกับการ vibe coding บน Antigravity อยู่ใช่ไหม? 
อ่าน context ทั้งโปรเจกต์ทั้งที่แก้แค่บรรทัดเดียว วางแผนยาวเหยียดสำหรับงานง่ายๆ หรือติดลูปวนแก้บั๊กเดิมซ้ำไปเรื่อยๆ จน Time out เสียเวลา เสีย Token ไปเปล่าๆ

**Aileron Protocol** เข้ามาแก้ปัญหานี้ตรงจุด — แยกกฎเป็น **5 โปรไฟล์ตามเป้าหมายของงาน** เลือกใช้เพื่อควบคุม Context ให้คลีน และป้องกัน Token รั่วไหล:

| ตัวชี้วัด | ไม่ใช้ Aileron (Default Harness) | ใช้ Aileron Protocol | ประโยชน์สูงสุดสำหรับ Developer |
| :--- | :--- | :--- | :--- |
| **ความเร็ว** | 🐌 ช้า — งานเล็กก็โดนยัดขั้นตอนแผนงานเต็มพิกัด | ⚡ ไว — โหลดเฉพาะกฎที่เกี่ยวข้องจริงเท่านั้น | Dev loops รวดเร็วขึ้นทันตา |
| **Token** | 💸 เปลือง — อ่านไฟล์ไม่เกี่ยวข้อง วางแผนเกินความจำเป็น | 📉 ประหยัด — ข้ามแผนในจุดแก้ไขเล็กน้อย รักษา Context ให้คลีน | ลดค่าใช้จ่าย & เคลียร์บริบท |
| **UI** | 🧪 AI Slop — ไล่เฉดสีมั่ว Layout พัง ไม่มีมาตราส่วนที่ชัดเจน | 🎨 คุณภาพสูง — ใช้โทนสี OKLCH สเปซสวยงาม คุม Contrast | หน้าจอสวยพรีเมียมตั้งแต่ Gen แรก |
| **Debug** | 🔄 วนลูป — แก้ไขบักจุดเดิมซ้ำซากจนหมดเวลา | 🛑 หยุดทัน — แจ้งข้อผิดพลาดหลังพลาด 2 ครั้งเพื่อขอคำแนะนำ | ไม่เสียโควตารันคำสั่งฟรี |
| **Safety** | ⚠️ เสี่ยง — ปรับเปลี่ยน config, route, deps เองโดยไม่ถาม | 🏗️ รอบคอบ — ตรวจสอบ caller, API contract และ DB risk ก่อน | ลดความเสี่ยงระบบพังหลังจาก AI สั่งเสร็จ |

> [!TIP]
> **การเข้ากันได้กับโมเดล:** Aileron ถูกปรับแต่งมาสำหรับทุกโมเดลบน Antigravity 2.0 แต่ถ้าอยากได้ประสิทธิภาพสูงสุดในทุกประเภทงาน แนะนำให้รันคู่กับ Gemini 3.5 Flash

---

## ⚡ Profiles

5 โปรไฟล์ บนพื้นฐานเดียวกัน แต่เน้นลำดับความสำคัญคนละด้าน:

| โปรไฟล์ | เหมาะสำหรับ | สิ่งที่เน้นย้ำ |
| :--- | :--- | :--- |
| [⚡ Lite](Aileron/lite/GEMINI.md) | งานแก้บักด่วน, การสำรวจโค้ด | ความเร็วเป็นหลัก — ทำตามสั่ง ข้ามขั้นตอนแผนงาน ยอมให้โมเดลทำงานไวที่สุด |
| [⚖️ Balanced](Aileron/balanced/GEMINI.md) | งานสร้างฟีเจอร์ทั่วไปในแต่ละวัน | ความสมดุล — อ่านโค้ดรอบด้านเพื่อป้องกันความผิดพลาด เขียนแผนเท่าที่จำเป็น |
| [🎨 Studio](Aileron/studio/GEMINI.md) | งาน UI และความละเอียดทางดีไซน์ | รูปลักษณ์และการจัดหน้าจอ — การจัดองค์ประกอบ, มาตราส่วนสเปซ, ตรรกะสี และการรันตรวจ Alignment |
| [🏗️ Architect](Aileron/architect/GEMINI.md) | งานระบบโครงสร้างที่มีความเสี่ยงสูง | ตรวจสอบแรงกระแทกก่อนลงมือ — caller, API contracts, แผนรับมือยามระบบขัดข้อง |
| [👑 Ultimate](Aileron/ultimate/GEMINI.md) | งานเตรียมขึ้น Production ระดับสูง | ครอบคลุมรอบด้าน — UI สวยพรีเมียม โค้ดเสถียร ระบบแข็งแกร่ง |

---

## 📂 โครงสร้างโฟลเดอร์

แต่ละโปรไฟล์จะแยกเป็นไฟล์ `GEMINI.md` อิสระ หยิบใช้งานง่าย:

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

---

## 🛠️ การติดตั้งและใช้งาน

โปรไฟล์ของ Aileron สามารถติดตั้งได้ทั้งแบบ **Global** (เป็นมาตรฐานเครื่อง) หรือแบบ **Workspace** (ควบคุมเฉพาะโปรเจกต์)

## Recommended

### 🌍 ติดตั้งแบบ Global (เป็นมาตรฐานทั้งเครื่อง)
คัดลอกไฟล์โปรไฟล์ที่คุณเลือก (`GEMINI.md`) ไปวางที่:
*   **Windows:** `%USERPROFILE%\.gemini\GEMINI.md` (เทียบเท่า `C:\Users\<ชื่อผู้ใช้>\.gemini\GEMINI.md`)
*   **macOS / Linux:** `~/.gemini/GEMINI.md`

## Optional

### 📁 ติดตั้งแบบ Workspace (Override เฉพาะโปรเจกต์)
คัดลอกไฟล์โปรไฟล์ไปวางไว้ในพื้นที่ทำงานของโปรเจกต์ของคุณ โดยเลือกทำข้อใดข้อหนึ่ง:

*   **วิธี A (Root):** วางไฟล์ `GEMINI.md` ไว้ที่ Root ของโปรเจกต์ตรงๆ
*   **วิธี B (Rules Dir):** บันทึกเป็นไฟล์ชื่อ `.agents/rules/project-rules.md` (หรือชื่อไฟล์ใดๆ ที่กำหนดเอง)

> [!IMPORTANT]
> หากเลือก **วิธี B** คุณต้องระบุหัวข้อ Trigger ไว้บนสุดของไฟล์เสมอ (โดยต้องเว้นบรรทัดว่าง 1 บรรทัดหลังจากปิดเครื่องหมาย `---`):
> ```markdown
> ---
> trigger: always_on
> ---
> 
> [เนื้อหากฎโปรไฟล์เริ่มต้นตรงนี้...]
> ```

---

## 📄 License

เผยแพร่ภายใต้เงื่อนไข **MIT License** รายละเอียดเพิ่มเติมดูได้ที่ [LICENSE](LICENSE)
