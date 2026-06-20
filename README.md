# ยินดีต้อนรับสู่คลังรวมโปรเจกต์ของ Marwan

Repository นี้จัดทำขึ้นเพื่อรวบรวมและบันทึกผลงานการพัฒนาซอฟต์แวร์ทั้งหมดของฉัน โดยแยกตามประเภทและหมวดหมู่ของเทคโนโลยีที่ใช้ครับ

---

## Tech Stack ที่เชี่ยวชาญ
<p align="left">
  <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=FastAPI&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=PostgreSQL&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
</p>

---

## Featured Projects

### BloodPrompt | Blood Donation Booking Web App
เว็บแอปพลิเคชันสำหรับระบบจองคิวบริจาคเลือดออนไลน์ เพื่ออำนวยความสะดวกให้ผู้บริจาคสามารถเลือกวัน เวลา และจัดการนัดหมายล่วงหน้าได้อย่างสะดวกรวดเร็ว
* **Key Features & Dev Details:**
  * พัฒนาฝั่ง Frontend และจัดโครงสร้างแอปพลิเคชันด้วย SvelteKit เพื่อเน้นความเร็วในการโหลดและการทำ Server-Side Rendering (SSR)
  * ใช้ TypeScript ในการเขียนควบคุม Logic ทั้งหมดเพื่อลด Error ในระบบและช่วยให้จัดการ Data Flow ได้แม่นยำขึ้น
  * ออกแบบและตกแต่งหน้าจอแบบ Responsive UI ด้วย Tailwind CSS เพื่อให้ผู้ใช้งานเข้าถึงผ่านมือถือได้ง่ายและมี UI/UX ที่ลื่นไหล
* **Tech Stack:** Svelte, SvelteKit, TypeScript, Tailwind CSS
* **Repository:** 🔗 [DrowningToast/BloodPrompt](https://github.com/DrowningToast/BloodPrompt)

### MUMOOD | Music Discovery & Social Review App
แอปพลิเคชันบนมือถือแบบ Cross-platform สำหรับรีวิวเพลงตามอารมณ์ โดยผู้ใช้สามารถให้คะแนนเพลงผ่านมิติต่างๆ เช่น จังหวะ (Beat), เนื้อเพลง (Lyric) และ Mood ผ่านสีสันที่เลือก
* **Key Features & Dev Details:**
  * พัฒนา Mobile App (iOS/Android) ให้รองรับระบบ Color-based Emotion Selection
  * เชื่อมต่อกับ Spotify API เพื่อดึงข้อมูลเพลง และ Deezer API สำหรับดึงตัวอย่างเสียงความยาว 30 วินาทีมาเปิดเล่นในแอป
  * ออกแบบ Backend ด้วย FastAPI ร่วมกับ SQLAlchemy ORM จัดการระบบ User Auth, Review History, รายการโปรด และระบบจัดการเพลงของ Admin
* **Tech Stack:** Flutter, FastAPI, OAuth 2.0, PostgreSQL, Spotify API, Deezer API
* **Repository:** 🔗 [pp811010/MuMood-musicReview](https://github.com/pp811010/MuMood-musicReview)

### EZTEST | AI-Driven Test Generation Platform
เครื่องมือสำหรับช่วยทำ Automation Test บน Desktop โดยใช้พลังของ LLM ในการวิเคราะห์ Requirements แล้วเจนออกมาเป็น Test Cases และ Test Scripts ที่พร้อมใช้งาน ปรับแต่งมาเพื่อเน้นประสิทธิภาพการทำงานบน Local Environment
* **Key Features & Dev Details:**
  * ออกแบบ Responsive Web UI ด้วย Next.js และ TypeScript เพื่อช่วยให้การกรอกข้อมูล Requirement และการจัดการ Asset ของตัวทดสอบทำได้ง่ายขึ้น
  * วางโครงสร้าง Backend แบบ Privacy-focused บน Local ด้วย FastAPI และ SQLite เพื่อให้มั่นใจว่าข้อมูลสำคัญ (Sensitive Data) จะอยู่บนเครื่องผู้ใช้เท่านั้น ไม่หลุดออกไปข้างนอก
  * ร่วมพัฒนาการต่อเชื่อมกับ Local LLM โดยออกแบบตัวเลือกการ Deployment ผ่าน Hugging Face เพื่อให้รองรับสเปกฮาร์ดแวร์ที่หลากหลาย
* **Tech Stack:** Next.js, TypeScript, FastAPI, SQLite, Hugging Face, LLM (Llama)
* **Repository:** 🔗 [wanmaimarkz/sn-testgeneration-app](https://github.com/wanmaimarkz/sn-testgeneration-app)

### Sport Activity Booking
ระบบจองสนามและพื้นที่ทำกิจกรรมของมหาวิทยาลัย ที่มีระบบควบคุมสิทธิ์ในการเข้าถึงแบบ Role-based Access Control (RBAC) แยกการใช้งานระหว่างนักศึกษาและผู้ดูแลระบบชัดเจน
* **Key Features & Dev Details:**
  * พัฒนาฝั่ง Backend ด้วย Django จัดการระบบยืนยันตัวตน, Custom Booking Logic และระบบแจ้งรายงานปัญหา (Issue Reporting)
  * ทำระบบแจ้งเตือนอัตโนมัติ (Notification System) ผ่าน Gmail API เพื่อส่งข้อมูลอัปเดตสถานะการจองและใบยืนยันแบบ Real-time
  * ออกแบบหน้าเว็บด้วย Tailwind CSS รองรับการแสดงผลแบบ Responsive ตอบโจทย์การใช้งานบนทุกอุปกรณ์
* **Tech Stack:** HTML, Tailwind CSS, JavaScript, Django, PostgreSQL, Gmail API
* **Repository:** 🔗 [pp811010/SportActivityBooking](https://github.com/pp811010/SportActivityBooking)

