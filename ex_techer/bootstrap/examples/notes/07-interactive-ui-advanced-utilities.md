# 07 - Interactive UI and Advanced Utilities

## เป้าหมายบทเรียน

ให้นักเรียนสร้าง UI ที่โต้ตอบได้มากขึ้น และใช้ utilities ขั้นสูงในการควบคุม layout/state

## Plugin และ Utilities ในตัวอย่าง

- Tabs
- Accordion
- Offcanvas
- Progress
- Toast
- `position-fixed`, `bottom-0`, `end-0`
- `justify-content-between`, `align-items-center`

## จุดที่ควรชี้ในไฟล์ HTML

- Tabs ใช้ `data-bs-toggle="tab"` และ `data-bs-target`
- Accordion ใช้ `data-bs-parent` เพื่อให้เปิดทีละ item
- Offcanvas เหมาะกับ filter/sidebar บน mobile
- Toast ต้องเรียกด้วย JavaScript เล็กน้อย

## Live Coding Flow

1. เพิ่ม tab ใหม่ชื่อ Reports
2. เพิ่ม accordion item ที่ 2
3. เปลี่ยน offcanvas จาก `offcanvas-end` เป็น `offcanvas-start`
4. เปลี่ยน progress จาก 70% เป็นค่าอื่น
5. แก้ข้อความใน toast และลองกดแสดงผล

## แบบฝึกหัด

- ทำหน้า dashboard ที่มี filter offcanvas
- ทำ onboarding checklist ด้วย accordion
- ทำ save notification ด้วย toast

## คำถามท้ายบท

- Tabs เหมาะกับข้อมูลแบบไหน
- Offcanvas ต่างจาก modal อย่างไร
- Toast ควรใช้แทน alert หรือไม่
