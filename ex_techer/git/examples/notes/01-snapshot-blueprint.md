# 01 - Git Snapshot Blueprint

## เป้าหมาย

ให้นักเรียนเข้าใจว่า Git ไม่ใช่ระบบ save ทับไฟล์ แต่เป็นระบบ snapshot ที่มี Working Directory, Staging Area และ Repository

## Flow การสอน

1. เริ่มจาก `git config`
2. สร้าง repo ด้วย `git init`
3. สร้างไฟล์ใหม่แล้วอ่าน `git status`
4. ใช้ `git add` เพื่อย้ายไป staging
5. ใช้ `git commit` เพื่อสร้าง snapshot
6. สรุป workflow: edit -> status -> add -> commit -> status

## Lab ที่ใช้

- `topics/01-01-config-init-status.html`
- `topics/01-02-working-staging-repository.html`
- `topics/01-03-add-commit-file-states.html`
- `topics/01-04-master-snapshot-workflow.html`
