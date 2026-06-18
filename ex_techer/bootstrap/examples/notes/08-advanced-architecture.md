# 08 - Advanced Architecture

## เป้าหมายบทเรียน

ให้นักเรียนเข้าใจวิธีใช้ Bootstrap ในโปรเจกต์จริง โดยแยกหน้าที่ระหว่าง utility classes, components และ custom CSS

## Concept ที่ควรสอน

- Page shell
- Sidebar layout
- Custom CSS variables
- App-specific class prefix
- Component reuse
- การไม่เขียน CSS ทับ Bootstrap โดยไม่จำเป็น

## จุดที่ควรชี้ในไฟล์ HTML

- `:root` เก็บ design tokens เช่น `--app-accent`
- `.app-shell`, `.app-sidebar`, `.app-stat` เป็น class ของ app เอง
- ใช้ Bootstrap utilities สำหรับ spacing/layout ที่ไม่ซับซ้อน
- ใช้ custom CSS เฉพาะส่วนที่เป็น architecture หรือ theme

## Live Coding Flow

1. เปลี่ยน `--app-accent` แล้วดู stat border เปลี่ยนทั้งระบบ
2. เปลี่ยน sidebar width จาก 280px เป็น 320px
3. เพิ่ม nav item ใหม่
4. เพิ่ม stat card ใบที่ 4 แล้วปรับ grid
5. แยก section ใหม่สำหรับ table หรือ recent activity

## แบบฝึกหัด

- เพิ่ม dashboard table ด้วย `table table-hover`
- เพิ่ม light/dark theme switch แบบง่ายด้วย CSS variables
- สร้าง reusable card pattern สำหรับ KPI

## คำถามท้ายบท

- เมื่อไรควรเขียน custom CSS
- ทำไมควร prefix class ของ app เช่น `app-*`
- Design token ช่วยให้ maintain ง่ายขึ้นอย่างไร
