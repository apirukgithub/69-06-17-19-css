# Bootstrap Practice Labs

โจทย์ฝึกชุดนี้จับคู่กับไฟล์ใน `topics/` มีระดับ Easy, Medium และ Hard เหมาะสำหรับให้ผู้เรียนทำหลังดู demo แต่ละหัวข้อ

## วิธีใช้

1. เปิดไฟล์ demo ใน `topics/`
2. ให้ผู้เรียน copy ไฟล์นั้นเป็นไฟล์ทดลองของตัวเอง หรือแก้บนไฟล์ demo ระหว่างคลาส
3. ทำโจทย์ Easy ก่อน แล้วต่อด้วย Medium
4. ใช้ Hard สำหรับผู้เรียนที่ทำเสร็จเร็วหรือเป็นงานท้ายคาบ
5. ใช้ Check เป็นเกณฑ์ตรวจงานแบบเร็ว

---

## 01 - Essentials, Content and Utilities

### `01-01-display-headings-text-truncation.html`

**Easy:** เพิ่มหัวข้อ `display-6` อีก 1 บรรทัด และเพิ่ม paragraph แบบ `lead`

**Medium:** สร้างกล่องรายการข่าว 3 รายการด้วย `border rounded p-3` โดยให้ชื่อข่าวยาว ๆ ใช้ `text-truncate`

**Hard:** สร้าง news list 5 รายการที่มี title, summary, category label แบบข้อความเล็ก และทุก title ต้อง truncate โดยกล่องแต่ละรายการสูงสม่ำเสมอ

**Check:** ข้อความยาวต้องไม่ล้นกล่อง และ hierarchy ของหัวข้ออ่านง่าย

### `01-02-responsive-images-tables.html`

**Easy:** เพิ่มรูป thumbnail อีก 2 รูปด้วย `img-thumbnail`

**Medium:** เพิ่ม column ใหม่ใน table เช่น `Updated at` แล้วทำให้ table ยัง responsive บนมือถือ

**Hard:** ทำ section inventory ที่มีรูปสินค้า responsive และ table 6 columns พร้อม status text แบบข้อความเล็ก

**Check:** บนจอแคบ table ต้อง scroll แนวนอนได้ ไม่บีบจนอ่านไม่ได้

### `01-03-spacing-flex-alignment.html`

**Easy:** เปลี่ยน spacing จาก `p-3` เป็น `p-4` และเพิ่ม `mb-3`

**Medium:** สร้างแถบ action ที่มี title ซ้าย และข้อความ action 2 ชิ้นอยู่ขวา โดย wrap ได้บนมือถือ

**Hard:** สร้าง responsive action bar ที่ desktop เป็นแนวนอน แต่ mobile แยกเป็น 2 แถวและยัง spacing สวย

**Check:** action items ไม่ชนกัน และ spacing สม่ำเสมอทั้ง desktop/mobile

### `01-04-utility-synthesis-profile-panel.html`

**Easy:** เปลี่ยนชื่อ ตำแหน่ง และ label ข้อความเล็กในกล่อง profile

**Medium:** เพิ่มแถว stats 3 ช่อง เช่น Projects, Rating, Students โดยใช้ `d-flex` หรือ `row`

**Hard:** ทำกล่อง profile 3 ใบใน grid พร้อมรูป, labels, stats และข้อความ action โดยไม่เขียน CSS เพิ่ม

**Check:** กล่อง profile ยังไม่ล้นบนมือถือ และรูป profile ไม่บิดสัดส่วน

---

## 02 - Layout and Grid System

### `02-01-containers-breakpoints.html`

**Easy:** เพิ่ม `container-sm`, `container-md`, `container-lg` เพื่อเทียบความกว้าง

**Medium:** ทำ section ที่มือถือ 1 column, tablet 2 columns, desktop 4 columns

**Hard:** ทำ breakpoint demo page ที่แต่ละ breakpoint เปลี่ยนจำนวนกล่องข้อมูล และแสดง label breakpoint ปัจจุบันด้วย utility classes

**Check:** resize browser แล้ว layout เปลี่ยนตาม breakpoint

### `02-02-grid-math-wrapping-gutters.html`

**Easy:** เปลี่ยน `g-4` เป็น `g-2` และสังเกต gutter

**Medium:** สร้าง layout 3 แถว: `8+4`, `6+6`, `3+3+3+3`

**Hard:** สร้าง dashboard layout ที่มี hero 8+4, KPI 3+3+3+3 และ content 7+5 พร้อม gutters สม่ำเสมอ

**Check:** ผลรวม column ต่อแถวต้องไม่เกิน 12 ยกเว้นตั้งใจให้ wrap

