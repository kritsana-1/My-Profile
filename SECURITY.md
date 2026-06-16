# My Profile
Hi, I'm Q. I'm a Computer Science student who loves learning new things and conquering tech challenges!

## 🔒 About Security

This repository documents my journey through cybersecurity learning and wargame challenges. It focuses on building foundational security skills through hands-on practice with tools and Linux command-line techniques.

---

## Bandit Wargame Progress

### Level 0 - Level 5
วันนี้ผ่านด้าน bandit level0 to level5

**คำสั่งที่ได้ใช้บ่อย:**
- `ls`: ดูว่ามีไฟล์อะไรบ้าง
- `cd`: เข้าถึงไฟล์
- `ls -a`: หาไฟล์หรือโฟรเดอร์ที่ซ่อนอยู่ทั้งหมด
- `find . -type f -size 1033c !executable`
  - `by .`: ค้นหาตั้งแต่ที่อยู่ปัจจุบัน
  - `-type`: ประกาศเพื่อระบุชนิดที่ต้องการ
  - `f`: ย่อมาจาก file
  - `-size`: ประกาศเพื่อระบุ size ที่ต้องการ
  - `1033`: ขนาดไซด์
  - `c`: ย่อมาจาก bytes
  - `!executable`: บอกว่าไม่ต้องสิ่งนี้

### Level 6 - Level 15 (15/06/2025)

**คำสั่ง:** `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null`
- `find /`: สั่งให้ค้นหาจากไดเรกทอรีนอกสุด (Root)
- `-user bandit7`: กรองเฉพาะไฟล์ที่เจ้าของคือ bandit7
- `-group bandit6`: กรองเฉพาะไฟล์ที่อยู่ภายใต้กลุ่ม bandit6
- `2>/dev/null`: ช่วยซ่อนข้อความแจ้งเตือนที่จำเป็น

**คำสั่ง:** `grep "millionth" data.txt`
- `grep`: เป็นคำสั่งที่ใช้ค้นหาข้อความหรือแพทเทิร์นที่เราต้องการภายในไฟล์
- `"millionth"`: คือคำค้นหา (Keyword) ที่โจทย์กำหนดมาให้
- `data.txt`: คือชื่อไฟล์ที่เราต้องการจะค้นหาข้างใน

**คำสั่ง:** `sort data.txt | uniq -u`
- `sort`: เรียงตามตัวอักษร
- `|`: จะรับข้อมูลจากคำสั่งก่อนหน้าแล้วส่งต่อให้คำสั่งต่อไป
- `uniq`: อ่านข้อมูลในไฟล์ถ้ามีข้อมูลซํ้าก็จะข้ามไป แต่มีข้อจำกัดคือจะจัดการก็ต่อเมื่อข้อมูลนั้นเรียงอยุ่ติดกันเท่านั้น
- `-u`: ให้แสดงเฉพาะบรรทัดที่ไม่มีคู่ซ้ำเลย

**คำสั่ง:** `strings data.txt | grep "==="`
- `strings data.txt`: ทำหน้าที่เปิดอ่านไฟล์ data.txt แล้วคัดกรองพิมพ์ออกมาเฉพาะข้อความปกติที่มนุษย์อ่านรู้เรื่อง
- `grep "==="`: ทำการค้นหาบรรทัดที่มีเครื่องหมาย = เรียงติดกันหลายๆ ตัว

**คำสั่ง:** `base64 -d data.txt`
- `base64`: เป็นคำสั่งที่ใช้สำหรับเข้ารหัสหรือถอดรหัส Base64
- `-d or --decode`: เป็นการบอกว่าเราต้องการจะถอดรหัส (Decode) ข้อมูลนะ
