# Pawwwpack — เว็บสาธารณะ 🐾

หน้าเว็บ HTML ของ Pawwwpack ที่เปิดให้ทุกคนเข้าดูได้ ขึ้นบน GitHub Pages ฟรี
ทุกหน้าเป็นไฟล์ HTML ไฟล์เดียว รูปฝังเป็น base64 ไม่มีเซิร์ฟเวอร์ ไม่มีฐานข้อมูล

| หน้า | ลิงก์ | ไฟล์ |
|---|---|---|
| สรุปดีไซน์ (design handoff) | <https://na-subin.github.io/pawwwpack-site/> | `index.html` · `boards/*.html` · `canvas.json` |
| สไลด์นำเสนอ | <https://na-subin.github.io/pawwwpack-site/presentation/> | `presentation/index.html` |
| เครื่องมือวงเพื่อน | <https://na-subin.github.io/pawwwpack-site/tools/> | `tools/index.html` |

เครื่องมือวงเพื่อน: หารค่าอาหาร (`#split`) · เกมวงเหล้า (`#party`) · นับถอยหลังพร้อมพลุ (`#countdown`) — ไม่ต้องล็อกอิน ไม่บันทึกข้อมูล

## อย่าแก้ไฟล์ในนี้โดยตรง

ต้นฉบับอยู่ใน repo หลักของระบบ (private) แล้วคัดลอกมาที่นี่ด้วยสคริปต์:

```bash
# ใน repo หลัก
bun scripts/sync-site.mjs        # คัดลอกไปที่ ../pawwwpack-site
cd ../pawwwpack-site
git add -A && git commit -m "Sync pages" && git push
```

push เข้า `main` แล้ว GitHub Actions จะอัปเดตเว็บให้ภายใน 1–2 นาที

## ค่าใช้จ่าย

ฟรี ตราบใดที่ repo นี้เป็น public — ไม่จำกัดจำนวนครั้งที่เปิด (soft limit ประมาณ 100 GB ต่อเดือน เกินแล้ว GitHub แค่ส่งอีเมลเตือน ไม่เก็บเงิน)