### `02-03-flex-order-stacks-css-grid.html`

**Easy:** สลับ order ของ column บน `md` breakpoint

**Medium:** สร้าง filter chips แบบกล่องข้อความ 3 ชิ้นด้วย `hstack` หรือ `d-flex gap-2`

**Hard:** ทำ responsive toolbar ที่ desktop เรียง title/search/actions แต่ mobile ให้ actions ขึ้นก่อนด้วย order utilities

**Check:** บนมือถือ elements ต้องไม่บีบจนอ่านยาก

### `02-04-master-product-detail-layout.html`

**Easy:** เปลี่ยนชื่อสินค้า ราคา และข้อความสถานะ

**Medium:** เพิ่ม feature 4 จุดใน grid และกล่อง CTA ด้านล่าง

**Hard:** สร้าง product detail layout ที่มี gallery thumbnail, price, feature grid และ CTA โดย layout เปลี่ยนตาม breakpoint

**Check:** layout ต้องเป็น 1 column บนมือถือ และ 2 columns บน desktop

---

## 03 - UI Components

### `03-01-buttons-button-groups.html`

**Easy:** เพิ่มปุ่ม variant `danger`, `warning`, `info`

**Medium:** ทำ segmented control เลือก billing: Monthly / Yearly / Lifetime

**Hard:** ทำ toolbar เลือก view mode 3 แบบและ action 2 ปุ่ม โดยใช้ button groups เท่านั้น

**Check:** active state ต้องชัด และใช้ `btn-check` ถูกต้อง

### `03-02-badges-notification-positioning.html`

**Easy:** เปลี่ยนตัวเลข badge และสี badge

**Medium:** สร้างปุ่ม cart ที่มี badge จำนวนสินค้าอยู่มุมขวาบน

**Hard:** สร้าง notification center 3 ปุ่ม เช่น Inbox, Cart, Alerts พร้อม badge คนละตำแหน่งและสี

**Check:** badge ต้องอยู่ตรงมุม ไม่ดัน layout ปุ่ม

### `03-03-cards-images-overlays-groups.html`

**Easy:** เปลี่ยนภาพและข้อความใน card

**Medium:** ทำ card overlay อีก 1 ใบ พร้อม gradient ด้านล่างเพื่อให้อ่าน text ชัด

**Hard:** ทำ card showcase 3 แบบ: image cap, overlay, horizontal card และให้ responsive สวยทุกจอ

**Check:** ตัวอักษรบนภาพต้องอ่านได้ทั้ง desktop/mobile

### `03-04-grid-cards-equal-height.html`

**Easy:** เพิ่ม card ใบที่ 4

**Medium:** ทำ card grid ที่มือถือ 1, tablet 2, desktop 4 columns

**Hard:** สร้าง pricing grid 4 แผนที่ card สูงเท่ากัน มี badge popular และปุ่มอยู่ล่างสุดทุกใบ

**Check:** card ทุกใบสูงเท่ากัน และ footer อยู่ระดับเดียวกัน

### `03-05-list-groups-interactive.html`

**Easy:** เพิ่ม list item อีก 2 รายการ

**Medium:** สร้าง settings list ที่มีรายการ 3 แถว พร้อม badge แสดงสถานะ เช่น New, Active, Locked

**Hard:** ทำ settings panel แบบ list group ที่มี active item, disabled item, badge status และคำอธิบายย่อยในแต่ละแถว

**Check:** active/disabled state ต้องชัด และ spacing ระหว่าง title/description/badge อ่านง่าย

### `03-06-component-mashup-css-variables.html`

**Easy:** เปลี่ยนสี border ของ card ผ่าน CSS variable

**Medium:** เพิ่ม section stats 2 แถวใน card โดยใช้ `list-group`

**Hard:** ทำ mini dashboard card ที่ใช้ CSS variables เปลี่ยน theme ของ card ได้อย่างน้อย 2 โทน

**Check:** custom CSS ต้องอยู่เฉพาะจุด ไม่เขียนทับ Bootstrap กว้างเกินไป

---

## 04 - Forms and Validation

### `04-01-form-controls-selects.html`

**Easy:** เพิ่ม input เบอร์โทรและ select จังหวัด

**Medium:** จัด form เป็น 2 columns บน desktop และ 1 column บน mobile

**Hard:** สร้าง form สมัครสมาชิก 2 sections: personal info และ preferences โดยใช้ grid และ form controls ครบ

**Check:** label ต้องผูกกับ input ด้วย `for`/`id`

### `04-02-checks-radios-switches.html`

**Easy:** เพิ่ม checkbox อีก 1 รายการ

