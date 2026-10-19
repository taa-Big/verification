# สไลด์: คู่มือยืนยันตัวตนหรือองค์กร (Meta Ads)

สไลด์ Reveal.js แบบ static ไฟล์เดียว (`index.html`) — ไม่ต้อง build

## ดูในเครื่อง
เปิด `index.html` ในเบราว์เซอร์ได้เลย (ต้องต่ออินเทอร์เน็ต เพราะโหลด Reveal.js/ฟอนต์จาก CDN)

คีย์ลัด: `S` โหมดผู้พูด · `F` เต็มจอ · `Esc` ภาพรวมสไลด์ · `?` ดูคีย์ลัดทั้งหมด

## ขึ้น GitHub
```bash
git init
git add .
git commit -m "Add Reveal.js slides"
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
```

## ออโตโฮสบน Cloudflare Pages
1. Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**
2. เลือก repo นี้ แล้วตั้งค่า
   - Framework preset: **None**
   - Build command: *(เว้นว่าง)*
   - Build output directory: `/`
3. กด **Save and Deploy** — ต่อไปทุกครั้งที่ push เข้า `main` จะ deploy อัตโนมัติ
