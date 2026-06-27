# Portto — แอปบันทึกการเทรดหุ้น

เว็บแอปบันทึกพอร์ตหุ้นและกองทุน (ทำงานบนเบราว์เซอร์ เก็บข้อมูลในเครื่องด้วย localStorage ไม่ต้องมีเซิร์ฟเวอร์)

## ไฟล์ในโฟลเดอร์นี้
- `index.html` — หน้าเริ่มต้น / สมัคร-เข้าสู่ระบบ (entry point)
- `app.html` — ตัวแอปบันทึกการเทรด
- `favicon.svg`, `favicon-32.png`, `favicon-16.png` — ไอคอนบนแท็บเบราว์เซอร์
- `apple-touch-icon.png` — ไอคอนตอน "เพิ่มลงหน้าจอโฮม" (iOS)
- `icon-192.png`, `icon-512.png`, `manifest.webmanifest` — ไอคอน/ข้อมูลแอป (Android / PWA)
- `.nojekyll` — ให้ GitHub Pages เสิร์ฟไฟล์ตามจริง

## วิธี deploy ขึ้น GitHub Pages

### 1. เปิด repo `portto` บน github.com

### 2. อัปโหลด **ทุกไฟล์ในโฟลเดอร์นี้**
หน้า repo → "Add file" → "Upload files" → ลากไฟล์ **ทั้งหมด** ในโฟลเดอร์ `dist` เข้าไป → "Commit changes"

> สำคัญ: ต้องอัปทุกไฟล์ (รวมไอคอนและ manifest) ไม่งั้นโลโก้บนแท็บจะไม่ขึ้น

### 3. เปิด GitHub Pages
repo → Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / `/ (root)` → Save

รอ 1–2 นาที เว็บจะอยู่ที่:
```
https://niimph-max.github.io/portto/
```