**Medium:** ทำกลุ่ม radio สำหรับเลือก package 3 แบบ และ switch สำหรับเปิดแจ้งเตือน

**Hard:** ทำ permission form ที่มี checkbox group, radio role, และ switch notifications พร้อมคำอธิบายแต่ละตัวเลือก

**Check:** radio ที่อยู่กลุ่มเดียวกันต้องใช้ `name` เดียวกัน

### `04-03-input-group-range-datalist.html`

**Easy:** เปลี่ยน input group เป็นช่องราคา มี `$` ด้านหน้า

**Medium:** เพิ่ม range สำหรับเลือกจำนวนผู้ใช้ และ datalist สำหรับเลือกเมือง

**Hard:** ทำ pricing calculator form มี input group ราคา, range จำนวนผู้ใช้, datalist เมือง และ summary box

**Check:** input group ต้องไม่แตกเมื่อจอแคบ

### `04-04-floating-labels.html`

**Easy:** เพิ่ม floating input สำหรับ phone

**Medium:** ทำ floating textarea สำหรับ feedback และ floating select สำหรับ department

**Hard:** ทำ contact form ด้วย floating labels ทั้งหมด รวม input, select และ textarea พร้อม layout responsive

**Check:** ทุก input ต้องมี `placeholder` เพื่อให้ floating label ทำงาน

### `04-05-validation-states-feedback.html`

**Easy:** เพิ่ม required field อีก 1 ช่อง

**Medium:** เพิ่ม checkbox terms ที่ต้องติ๊กก่อน submit

**Hard:** เพิ่ม custom validation logic ง่าย ๆ ให้เช็ก password length และ confirm password ตรงกัน

**Check:** submit โดยไม่กรอกต้องเห็น `invalid-feedback`

### `04-06-comprehensive-form.html`

**Easy:** เปลี่ยนชื่อ form เป็น registration สำหรับคอร์สเรียน

**Medium:** เพิ่ม section billing info ด้วย input group และ select

**Hard:** ทำ multi-section checkout form ที่มี contact, billing, package และ terms โดยยังอ่านง่ายบนมือถือ

**Check:** form ต้องยังอ่านง่าย ไม่ยาวเป็นก้อนเดียว

---

## 05 - Landing Page Workshop

### `05-01-landing-page-complete-workshop.html`

**Easy:** เปลี่ยน brand, headline และ service cards

**Medium:** เพิ่ม testimonial section 3 cards ก่อนท้ายหน้า

**Hard:** ต่อยอด landing page ให้มี clients logo strip, FAQ cards แบบ static และ contact form ในหน้าเดียว

**Check:** navbar link ต้อง scroll ไป section ที่ถูกต้อง

### `05-02-breakpoint-checklist.html`

**Easy:** เพิ่ม row ใหม่ใน checklist table

**Medium:** ทำ checklist สำหรับหน้า admin: sidebar, topbar, table, cards

**Hard:** ทำหน้า responsive QA checklist สำหรับตรวจ mobile/tablet/desktop พร้อม badge ผ่าน/ไม่ผ่าน

**Check:** table ต้อง responsive และอ่านได้บนมือถือ

---

## 06 - JavaScript Plugins Part 1

### `06-01-data-attribute-equation.html`

**Easy:** เปลี่ยน collapse target และข้อความใน card

**Medium:** เพิ่ม collapse อีก 2 อันให้เป็น FAQ สั้น ๆ

**Hard:** ทำ FAQ 5 ข้อด้วย collapse โดยปุ่มแต่ละข้อมี icon และ target ไม่ซ้ำกัน

**Check:** ปุ่มต้องเปิด/ปิด target ที่ถูกต้อง

### `06-02-modal-pro-tips.html`

**Easy:** เปลี่ยนข้อความ modal และเพิ่ม footer button

**Medium:** ทำ delete confirmation modal แบบ static backdrop

**Hard:** ทำ modal form สำหรับเพิ่มรายการใหม่ มี header/body/footer และปุ่ม reset/submit

**Check:** ปุ่ม close ต้องปิด modal ได้ และ static backdrop ต้องไม่ปิดเมื่อคลิกข้างนอก

### `06-03-offcanvas-navbar-directions.html`

**Easy:** เปลี่ยน offcanvas start เป็น end

**Medium:** ทำ filter panel ด้วย checkbox 4 ตัวใน offcanvas

**Hard:** ทำ mobile filter offcanvas ที่มี section category, price range และ apply/clear buttons

**Check:** offcanvas ต้องปิดได้และไม่บัง layout หลังปิด

### `06-04-collapse-accordion-dropdowns.html`

