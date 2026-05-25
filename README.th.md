# 🌌 Antigravity 2.0 — Aileron Protocol

<div align="center">

<a href="https://github.com/"><img src="https://img.shields.io/badge/Antigravity-2.0-8A2BE2?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity 2.0" /></a>
<a href="https://gemini.google.com/"><img src="https://img.shields.io/badge/Designed_For-Gemini_Agent-FF6B00?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Gemini Agent" /></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-00C853?style=for-the-badge" alt="MIT License" /></a>

</div>

> **Aileron Protocol** คือชุดไฟล์ `GEMINI.md` สำหรับใช้เป็น baseline ของ Antigravity 2.0
> เป้าหมายคือทำให้ agent วางแผน อ่าน context ใช้ tool และตรวจงานในระดับที่พอดีกับงานจริง

[Read in English](README.md)

---

## ทำไมต้องมี

Default harness ของ Antigravity ครอบคลุมกว้างมาก ซึ่งมีประโยชน์ในแง่ความยืดหยุ่น แต่บางงานก็ทำให้ agent วางแผนเยอะเกิน อ่านไฟล์เกิน ใช้ tool เกิน สร้าง artifact ที่ไม่จำเป็น ไล่ทำ UI effect แบบ generic หรือวน debug โดยไม่มีหลักฐานใหม่

Aileron เป็น global baseline ที่ช่วยคุมพฤติกรรมเหล่านี้ให้แคบและตรงงานขึ้น โดยยังให้กฎระดับ workspace เช่น `GEMINI.md` หรือ `.agents/rules` มาทับได้ตามแต่ละโปรเจกต์

---

## โปรไฟล์

แต่ละโปรไฟล์เป็นไฟล์ standalone ใช้งานได้เดี่ยวๆ ให้เลือกหนึ่งไฟล์แล้วนำไปใช้เป็น `GEMINI.md`

| Profile | แนวทาง | UI default | Verification | เหมาะกับ |
| :--- | :--- | :--- | :--- | :--- |
| **Lite** | เร็วที่สุด พิธีรีตองน้อยสุด | UI พอใช้จริงระดับ production แบบเรียบ อ่านง่าย | ตรวจเท่าที่จำเป็น | งานเล็ก งานชัด แก้เร็ว |
| **Balanced** | baseline สำหรับใช้ทุกวัน | minimal product UI ที่ดูเรียบร้อย | ตรวจจริงเมื่อมีความเสี่ยง | งานทั่วไป งานขนาดกลาง |
| **Studio** | เน้น UI/render/design | งาน UI หน้าตาดีระดับ premium | render check สำหรับ UI สำคัญ | Frontend, landing page, visual polish |
| **Architect** | เน้นความเสี่ยงและโครงสร้างระบบ | UI เชิงระบบที่ชัดและดูแลต่อได้ แต่ยังทำงาน aesthetic ได้เมื่อสั่ง | ตรวจลึกขึ้นเมื่อแตะ shared behavior | refactor, API, schema, migration |
| **Ultimate** | guardrail ครบสุด | premium เมื่อเป็นงาน UI | ตรวจเข้มที่สุด | งานสำคัญ งานเสี่ยง งานคลุมเครือ |

โครงสร้างไฟล์อาจคล้ายกัน เพราะทุกไฟล์ต้องใช้งานเดี่ยวได้ ความต่างหลักอยู่ที่ threshold และแรงบังคับ: Lite ปล่อยให้ agent ลงมือเร็วกว่า ส่วน Ultimate ปิดช่องหลุดของ harness เดิมมากกว่า

---

## เลือกตัวไหนดี

- ใช้ **Lite** เมื่องานชัด และต้องการให้ agent ลงมือเร็ว
- ใช้ **Balanced** เป็น global baseline หลักสำหรับงานประจำ
- ใช้ **Studio** เมื่อหน้าตา UI คือส่วนสำคัญของงาน
- ใช้ **Architect** เมื่องานแตะ shared behavior, schema, API, migration หรือ architecture
- ใช้ **Ultimate** เมื่องานต้องการความถูกต้อง คุณภาพ UI และการคุมความเสี่ยงมากกว่าความเร็ว

---

## Aileron คุมอะไรบ้าง

- ลด planning/artifact ceremony ในงานทั่วไป
- ลดการแนะนำ slash command หรือ subagent ที่ไม่จำเป็น
- ลดการอ่าน context กว้างเกินและการย้อนอ่าน transcript เก่า
- หยุด debug loop ที่ไม่มีหลักฐานใหม่
- ลด bias ของ harness ที่ชอบบังคับ vanilla CSS ทั้งที่โปรเจกต์มี styling system อยู่แล้ว
- ลด UI แนว generic "WOW", gradient/glass เกินจำเป็น, และการสร้าง asset แบบไม่มีเหตุผล
- กัน broken placeholder image path
- กัน SEO/meta/id churn ในทุกหน้าโดยไม่จำเป็น
- กันการบอกว่า verified ทั้งที่ยังไม่มีหลักฐานปัจจุบัน

---

## โครงสร้าง Repo

```text
aileron-protocol/
├── Aileron/
│   ├── lite/GEMINI.md
│   ├── balanced/GEMINI.md
│   ├── studio/GEMINI.md
│   ├── architect/GEMINI.md
│   └── ultimate/GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

---

## วิธีติดตั้ง

### Global Baseline

คัดลอกไฟล์โปรไฟล์ที่ต้องการ แล้วบันทึกเป็น global rules file:

```text
Aileron/<profile>/GEMINI.md -> ~/.gemini/GEMINI.md
```

Windows:

```text
%USERPROFILE%\.gemini\GEMINI.md
```

macOS / Linux:

```text
~/.gemini/GEMINI.md
```

### Workspace Override

ถ้าโปรเจกต์ไหนต้องมีกฎเฉพาะ ให้วาง rules เพิ่มใน workspace นั้น กฎระดับ workspace จะทับ global baseline

วางที่ root:

```text
your-project/
├── GEMINI.md
├── src/
└── package.json
```

หรือวางใน `.agents/rules`:

```text
your-project/
├── .agents/
│   └── rules/
│       └── project-rules.md
├── src/
└── package.json
```

ถ้าใช้ `.agents/rules` ให้ใส่ frontmatter นี้ไว้บนสุด:

```markdown
---
trigger: always_on
---

[rules start here]
```

เว้นบรรทัดว่างหลัง `---` ปิดเสมอ

---

## License

MIT ดูรายละเอียดใน [LICENSE](LICENSE)
