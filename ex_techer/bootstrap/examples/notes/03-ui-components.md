# 03 - UI Components

## เป้าหมายบทเรียน

ให้นักเรียนรู้จัก Bootstrap components ที่ใช้บ่อย และเข้าใจ pattern การประกอบ UI จาก component มาตรฐาน

## Component ในตัวอย่าง

- Navbar
- Alert
- Card
- Badge
- Button
- List group

## จุดที่ควรชี้ในไฟล์ HTML

- Navbar ใช้ `navbar`, `navbar-expand-lg`, `navbar-dark`, `bg-dark`
- Alert ต้องมี `role="alert"` เพื่อ accessibility
- Card แยกเป็น `card`, `card-body`, `card-title`, `card-text`
- List group ใช้ได้ทั้ง `<a>`, `<button>`, หรือ item ธรรมดา

## Live Coding Flow

1. เปลี่ยน navbar จาก dark เป็น light
2. เปลี่ยน alert จาก `alert-info` เป็น `alert-warning`
3. เพิ่ม card อีกใบและใช้ `badge text-bg-danger`
4. เปลี่ยนปุ่ม card เป็น `btn-primary`, `btn-outline-primary`, `btn-success`
5. เพิ่ม active state ใน list group item อื่น

## แบบฝึกหัด

- สร้าง pricing card 3 แผน
- เพิ่ม alert สำหรับ success, warning, danger
- ทำ list group เป็นเมนู settings

## คำถามท้ายบท

- Component ต่างจาก utility class อย่างไร
- ทำไม card ต้องมี `card-body`
- `active` state ควรใช้เมื่อไร
