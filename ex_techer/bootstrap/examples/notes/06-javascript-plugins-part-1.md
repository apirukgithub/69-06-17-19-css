# 06 - JavaScript Plugins Part 1

## เป้าหมายบทเรียน

ให้นักเรียนใช้ Bootstrap JavaScript plugins ผ่าน `data-bs-*` attributes และรู้ว่าเมื่อไรต้องโหลด `bootstrap.bundle.min.js`

## Plugin ในตัวอย่าง

- Collapse
- Dropdown
- Modal
- Carousel

## จุดที่ควรชี้ในไฟล์ HTML

- ต้องมี `<script src="...bootstrap.bundle.min.js"></script>`
- `data-bs-toggle` ระบุ plugin ที่ต้องการเปิด
- `data-bs-target` ชี้ไปยัง element เป้าหมาย
- Modal ต้องมีโครงสร้าง `modal`, `modal-dialog`, `modal-content`
- Carousel ต้องมี `carousel-inner` และ `carousel-item active`

## Live Coding Flow

1. ลบ script bundle แล้วให้ดูว่า plugin ไม่ทำงาน
2. เปลี่ยน target ของ collapse ให้ผิด แล้วดูผล
3. เพิ่ม item ใน dropdown
4. เพิ่มปุ่ม confirm ใน modal footer
5. เพิ่ม carousel item ที่ 3

## แบบฝึกหัด

- ทำ FAQ ด้วย collapse
- ทำ modal สำหรับ delete confirmation
- ทำ image carousel 3 slides

## คำถามท้ายบท

- `data-bs-toggle` กับ `data-bs-target` ทำหน้าที่อะไร
- ทำไมต้องใช้ bundle version
- Modal เหมาะกับงานแบบไหน และไม่เหมาะกับงานแบบไหน
