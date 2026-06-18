# Bootstrap 5.3 Teaching Examples

ชุดนี้จัดตามลำดับสไลด์ในโฟลเดอร์ `bootstrap/` เพื่อใช้สอน Bootstrap แบบเป็นเรื่อง ๆ

- ไฟล์ `.html` คือ code demo เปิดใน browser ได้โดยตรง
- โฟลเดอร์ `topics/` คือ code ตัวอย่างแบบละเอียด แยกตามหัวข้อในสไลด์
- ไฟล์ `notes/*.md` คือคู่มือสอนละเอียดสำหรับผู้สอน
- `LABS.md` คือโจทย์ฝึกง่าย-กลางสำหรับผู้เรียน แยกตามหัวข้อ
- `LAB_SOLUTIONS.md` คือเฉลยแนวทางสำหรับโจทย์ฝึก
- `SLIDE_COVERAGE.md` คือแผนที่ว่า slide topic ไหนอยู่ในตัวอย่างไฟล์ใด
- `index.html` คือหน้าเมนูรวมบทเรียนทั้งหมด

## วิธีใช้สอน

1. เปิด `index.html`
2. เลือกบทเรียนตามลำดับ 01-08
3. เปิดไฟล์ notes ของบทนั้นคู่กัน
4. เปิด `topics/index.html` เมื่ออยากสอนแบบลงรายละเอียดตามสไลด์
5. เปิด `LABS.md` เพื่อให้ผู้เรียนทำโจทย์หลังดู demo
6. สอนจาก demo ก่อน แล้วค่อยแก้ code สดตาม Live Coding Flow
7. ใช้แบบฝึกหัดท้าย notes เป็นงานให้นักเรียนทำ

## ลำดับบท

| บท | Code demo | Teaching notes | หัวข้อหลัก |
| --- | --- | --- | --- |
| 01 | `01-essentials-content-utilities.html` | `notes/01-essentials-content-utilities.md` | HTML setup, typography, spacing, colors, utilities |
| 02 | `02-layout-grid-system.html` | `notes/02-layout-grid-system.md` | container, row, columns, breakpoints, gutters |
| 03 | `03-ui-components.html` | `notes/03-ui-components.md` | navbar, alerts, cards, badges, buttons, list group |
| 04 | `04-forms-validation.html` | `notes/04-forms-validation.md` | form controls, layout, validation states |
| 05 | `05-landing-page-workshop.html` | `notes/05-landing-page-workshop.md` | landing page sections, hero, features, pricing |
| 06 | `06-javascript-plugins-part-1.html` | `notes/06-javascript-plugins-part-1.md` | collapse, dropdown, modal, carousel |
| 07 | `07-interactive-ui-advanced-utilities.html` | `notes/07-interactive-ui-advanced-utilities.md` | tabs, accordion, offcanvas, progress, toast |
| 08 | `08-advanced-architecture.html` | `notes/08-advanced-architecture.md` | page shell, app classes, CSS variables, architecture |

## หมายเหตุ

ตัวอย่างใช้ Bootstrap CDN เพื่อให้เปิดไฟล์ HTML ได้ทันที ถ้าจะใช้ใน production ควรติดตั้งผ่าน package manager หรือ build pipeline ของโปรเจกต์จริง
