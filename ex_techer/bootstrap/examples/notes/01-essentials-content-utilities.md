# 01 - Essentials, Content and Utilities

## เป้าหมายบทเรียน

ให้นักเรียนเข้าใจว่า Bootstrap เริ่มจาก 3 อย่างหลัก:

- โครงหน้า HTML ที่ถูกต้อง
- การเรียก Bootstrap CSS ผ่าน CDN
- การใช้ utility classes แทนการเขียน CSS เองในงานพื้นฐาน

## Concept ที่ควรสอน

- `container` ใช้จำกัดความกว้างและจัดกึ่งกลางเนื้อหา
- `py-5`, `p-4`, `mb-3`, `gap-2` คือ spacing utilities
- `display-5`, `lead`, `fw-bold`, `text-secondary` คือ typography utilities
- `bg-light`, `text-bg-dark`, `border`, `rounded-3` คือ visual utilities
- `d-flex`, `flex-wrap`, `gap-*` ใช้จัดปุ่มหรือ action group

## จุดที่ควรชี้ในไฟล์ HTML

- `<meta name="viewport">` จำเป็นสำหรับ responsive layout
- `<link ... bootstrap.min.css>` คือจุดที่ทำให้ class ของ Bootstrap ทำงาน
- Section แรกเป็น hero block ขนาดเล็ก ใช้สอน spacing, typography, buttons
- Cards 3 ใบด้านล่างใช้สอน `row`, `col-md-4`, `h-100`

## Live Coding Flow

1. เปิดไฟล์ `01-essentials-content-utilities.html`
2. ลบ class บางตัว เช่น `container`, `py-5`, `lead` แล้วให้นักเรียนดูผล
3. เปลี่ยน `text-bg-dark` เป็น `text-bg-primary`, `text-bg-success`
4. เปลี่ยน `p-4` เป็น `p-2` และ `p-5` เพื่อให้เห็น scale ของ spacing
5. เพิ่มปุ่มอีก 1 ปุ่มด้วย `btn btn-warning`

## แบบฝึกหัด

- เพิ่ม card ใบที่ 4 โดยให้ responsive เป็น 2 คอลัมน์บน tablet
- เปลี่ยน hero ให้เป็น dark theme โดยใช้ utility classes เท่านั้น
- เพิ่ม badge อีก 2 แบบ เช่น `text-bg-success`, `text-bg-danger`

## คำถามท้ายบท

- ถ้าไม่มี `container` หน้าเว็บจะต่างอย่างไร
- `btn-primary` กับ `btn-outline-primary` ต่างกันตรงไหน
- เมื่อไรควรใช้ utility classes และเมื่อไรควรเขียน CSS เอง
