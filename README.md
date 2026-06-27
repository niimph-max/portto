# Portto — แอปบันทึกการเทรดหุ้น

เว็บแอปบันทึกพอร์ตหุ้นและกองทุน (ทำงานบนเบราว์เซอร์ เก็บข้อมูลในเครื่องด้วย localStorage ไม่ต้องมีเซิร์ฟเวอร์)

## ไฟล์
- `index.html` — หน้าเริ่มต้น / สมัคร-เข้าสู่ระบบ (entry point)
- `app.html` — ตัวแอปบันทึกการเทรด
- `.nojekyll` — ให้ GitHub Pages เสิร์ฟไฟล์ตามจริง

ทั้งสองไฟล์เป็น HTML แบบ standalone รวมทุกอย่างในไฟล์เดียว เปิดได้เลยแม้ออฟไลน์

## วิธี deploy ขึ้น GitHub Pages

### 1. สร้าง repo ชื่อ `portto` บน GitHub (เว็บ github.com → New repository)

### 2. อัปโหลดไฟล์ (เลือกวิธีใดวิธีหนึ่ง)

**วิธี A — ลากวางบนเว็บ (ง่ายสุด)**
เปิดหน้า repo → "Add file" → "Upload files" → ลากไฟล์ `index.html`, `app.html`, `.nojekyll` เข้าไป → Commit

**วิธี B — ใช้ Git ในเครื่อง**
```bash
cd dist
git init
git add .
git commit -m "Deploy Portto"
git branch -M main
git remote add origin https://github.com/<ชื่อผู้ใช้>/portto.git
git push -u origin main
```

### 3. เปิด GitHub Pages
repo → Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / `/ (root)` → Save

รอ 1–2 นาที เว็บจะอยู่ที่:
```
https://<ชื่อผู้ใช้>.github.io/portto/
```
