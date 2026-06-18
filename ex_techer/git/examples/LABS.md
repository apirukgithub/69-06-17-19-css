# Git Practice Labs

โจทย์ฝึกชุดนี้จับคู่กับไฟล์ใน `topics/` มีระดับ Easy, Medium และ Hard โดยคุมลำดับบทเรียนไม่ให้ใช้คำสั่งที่ยังไม่เรียน

## วิธีใช้

1. สร้างโฟลเดอร์ทดลองใหม่ทุกครั้ง อย่าทำใน repository งานจริง
2. เปิด demo ใน `topics/`
3. ทำ Easy ก่อน ต่อด้วย Medium
4. ใช้ Hard เป็นงานท้ายคาบหรือสำหรับผู้เรียนที่ทำเร็ว
5. ใช้ Check ตรวจผลด้วยคำสั่งที่เรียนมาแล้วเท่านั้น

---

## 01 - Git Snapshot Blueprint

### `01-01-config-init-status.html`

**Easy:** ตั้งค่า `user.name` และ `user.email` แบบ global แล้วตรวจค่าที่ตั้งไว้

**Medium:** สร้างโฟลเดอร์ `git-lab-01`, รัน `git init`, แล้วใช้ `git status` ตรวจสถานะเริ่มต้น

**Hard:** สร้างไฟล์ `README.md` และ `notes.txt` แล้วใช้ `git status --short` อ่านสถานะของไฟล์ทั้งสอง

**Check:** ยังไม่ต้อง commit แต่ต้องอธิบายได้ว่าไฟล์อยู่ในสถานะ untracked

### `01-02-working-staging-repository.html`

**Easy:** สร้างไฟล์ `README.md`, ใช้ `git add`, แล้วดูสถานะก่อน commit

**Medium:** commit ไฟล์แรกด้วยข้อความ `Add README` แล้วใช้ `git status` ตรวจว่า working tree clean

**Hard:** แก้ไฟล์เดิม 1 ครั้ง แล้วทำ flow ครบ: status -> add -> commit -> status

**Check:** ใช้ได้เฉพาะ `git status`, `git add`, `git commit`

### `01-03-add-commit-file-states.html`

**Easy:** สร้างไฟล์ใหม่ 1 ไฟล์แล้วดูสถานะ untracked

**Medium:** add ไฟล์ แล้วดูสถานะ staged ด้วย `git status --short`

**Hard:** commit ไฟล์ จากนั้นแก้ไฟล์เดิมอีกครั้งเพื่อให้เห็นสถานะ modified

**Check:** ผู้เรียนต้องบอกได้ว่า untracked, staged, modified ต่างกันอย่างไร

### `01-04-master-snapshot-workflow.html`

**Easy:** ทำ commit แรกสำหรับ `README.md`

**Medium:** เพิ่มไฟล์ `todo.txt` แล้ว commit ด้วย message ที่อธิบายงานชัดเจน

**Hard:** ทำ 3 commits เล็ก ๆ โดยแต่ละ commit เปลี่ยนงานคนละเรื่อง

**Check:** หลังจบงาน `git status` ต้อง clean

---

## 02 - Git Inspection Mastery

### `02-01-log-timeline-filtering.html`

**Easy:** ใช้ `git log --oneline` ดูประวัติ commit

**Medium:** ใช้ `git log --oneline --graph --decorate` เพื่อดู timeline แบบอ่านง่าย

**Hard:** ใช้ filter เช่น `--since`, `--author`, หรือ `--grep` กับ repo ที่มีหลาย commit

**Check:** ใช้เฉพาะคำสั่งตรวจ history ที่เรียนในบทนี้

### `02-02-commit-anatomy-show.html`

**Easy:** เลือก commit hash จาก `git log --oneline`

**Medium:** ใช้ `git show <hash>` อ่านรายละเอียด commit

**Hard:** ใช้ `git show --stat <hash>` และ `git show --name-only <hash>` เปรียบเทียบผล

**Check:** ต้องอธิบายได้ว่า hash, author, date, message และ patch อยู่ตรงไหน

### `02-03-diff-working-index-head.html`

**Easy:** แก้ไฟล์ที่ commit แล้ว แล้วใช้ `git diff`

**Medium:** ใช้ `git add` แล้วตรวจสิ่งที่ staged ด้วย `git diff --staged`

**Hard:** มีทั้ง staged change และ unstaged change ในไฟล์เดียว แล้วใช้ `git diff`, `git diff --staged`, `git diff HEAD` เทียบกัน

**Check:** ต้องบอกได้ว่าแต่ละ diff เปรียบเทียบพื้นที่ไหน

### `02-04-compare-commits-branches.html`

**Easy:** เปรียบเทียบ commit ล่าสุดกับก่อนหน้าโดยใช้ `git diff HEAD~1 HEAD`

**Medium:** ใช้ `git log --oneline` หา commit 2 ตัว แล้วใช้ `git diff <old> <new>`

**Hard:** ใช้ `git show <hash>` ร่วมกับ `git diff <hash1> <hash2>` เพื่ออธิบายการเปลี่ยนแปลงเป็นลำดับ

