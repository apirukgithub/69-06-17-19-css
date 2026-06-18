# Bootstrap Practice Lab Solutions

ไฟล์นี้เป็นเฉลยแนวทางสำหรับ `LABS.md` ใช้ตรวจงานหรือใช้เป็น hint ระหว่างสอน ไม่ได้ตั้งใจให้ copy ทั้งหมดแทนการฝึกทำ

## วิธีใช้

- ให้ผู้เรียนทำจาก `LABS.md` ก่อน
- เปิดเฉลยนี้เมื่อผู้เรียนติด หรือใช้ตรวจหลังส่งงาน
- เฉลยเน้น class/pattern ที่ควรใช้ ไม่จำเป็นต้องเหมือนทุกตัวอักษร

---

## 01 - Essentials, Content and Utilities

### `01-01-display-headings-text-truncation.html`

**Easy:** ใช้ `h2.display-6` และ `p.lead.text-secondary`

**Medium:** ใช้ `row g-3`; แต่ละรายการเป็น `div.border.rounded.p-3.h-100` และ title ใช้ `class="text-truncate"`

**Hard:** ใช้ `row row-cols-1 row-cols-md-2 row-cols-lg-3 g-3`; แต่ละข่าวมี label เป็น `small text-uppercase text-secondary`, `h3.text-truncate`, `p.text-secondary`

### `01-02-responsive-images-tables.html`

**Easy:** เพิ่ม `<img class="img-thumbnail">` หรือ `<img class="img-fluid rounded">` และกำหนดความกว้างด้วย utility หรือ inline width แบบง่าย

**Medium:** เพิ่ม `<th>Updated at</th>` และ `<td>...</td>` โดยยังครอบ table ด้วย `.table-responsive`

**Hard:** ใช้ layout `row g-4`; ซ้ายเป็น product image ด้วย `.img-fluid`, ขวาเป็น `.table-responsive > table.table.table-striped`

### `01-03-spacing-flex-alignment.html`

**Easy:** เปลี่ยน utility เป็น `p-4 mb-3`

**Medium:** ใช้ `d-flex flex-column flex-md-row justify-content-between align-items-md-center gap-3`

**Hard:** ใช้ toolbar 2 ชั้น: ชั้น title/search และชั้น actions โดยใช้ `flex-wrap`, `gap-2`, `ms-md-auto`

### `01-04-utility-synthesis-profile-panel.html`

**Easy:** แก้ text และ label ด้วย `small text-secondary`

**Medium:** ใช้ `row row-cols-3 g-2` หรือ `d-flex justify-content-between` สำหรับ stats 3 ช่อง

**Hard:** ใช้ `row row-cols-1 row-cols-md-3 g-3`; กล่องแต่ละใบใช้ `border rounded p-3 h-100`, `rounded-circle`, `small text-secondary`, `d-flex gap-2`

---

## 02 - Layout and Grid System

### `02-01-containers-breakpoints.html`

**Easy:** เพิ่ม block `.container-sm`, `.container-md`, `.container-lg`

**Medium:** ใช้ `row row-cols-1 row-cols-md-2 row-cols-lg-4 g-3`

**Hard:** ใช้ grid ของกล่องข้อมูล พร้อม label เช่น `d-none d-md-inline` เพื่อแสดง breakpoint-specific text

### `02-02-grid-math-wrapping-gutters.html`

**Easy:** เปลี่ยน `g-4` เป็น `g-2`

**Medium:** สร้าง `row g-3` หลายแถวด้วย `col-lg-8`, `col-lg-4`, `col-md-6`, `col-lg-3`

**Hard:** ใช้ sections แยก: hero `8+4`, KPI `row-cols-lg-4`, content `col-lg-7` และ `col-lg-5`

### `02-03-flex-order-stacks-css-grid.html`

**Easy:** ใช้ `order-md-1`, `order-md-2`

**Medium:** ใช้ `<div class="hstack gap-2 flex-wrap">` และทำ filter chips ด้วย `span.border.rounded-pill.px-3.py-2`

**Hard:** ใช้ `order-1 order-md-2`, `order-2 order-md-1` และ `flex-column flex-lg-row`

### `02-04-master-product-detail-layout.html`

**Easy:** แก้ headline, price และ status text

**Medium:** เพิ่ม `row row-cols-2 row-cols-md-4 g-2` สำหรับ feature tiles และเพิ่มกล่อง CTA ด้วย `border rounded p-3`

**Hard:** ใช้ `row g-4 align-items-center`; ซ้าย gallery, ขวารายละเอียดสินค้า, CTA ด้วย `d-flex gap-2 flex-wrap`

---

## 03 - UI Components

