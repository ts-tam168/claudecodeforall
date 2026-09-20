# Task List: Thai Food Recommender

อ้างอิงคำนิยามจาก `CONTEXT.md` (Dish, Random Pick, Featured Dish, Favorite)

## 1. โครงสร้างโปรเจกต์

- [X] สร้างโฟลเดอร์ `thai-food-recommender/`
- [X] สร้างไฟล์ `index.html` แบบ self-contained (HTML + CSS + JS ในไฟล์เดียว)

## 2. ข้อมูล Dish

- [X] เตรียม array ของ Dish ~30 รายการ แต่ละรายการมี: `id`, ชื่อไทย, ชื่ออังกฤษ, คำอธิบายสั้น 1 ประโยค, หมวดหมู่ (แกง/ผัด/ทอด/ก๋วยเตี๋ยว/ยำ-ส้มตำ/ของหวาน/เครื่องดื่ม), อิโมจิ/ไอคอนประกอบ

## 3. UI โครงหน้า (หน้าเดียว)

- [X] ส่วนหัว: ชื่อเว็บ + คำโปรย (ไทยเป็นหลัก + อังกฤษกำกับ)
- [X] การ์ด Featured Dish: แสดงไอคอน, ชื่อไทย/อังกฤษ, คำอธิบาย, หมวดหมู่ ของ Dish ที่กำลังแสดงอยู่
- [X] ปุ่ม "สุ่มอาหารไทยวันนี้" (Random Pick)
- [X] ปุ่มหัวใจ toggle Favorite บน Featured Dish ปัจจุบัน (แสดงสถานะ ถูกใจแล้ว/ยังไม่ถูกใจ)
- [X] Section "รายการโปรด" แสดงรายการ Favorite ทั้งหมด (การ์ดย่อ คลิกเพื่อตั้งเป็น Featured Dish, ปุ่มลบออกจากรายการโปรด)
- [X] Empty state ของ section รายการโปรด เมื่อยังไม่มี Favorite

## 4. Logic

- [X] ฟังก์ชัน Random Pick: สุ่ม Dish จาก array ทั้งหมด ตั้งเป็น Featured Dish ใหม่ทุกครั้งที่กดปุ่ม
- [X] เรียก Random Pick อัตโนมัติ 1 ครั้งตอนโหลดหน้าเว็บ (auto-feature ตั้งแต่เปิดมา)
- [X] Toggle Favorite: เพิ่ม/เอา Dish ID ออกจากชุด Favorite, sync กับ localStorage ทันที
- [X] โหลด Favorite จาก localStorage ตอนเปิดหน้าเว็บ, render section รายการโปรด
- [X] คลิกรายการใน Favorite list → ตั้ง Dish นั้นเป็น Featured Dish ใหม่ (ไม่ลบออกจาก Favorite)

## 5. ดีไซน์

- [X] โทนสีอุ่นแบบไทย (แดงเข้ม/ทอง/ครีม)
- [X] Responsive สำหรับมือถือ

## 6. ส่งมอบ

- [X] ทดสอบ flow: เปิดหน้า → เห็น Featured Dish ทันที → กดสุ่มซ้ำ → กดถูกใจ → รีเฟรชหน้าแล้ว Favorite ยังอยู่ → คลิกจาก Favorite list กลับมาเป็น Featured Dish
- [X] Publish เป็น Claude Artifact จาก `index.html`