**Check:** ใช้เฉพาะ commit ที่มีอยู่เพื่อฝึกเปรียบเทียบ

### `02-05-inspection-command-matrix.html`

**Easy:** เติมตาราง command matrix ของตัวเอง 3 สถานการณ์

**Medium:** จำลองสถานการณ์ staged/unstaged แล้วเลือกคำสั่งตรวจสอบให้ถูก

**Hard:** เขียน checklist ก่อน commit 5 ข้อ โดยใช้เฉพาะ `status`, `log`, `diff`, `show`

**Check:** ทุกคำสั่งต้องเป็นกลุ่ม inspection เท่านั้น

---

## 03 - Git Branching and Merging

### `03-01-branch-list-create-delete.html`

**Easy:** ใช้ `git branch` ดู branch ปัจจุบัน

**Medium:** สร้าง branch ใหม่ด้วย `git branch feature/demo`

**Hard:** สร้าง branch ชั่วคราว แล้วลบด้วย `git branch -d` หลังไม่ใช้งาน

**Check:** ใช้เฉพาะคำสั่งจัดการ branch ในเครื่องเท่านั้น

### `03-02-switch-checkout-feature-lifecycle.html`

**Easy:** สลับไป branch ใหม่ด้วย `git switch`

**Medium:** ใช้ `git switch -c feature/page-title`, แก้ไฟล์, add และ commit

**Hard:** ทำ feature lifecycle ครบ: main -> create branch -> work -> commit -> switch main

**Check:** ต้องอธิบายได้ว่า `git switch` ต่างจาก `git branch` อย่างไร

### `03-03-merge-fast-forward-three-way.html`

**Easy:** merge feature branch ที่ main ยังไม่มี commit ใหม่ เพื่อดู fast-forward

**Medium:** สร้างสถานการณ์ที่ main และ feature มี commit แยกกัน แล้ว merge ให้เกิด merge commit

**Hard:** วาดหรือเขียน timeline ก่อน/หลัง merge ด้วย commit id สั้น ๆ

**Check:** ต้องบอกได้ว่า fast-forward กับ three-way merge ต่างกันตรงไหน

### `03-04-conflicts-resolution.html`

**Easy:** สร้าง conflict ง่าย ๆ โดยแก้บรรทัดเดียวกันใน 2 branch

**Medium:** เปิดไฟล์ conflict แล้วลบ marker `<<<<<<<`, `=======`, `>>>>>>>`

**Hard:** แก้ conflict ให้รวมเนื้อหาจากทั้งสอง branch แล้ว commit ผลลัพธ์

**Check:** หลังแก้ conflict ต้อง `git status` clean

### `03-05-stash-golden-rules.html`

**Easy:** แก้ไฟล์โดยยังไม่ commit แล้วใช้ `git stash`

**Medium:** ใช้ `git stash list` และ `git stash pop`

**Hard:** ฝึกสถานการณ์ต้องสลับ branch แต่มีงานค้าง ใช้ stash เพื่อพักงานแล้วกลับมาทำต่อ

**Check:** ต้องรู้ว่า stash ไม่ใช่ commit ถาวร

---

## 04 - Git Remotes

### `04-01-local-remote-clone-remote.html`

**Easy:** clone repository ทดลอง หรืออธิบายคำสั่ง `git clone <url>`

**Medium:** ใช้ `git remote -v` ดู remote ที่ผูกอยู่

**Hard:** เพิ่ม remote ใหม่ใน repo ทดลองด้วย `git remote add origin <url>` แล้วตรวจด้วย `git remote -v`

**Check:** ต้องบอกได้ว่า `origin` เป็นชื่อเล่นของ remote

### `04-02-fetch-pull-difference.html`

**Easy:** อธิบายความต่างของ `git fetch` กับ `git pull`

**Medium:** ใช้ `git fetch origin` แล้วตรวจว่าข้อมูลถูกโหลดมาแต่ยังไม่รวมเข้า working branch

**Hard:** ใช้ `git fetch` ก่อน แล้วค่อยตัดสินใจว่าจะ merge/pull หรือยัง

**Check:** ต้องอธิบายได้ว่า pull = fetch + integrate

### `04-03-push-origin-main.html`

**Easy:** อธิบายโครงสร้างคำสั่ง `git push origin main`

**Medium:** push branch ปัจจุบันขึ้น remote ทดลอง

**Hard:** ใช้ `git push -u origin feature/demo` แล้วอธิบาย upstream tracking

**Check:** ต้องรู้ว่า push ส่ง commit จาก local ไป remote

### `04-04-team-collaboration-loop.html`

**Easy:** เขียน daily loop ของตัวเอง: pull/fetch -> branch -> commit -> push

**Medium:** จำลอง feature branch workflow แล้ว push branch ขึ้น remote ทดลอง

**Hard:** เขียน checklist ก่อนเปิด pull request 5 ข้อ เช่น status clean, log อ่านง่าย, fetch ล่าสุด, push branch, อธิบาย change

**Check:** workflow ต้องลดโอกาสชนงานคนอื่น ไม่ใช่แค่ push ให้จบ
