# 02 - Layout and Grid System

## เป้าหมายบทเรียน

ให้นักเรียนเข้าใจระบบ 12 columns ของ Bootstrap และสามารถออกแบบ layout ที่เปลี่ยนตามขนาดหน้าจอได้

## Concept ที่ควรสอน

- `container` และ `container-fluid`
- `row` เป็น wrapper ของ columns
- `col-12`, `col-md-8`, `col-md-4` คือ responsive columns
- `row-cols-*` ใช้กำหนดจำนวนคอลัมน์แบบรวดเร็ว
- `g-3`, `gx-*`, `gy-*` ใช้จัดช่องว่างระหว่าง columns

## จุดที่ควรชี้ในไฟล์ HTML

- Main content ใช้ `col-12 col-md-8`: มือถือเต็มแถว, desktop กว้าง 8/12
- Sidebar ใช้ `col-12 col-md-4`: มือถืออยู่แถวใหม่, desktop อยู่ข้างกัน
- Feature grid ใช้ `row-cols-1 row-cols-sm-2 row-cols-lg-4`

## Live Coding Flow

1. เปลี่ยน `col-md-8` เป็น `col-lg-8` แล้ว resize browser
2. เปลี่ยน `row-cols-lg-4` เป็น `row-cols-lg-3`
3. เพิ่ม `g-5` เพื่อให้เห็นผลของ gutters
4. เพิ่ม column ใหม่แล้วดูว่า layout wrap อย่างไร
5. ทดลองใช้ `order-md-2` กับ sidebar

## แบบฝึกหัด

- สร้าง layout dashboard: sidebar 3 columns, content 9 columns
- ทำ card grid ที่มือถือ 1 คอลัมน์, tablet 2 คอลัมน์, desktop 3 คอลัมน์
- เพิ่ม nested row ภายใน main content

## คำถามท้ายบท

- ทำไมต้องวาง `.col-*` ไว้ใน `.row`
- `col-md-6` แปลว่าอะไร
- `row-cols-*` เหมาะกับ use case แบบไหน