### `03-01-buttons-button-groups.html`

**Easy:** เพิ่ม `btn-danger`, `btn-warning`, `btn-info`

**Medium:** ใช้ `btn-check` + `label.btn.btn-outline-dark` และ `name` เดียวกัน

**Hard:** ใช้ `btn-group` 2 ชุดใน `d-flex gap-2 flex-wrap` และปุ่ม primary action 1 ปุ่ม

### `03-02-badges-notification-positioning.html`

**Easy:** แก้ text และ class เช่น `bg-warning`, `bg-success`

**Medium:** ใช้ parent `position-relative` และ badge `position-absolute top-0 start-100 translate-middle`

**Hard:** ทำ 3 ปุ่มใน `d-flex gap-3`; badge แต่ละปุ่มใช้ตำแหน่ง/สีต่างกัน

### `03-03-cards-images-overlays-groups.html`

**Easy:** เปลี่ยน `src`, `alt`, title, text

**Medium:** ใช้ `card-img-overlay` และ inline/background gradient overlay

**Hard:** ทำ 3 card: `card-img-top`, `card-img-overlay`, และ horizontal card ด้วย `row g-0`

### `03-04-grid-cards-equal-height.html`

**Easy:** เพิ่ม `.col` อีกใบ

**Medium:** ใช้ `row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4`

**Hard:** pricing card ใช้ `card h-100`, `card-body`, `card-footer bg-transparent mt-auto`

### `03-05-list-groups-interactive.html`

**Easy:** เพิ่ม `.list-group-item`

**Medium:** ใช้ `.list-group-item d-flex justify-content-between align-items-center` พร้อม `badge`

**Hard:** ใช้ `.list-group-item.active`, `.list-group-item.disabled`, `badge`, และ `small text-secondary` สำหรับคำอธิบายย่อย

### `03-06-component-mashup-css-variables.html`

**Easy:** แก้ `--bs-card-border-color`

**Medium:** เพิ่ม `list-group list-group-flush` เป็น stats rows

**Hard:** ทำ class theme เช่น `.theme-blue`, `.theme-pink` ที่ set CSS variables เฉพาะ card

---

## 04 - Forms and Validation

### `04-01-form-controls-selects.html`

**Easy:** เพิ่ม `input.form-control` และ `select.form-select`

**Medium:** ใช้ `row g-3`, `col-md-6`, `col-12`

**Hard:** แบ่ง form ด้วย heading ย่อยและ `border-top pt-3 mt-3`

### `04-02-checks-radios-switches.html`

**Easy:** เพิ่ม `.form-check`

**Medium:** radio ใช้ `name="package"` เดียวกัน และ switch ใช้ `.form-switch`

**Hard:** สร้าง permission card หลายใบด้วย `row row-cols-1 row-cols-md-3 g-3`

### `04-03-input-group-range-datalist.html`

**Easy:** ใช้ `.input-group` + `.input-group-text`

**Medium:** เพิ่ม `input.form-range` และ `input[list]` + `datalist`

**Hard:** summary box ใช้ `alert alert-info` หรือ card ด้านขวาใน `row g-4`

### `04-04-floating-labels.html`

**Easy:** เพิ่ม `.form-floating` พร้อม `input.form-control`

**Medium:** ใช้ `.form-floating` กับ `textarea` และ `select`

**Hard:** ทุก field อยู่ใน `row g-3`; label ต้องอยู่หลัง input/select/textarea

### `04-05-validation-states-feedback.html`

**Easy:** เพิ่ม `required` และ `.invalid-feedback`

**Medium:** checkbox terms ต้องมี `required` และ feedback

**Hard:** ใช้ JS เช็ก `password.value.length >= 8` และ `password.value === confirm.value`; ตั้ง `setCustomValidity`

### `04-06-comprehensive-form.html`

**Easy:** แก้ title และ labels

**Medium:** billing ใช้ `input-group`, `select`, และ `row g-3`

**Hard:** แบ่งเป็น sections ด้วย `fieldset` หรือ heading และใช้ `card`/`border` แยกกลุ่ม

---

## 05 - Landing Page Workshop

### `05-01-landing-page-complete-workshop.html`

**Easy:** แก้ brand/headline/cards

**Medium:** เพิ่ม `row row-cols-1 row-cols-md-3 g-3` สำหรับ testimonials

**Hard:** เพิ่ม logo strip, FAQ cards แบบ static และ contact form พร้อม anchor links

### `05-02-breakpoint-checklist.html`

**Easy:** เพิ่ม `<tr>`

**Medium:** ทำ table columns: Area, Mobile, Tablet, Desktop, Status