**Easy:** เพิ่ม accordion item อีก 1 อัน

**Medium:** เพิ่ม dropdown ที่มี divider และ disabled item

**Hard:** สร้าง help center ที่มี accordion FAQ และ dropdown เลือกหมวดหมู่ในหน้าเดียว

**Check:** accordion ต้องเปิดทีละ item เมื่อใช้ `data-bs-parent`

### `06-05-js-events-lifecycle.html`

**Easy:** เพิ่ม log เมื่อ modal เปิด

**Medium:** เพิ่มปุ่ม clear event log

**Hard:** ทำ event logger ที่บันทึก modal lifecycle พร้อม timestamp และปุ่ม clear log

**Check:** event log ต้องเรียงตามลำดับ show -> shown -> hide -> hidden

---

## 07 - Interactive UI and Advanced Utilities

### `07-01-carousel-autoplay-controls.html`

**Easy:** เพิ่ม slide ที่ 3

**Medium:** เพิ่ม caption และปรับ interval แต่ละ slide ไม่เท่ากัน

**Hard:** สร้าง carousel campaign 4 slides พร้อม caption, indicators, controls และ interval ต่างกัน

**Check:** indicators และ prev/next ต้องทำงานครบทุก slide

### `07-02-alerts-toasts-spinners.html`

**Easy:** เปลี่ยน alert เป็น warning และเพิ่ม dismiss button

**Medium:** ทำ toast แจ้ง “Saved draft” และปุ่ม loading state

**Hard:** ทำ save workflow: กดปุ่มแล้วเปลี่ยนเป็น loading 1 วินาที จากนั้นแสดง toast success

**Check:** toast ต้องแสดงเมื่อกดปุ่ม และ alert ปิดได้

### `07-03-tooltips-popovers.html`

**Easy:** เพิ่ม tooltip อีก 2 ปุ่ม

**Medium:** เพิ่ม popover ที่มี title และ content สำหรับอธิบาย feature

**Hard:** สร้าง toolbar 5 ปุ่มที่มี tooltip ทุกปุ่ม และมี popover สำหรับปุ่ม help

**Check:** tooltip/popover ต้อง initialize ผ่าน JavaScript

### `07-04-z-index-fixed-sticky-object-fit.html`

**Easy:** เปลี่ยนรูป object-fit จาก `cover` เป็น `contain` แล้วเทียบผล

**Medium:** ทำ sticky toolbar พร้อมปุ่ม 2 ปุ่ม

**Hard:** ทำ sticky header + fixed help button + image card ที่ใช้ object-fit โดยไม่ให้ element ทับกัน

**Check:** sticky ต้องไม่ทับ content แบบอ่านไม่ได้

---

## 08 - Advanced Architecture

### `08-01-customization-sass-dark-mode.html`

**Easy:** เปลี่ยนปุ่ม theme switch ให้เปลี่ยนข้อความ Light/Dark

**Medium:** เพิ่ม card ที่สีเปลี่ยนตาม `data-bs-theme`

**Hard:** ทำ theme switch ที่เปลี่ยนทั้งหน้าเป็น light/dark และมี card อย่างน้อย 3 ใบที่อ่านชัดทั้งสองโหมด

**Check:** โหมด dark ต้องไม่ทำให้ text อ่านยาก

### `08-02-accessibility-visually-hidden.html`

**Easy:** เพิ่ม `visually-hidden` text ให้ปุ่ม icon

**Medium:** ทำ search input ที่มี label ซ่อนแต่ screen reader อ่านได้

**Hard:** ทำ icon-only toolbar 4 ปุ่มที่ทุกปุ่มมี accessible name ด้วย visually-hidden หรือ aria-label

**Check:** element ที่ซ่อนต้องยังมีความหมายต่อ accessibility

### `08-03-admin-dashboard-subsystems.html`

**Easy:** เพิ่ม stat card อีก 1 ใบ

**Medium:** เพิ่ม table recent activity 3 rows

**Hard:** ต่อยอด admin dashboard ให้มี sidebar, KPI cards, table และ toast notification เมื่อกดปุ่ม

**Check:** dashboard ต้องยัง responsive และ sidebar ไม่ทำให้ content ล้น

### `08-04-build-tool-matrix-cheatsheet.html`

**Easy:** เพิ่ม row ใหม่ใน build tool matrix

**Medium:** ทำ checklist ก่อน deploy 5 ข้อด้วย list group

**Hard:** ทำ production readiness page มี build matrix, deploy checklist และ accordion อธิบายแต่ละ tool

**Check:** ข้อมูลต้องอ่านง่ายและ table ต้องไม่ล้นจอบนมือถือ
