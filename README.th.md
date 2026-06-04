<a id="readme-top"></a>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&color=0:F87171,100:FCD34D&height=220&section=header&text=Aileron%20Protocol&fontSize=70&fontAlignY=50&fontColor=FFF7ED" width="100%" alt="Aileron Protocol Banner" />
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Inter&size=20&pause=1000&color=e2c08a&center=true&vCenter=true&width=700&lines=%E0%B8%84%E0%B8%A7%E0%B8%9A%E0%B8%84%E0%B8%B8%E0%B8%A1+AI+Agent+%E0%B9%84%E0%B8%94%E0%B9%89%E0%B8%A1%E0%B8%B5%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%AA%E0%B8%B4%E0%B8%97%E0%B8%98%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%9E%E0%B8%A2%E0%B8%B4%E0%B9%88%E0%B8%87%E0%B8%82%E0%B8%B6%E0%B9%89%E0%B8%99;%E0%B8%AB%E0%B8%A2%E0%B8%B8%E0%B8%94%E0%B8%A7%E0%B8%87%E0%B8%88%E0%B8%A3%E0%B9%81%E0%B8%81%E0%B9%89%E0%B8%9A%E0%B8%B1%E0%B9%8A%E0%B8%81%E0%B8%8B%E0%B9%89%E0%B8%B3%E0%B8%8B%E0%B8%B2%E0%B8%81;%E0%B8%A5%E0%B8%94%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%AD%E0%B9%88%E0%B8%B2%E0%B8%99%E0%B9%84%E0%B8%9F%E0%B8%A5%E0%B9%8C%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%84%E0%B8%A1%E0%B9%88%E0%B8%88%E0%B8%B3%E0%B9%80%E0%B8%9B%E0%B9%87%E0%B8%99;%E0%B9%80%E0%B8%A5%E0%B8%B4%E0%B8%81%E0%B8%A7%E0%B8%B2%E0%B8%87%E0%B9%81%E0%B8%9C%E0%B8%99%E0%B8%A2%E0%B8%B7%E0%B8%94%E0%B9%80%E0%B8%A2%E0%B8%B7%E0%B9%89%E0%B8%AD%E0%B8%AA%E0%B8%B3%E0%B8%AB%E0%B8%A3%E0%B8%B1%E0%B8%9A%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B8%87%E0%B9%88%E0%B8%B2%E0%B8%A2%E0%B9%86" alt="Typing SVG" />
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

## ทำไมต้อง Aileron?

หงุดหงิดกับการ vibe coding บน Antigravity อยู่ใช่ไหม? Agent อ่าน context ทั้งโปรเจกต์ทั้งที่แก้แค่บรรทัดเดียว วางแผนยาวเหยียดสำหรับงานง่ายๆ ติดลูปวนแก้บั๊กเดิมซ้ำจนหมดเวลา ทำให้เสีย Token ไปเปล่าๆ

<br />

**Aileron Protocol** คือ `GEMINI.md` สำเร็จรูปที่วางลง project หรือ global config ได้เลย คุม behavior ของ agent ให้ plan น้อยลง อ่านน้อยลง และไม่วน debug loop

<br />

| พฤติกรรม | Default Harness | ติดตั้ง Aileron แล้ว |
| :--- | :--- | :--- |
| **การวางแผน** | บังคับสร้าง plan ทุกงาน แม้แค่แก้โค้ดบรรทัดเดียว | ข้าม plan งานทั่วไป วางแผนเฉพาะงานที่กระทบ structure หลัก |
| **การอ่านไฟล์** | อ่านไฟล์กว้างเกินจำเป็นจน context บวมเสีย token | อ่านเฉพาะไฟล์ที่เกี่ยวก่อน ไม่กวาดอ่านทั้ง repo |
| **การ debug** | วน retry วิธีเดิมซ้ำจนโควตาหมดหรือ timeout | fix พลาด 2 รอบติดกัน หยุดและแจ้ง user ทันที |
| **Safety** | แก้ shared file โดยไม่เช็คผลกระทบ | เช็ค caller ก่อนแก้ shared API ทุกครั้ง |
| **ดีไซน์ UI** | สาดสีสุ่มไล่เฉดรกสายตาสไตล์ AI Slop | บล็อก effect รกสายตา คุม color strategy อย่างเป็นระบบ |

> [!NOTE]
> ใช้ได้กับทุก model บน Antigravity 2.0 แนะนำ Gemini 3.5 Flash สำหรับ speed กับ quality ที่สมดุล

<p align="right">(<a href="#readme-top">กลับสู่ด้านบน</a>)</p>

## โครงสร้างโปรเจกต์

```text
aileron-protocol/
├── Aileron/
│   └── GEMINI.md
├── README.md
├── README.th.md
└── LICENSE
```

## การติดตั้ง

เลือก deploy ได้ 2 แบบ — **Global** ใช้กับทุก project ในเครื่อง หรือ **Workspace** จำกัดเฉพาะ project นั้น

### Global

Copy `GEMINI.md` ไปวางที่
* **Windows:** `%USERPROFILE%\.gemini\GEMINI.md`
* **macOS / Linux:** `~/.gemini/GEMINI.md`

### Workspace

นำ `GEMINI.md` ไปวางใน project ที่ต้องการ เลือกได้ 2 วิธี
* **วิธี A:** วางที่ root ของ project ตรงๆ
* **วิธี B:** วางใน path อื่น เช่น `.agents/rules/project-rules.md` ก็ได้

> [!IMPORTANT]
> ถ้าเลือกวิธี B ต้องใส่ trigger header ไว้บนสุดของไฟล์ และเว้น 1 บรรทัดหลัง `---`
> ```markdown
> ---
> trigger: always_on
> ---
>
> [Rules start here...]
> ```

<p align="right">(<a href="#readme-top">กลับสู่ด้านบน</a>)</p>

## ลิขสิทธิ์การใช้งาน

เผยแพร่ภายใต้ **CC BY-NC-SA 4.0** ดูรายละเอียดที่ [LICENSE](LICENSE)
