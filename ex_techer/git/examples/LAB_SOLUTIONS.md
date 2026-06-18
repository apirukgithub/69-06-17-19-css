# Git Practice Lab Solutions

ไฟล์นี้เป็นเฉลยแนวทางสำหรับ `LABS.md` ใช้เป็น hint หรือตรวจงาน ไม่ควรให้ผู้เรียนเปิดก่อนลงมือทำ

## 01 - Git Snapshot Blueprint

### `01-01-config-init-status.html`

**Easy:** ใช้ `git config --global user.name "Name"` และ `git config --global user.email "email@example.com"` แล้วตรวจด้วย `git config --global --list`

**Medium:** ใช้ `mkdir git-lab-01`, `cd git-lab-01`, `git init`, `git status`

**Hard:** สร้างไฟล์ด้วย editor หรือ `echo`, ตรวจด้วย `git status --short`; ควรเห็น `?? README.md` และ `?? notes.txt`

### `01-02-working-staging-repository.html`

**Easy:** `echo "# Lab" > README.md`, `git add README.md`, `git status`

**Medium:** `git commit -m "Add README"` แล้ว `git status` ต้องบอกว่า clean

**Hard:** แก้ไฟล์, `git status`, `git add README.md`, `git commit -m "Update README"`, `git status`

### `01-03-add-commit-file-states.html`

**Easy:** untracked แสดงเป็น `?? file`

**Medium:** staged แสดงเป็น `A  file` หรือเห็นใน section “Changes to be committed”

**Hard:** หลัง commit แล้วแก้ไฟล์เดิม ควรเห็น modified เช่น ` M file`

### `01-04-master-snapshot-workflow.html`

**Easy:** commit แรกควรมี message ชัด เช่น `Add README`

**Medium:** `todo.txt` ควรอยู่ใน commit แยกจาก README

**Hard:** 3 commits ควรเป็นงานเล็กคนละเรื่อง เช่น add readme, add todo, update notes

---

## 02 - Git Inspection Mastery

### `02-01-log-timeline-filtering.html`

**Easy:** `git log --oneline` แสดง commit hash สั้นและ message

**Medium:** `git log --oneline --graph --decorate` ช่วยเห็น timeline และ pointer

**Hard:** ตัวอย่าง filter: `git log --since="1 week ago"`, `git log --author="Name"`, `git log --grep="README"`

### `02-02-commit-anatomy-show.html`

**Easy:** ใช้ hash สั้นจาก `git log --oneline`

**Medium:** `git show <hash>` แสดง metadata และ patch

**Hard:** `--stat` เห็นสรุปจำนวนไฟล์/บรรทัด, `--name-only` เห็นชื่อไฟล์ที่เปลี่ยน

### `02-03-diff-working-index-head.html`

**Easy:** `git diff` แสดง unstaged changes

**Medium:** หลัง `git add`, ใช้ `git diff --staged` เพื่อดู staged changes

**Hard:** `git diff HEAD` รวมความต่างทั้งหมดจาก commit ล่าสุดถึง working tree

### `02-04-compare-commits-branches.html`

**Easy:** `git diff HEAD~1 HEAD` เทียบ commit ล่าสุดกับก่อนหน้า

**Medium:** ใช้ hash จริง เช่น `git diff abc123 def456`

**Hard:** ใช้ `git show` เพื่ออ่าน commit เดี่ยว และ `git diff` เพื่อเทียบสอง commit

### `02-05-inspection-command-matrix.html`

**Easy:** ตัวอย่าง matrix: ดูสถานะ = `git status`, ดู timeline = `git log --oneline`, ดู unstaged = `git diff`

**Medium:** staged ใช้ `git diff --staged`; unstaged ใช้ `git diff`

**Hard:** checklist ควรมี `git status`, `git diff`, `git diff --staged`, `git log --oneline`, `git show <hash>`

---

## 03 - Git Branching and Merging

### `03-01-branch-list-create-delete.html`

**Easy:** `git branch` แสดง branch list และมี `*` ตรง branch ปัจจุบัน

**Medium:** `git branch feature/demo` สร้าง branch แต่ยังไม่สลับไป

**Hard:** ลบ branch ที่ merge แล้วด้วย `git branch -d temp-name`

### `03-02-switch-checkout-feature-lifecycle.html`

**Easy:** `git switch feature/demo` ใช้สลับ branch

**Medium:** `git switch -c feature/page-title` สร้างและสลับในคำสั่งเดียว

**Hard:** lifecycle จบที่กลับมา `main` และ feature branch มี commit ของตัวเอง

### `03-03-merge-fast-forward-three-way.html`

**Easy:** fast-forward คือ main เลื่อน pointer ไปข้างหน้าได้โดยไม่สร้าง merge commit

**Medium:** three-way merge เกิดเมื่อ main และ feature ต่างมี commit ใหม่

**Hard:** timeline ควรแสดง commit ก่อน merge และ commit หลัง merge ให้เห็น pointer ชัด

### `03-04-conflicts-resolution.html`

**Easy:** conflict marker มี `<<<<<<<`, `=======`, `>>>>>>>`

**Medium:** แก้ไฟล์ให้เหลือเนื้อหาสุดท้ายเท่านั้น แล้ว `git add <file>`

**Hard:** commit หลังแก้ conflict แล้ว `git status` ต้อง clean

### `03-05-stash-golden-rules.html`

**Easy:** `git stash` พักงานที่ยังไม่ commit

**Medium:** `git stash list` ดูรายการ stash และ `git stash pop` ดึงกลับ

**Hard:** ใช้ stash ก่อน switch branch เมื่อมีงานค้างที่ยังไม่พร้อม commit

---

## 04 - Git Remotes

### `04-01-local-remote-clone-remote.html`

**Easy:** `git clone <url>` สร้าง local copy จาก remote

**Medium:** `git remote -v` แสดง remote URL สำหรับ fetch/push

**Hard:** `git remote add origin <url>` เพิ่ม remote ชื่อ origin

### `04-02-fetch-pull-difference.html`

**Easy:** fetch โหลดข้อมูล, pull โหลดและรวมเข้า branch

**Medium:** `git fetch origin` ไม่เปลี่ยน working branch ทันที

**Hard:** หลัง fetch ให้ตรวจด้วย `git log HEAD..origin/main --oneline` ก่อนตัดสินใจรวม

### `04-03-push-origin-main.html`

**Easy:** `origin` คือ remote, `main` คือ branch

**Medium:** `git push origin main` ส่ง commit local branch ไป remote branch

**Hard:** `git push -u origin feature/demo` ตั้ง upstream เพื่อ push/pull ครั้งต่อไปสั้นลง

### `04-04-team-collaboration-loop.html`

**Easy:** loop พื้นฐาน: update -> branch -> commit -> push

**Medium:** feature branch workflow ควร push branch แยก ไม่ push main ตรงถ้าเป็นงานทีม

**Hard:** checklist ก่อน PR ควรมี status clean, log อ่านได้, fetch ล่าสุด, branch pushed, และ summary ชัดเจน