**Hard:** ใช้ badge `text-bg-success` / `text-bg-warning` / `text-bg-danger` ใน status column

---

## 06 - JavaScript Plugins Part 1

### `06-01-data-attribute-equation.html`

**Easy:** เปลี่ยน `data-bs-target` ให้ตรงกับ id ใหม่

**Medium:** ทำ FAQ 3 ข้อด้วยปุ่ม 3 ปุ่มและ collapse 3 target

**Hard:** 5 ข้อใช้ id ไม่ซ้ำ เช่น `faqOne` ถึง `faqFive`; ปุ่มมี icon และ `aria-controls`

### `06-02-modal-pro-tips.html`

**Easy:** เพิ่ม `.modal-footer`

**Medium:** ใช้ `data-bs-backdrop="static"` และ `data-bs-keyboard="false"`

**Hard:** modal form ใช้ `form`, `form-control`, footer มี Reset และ Submit

### `06-03-offcanvas-navbar-directions.html`

**Easy:** เปลี่ยน class เป็น `offcanvas-end`

**Medium:** เพิ่ม checkbox ใน `.offcanvas-body`

**Hard:** filter panel มี category checkboxes, range, และ footer buttons `Apply`/`Clear`

### `06-04-collapse-accordion-dropdowns.html`

**Easy:** เพิ่ม `.accordion-item`

**Medium:** dropdown ใช้ `.dropdown-divider` และ `.disabled`

**Hard:** help center มี sidebar/category dropdown ด้านบน และ accordion ด้านล่าง

### `06-05-js-events-lifecycle.html`

**Easy:** เพิ่ม event listener อีก event

**Medium:** ปุ่ม clear ใช้ `eventLog.innerHTML = ""`

**Hard:** timestamp ใช้ `new Date().toLocaleTimeString()` แล้ว append ใน `<li>`

---

## 07 - Interactive UI and Advanced Utilities

### `07-01-carousel-autoplay-controls.html`

**Easy:** เพิ่ม `.carousel-item`

**Medium:** เพิ่ม `.carousel-caption` และ `data-bs-interval`

**Hard:** เพิ่ม 4 slides, indicators 4 ปุ่ม, และตรวจ `data-bs-slide-to` ให้ตรง index

### `07-02-alerts-toasts-spinners.html`

**Easy:** ใช้ `alert-warning alert-dismissible fade show`

**Medium:** ใช้ `bootstrap.Toast.getOrCreateInstance(...).show()`

**Hard:** เมื่อกดปุ่มให้ add spinner, disable ปุ่ม, `setTimeout`, แล้ว show toast และคืนปุ่ม

### `07-03-tooltips-popovers.html`

**Easy:** เพิ่มปุ่มที่มี `data-bs-toggle="tooltip"`

**Medium:** popover ใช้ `data-bs-title` และ `data-bs-content`

**Hard:** initialize ทั้ง tooltip/popover ด้วย `querySelectorAll` และ `new bootstrap.Tooltip/Popover`

### `07-04-z-index-fixed-sticky-object-fit.html`

**Easy:** เปลี่ยน `object-fit`

**Medium:** sticky toolbar ใช้ `sticky-top bg-white border-bottom`

**Hard:** fixed help button ใช้ `position-fixed bottom-0 end-0 m-3`; ตรวจไม่ทับ footer/content

---

## 08 - Advanced Architecture

### `08-01-customization-sass-dark-mode.html`

**Easy:** เปลี่ยน text ปุ่มตอน toggle

**Medium:** card ใช้ CSS variables หรือ Bootstrap theme colors ที่อ่านได้ทั้งสองโหมด

**Hard:** ตั้ง `data-bs-theme` บน `document.documentElement` และปรับ 3 cards ให้ contrast ผ่าน

### `08-02-accessibility-visually-hidden.html`

**Easy:** เพิ่ม `<span class="visually-hidden">...</span>`

**Medium:** input search มี `<label class="visually-hidden" for="search">Search</label>`

**Hard:** icon toolbar ใช้ `button` พร้อม `aria-label` หรือ visually-hidden ครบ 4 ปุ่ม

### `08-03-admin-dashboard-subsystems.html`

**Easy:** เพิ่ม stat card ใน `row`

**Medium:** เพิ่ม `.table-responsive > table.table`

**Hard:** toast notification ใช้ Bootstrap Toast และปุ่ม trigger ใน dashboard

### `08-04-build-tool-matrix-cheatsheet.html`

**Easy:** เพิ่ม row ใน table

**Medium:** deploy checklist ใช้ `list-group` พร้อม checkbox

**Hard:** รวม table, checklist และ accordion; table ต้องอยู่ใน `.table-responsive`
