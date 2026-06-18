# 04 - Forms and Validation

## เป้าหมายบทเรียน

ให้นักเรียนสร้าง form ที่อ่านง่าย ใช้งานได้จริง และมี validation state แบบ Bootstrap

## Concept ที่ควรสอน

- `form-label`, `form-control`, `form-select`
- Grid ใน form ด้วย `row g-3`
- Required fields ด้วย HTML validation
- `invalid-feedback`
- `needs-validation` และ `was-validated`

## จุดที่ควรชี้ในไฟล์ HTML

- `novalidate` ปิด default browser tooltip เพื่อใช้ Bootstrap style
- `required` ทำให้ field ต้องกรอก
- `type="email"` ช่วย validate รูปแบบ email
- Script ท้ายไฟล์เพิ่ม class `was-validated` หลัง submit

## Live Coding Flow

1. กด submit โดยไม่กรอกข้อมูลเพื่อดู invalid state
2. กรอก email ผิดรูปแบบแล้ว submit
3. เพิ่ม field phone number
4. เพิ่ม checkbox ยอมรับเงื่อนไข
5. เปลี่ยน form จาก single column เป็น two columns

## แบบฝึกหัด

- เพิ่ม input group สำหรับ URL หรือ price
- เพิ่ม radio buttons สำหรับ package
- เพิ่ม success message หลัง validate ผ่าน

## คำถามท้ายบท

- `novalidate` มีไว้ทำไม
- `invalid-feedback` จะโชว์เมื่อไร
- Bootstrap validation แทน server validation ได้ไหม
