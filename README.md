
# Project Title

A brief description of what this project does and who it's for

# 🛡️ AegisFace: Multi-Angle AI Recognition System

**AegisFace** เป็นระบบ Face Recognition ยุคใหม่ที่เปลี่ยนการยืนยันตัวตนแบบเดิมๆ ให้มีความแม่นยำระดับสูงสุดด้วยเทคโนโลยี **Flex-Angle Capture** ซึ่งจำลองการทำงานของ Biometric Security ในสมาร์ทโฟนระดับเรือธง



## ✨ Key Features
* **15-Point Flex Registration:** ระบบลงทะเบียนที่เก็บข้อมูลใบหน้าถึง 15 มุม (หน้าตรง, หันซ้าย-ขวา, ก้ม-เงย, เอียง) เพื่อความแม่นยำ 360 องศา
* **VGG-Face Deep Learning:** ขับเคลื่อนด้วยโมเดล VGG-Face ผ่าน DeepFace Library ที่ให้ความแม่นยำสูงในระดับสากล
* **Real-time Recognition:** ตรวจสอบและยืนยันตัวตนได้ทันทีผ่านกล้อง WebCam พร้อมระบบคำนวณ Confidence Score (%)
* **Cloud-Native Integration:** ออกแบบมาเพื่อรันบน Google Colab โดยเก็บข้อมูลรูปภาพและ Embeddings ไว้บน Google Drive อย่างปลอดภัย
* **Modern UI/UX:** หน้าจอผู้ใช้งานที่สวยงามด้วย CSS ระดับพรีเมียม รองรับการใช้งานทั้ง Desktop และ Mobile

## 🚀 Tech Stack
* **Backend:** Python, Flask
* **AI/ML:** DeepFace, OpenCV, TensorFlow
* **Data Science:** NumPy, Pandas, Pickle
* **Frontend:** HTML5, CSS3 (Glassmorphism UI), JavaScript
* **Tunneling:** Pyngrok

## 🛠️ การติดตั้งและใช้งาน (Installation)

1.  **เชื่อมต่อ Google Drive:** เพื่อใช้สำหรับเก็บข้อมูลรูปภาพและ Encoded Vectors
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```

2.  **ติดตั้ง Library ที่จำเป็น:**
    ```bash
    pip install deepface pyngrok flask-ngrok pandas
    ```

3.  **ตั้งค่า Ngrok Token:** นำ Authtoken จาก [ngrok.com](https://dashboard.ngrok.com/) มาใส่ในโค้ดเพื่อสร้าง Public URL

4.  **รันแอปพลิเคชัน:**
    ```bash
    python app.py
    ```

## 📸 มุมที่ต้องลงทะเบียน (Registration Guide)
ระบบจะนำทางคุณให้ถ่ายภาพทั้งหมด 15 มุม เพื่อสร้าง "Digital Identity" ที่สมบูรณ์แบบที่สุด:
- **มุม 1:** หน้าตรง
- **มุม 2-5:** หันซ้าย/ขวา (15° และ 30°)
- **มุม 6-7:** ก้ม/เงยหน้า
- **มุม 8-9:** เอียงศีรษะ
- **มุม 10-15:** การผสมผสานมุมต่างๆ (Complex Angles)



## 🔒 Security & Privacy
ระบบนี้เก็บข้อมูลในรูปแบบของ **Face Embeddings (128-D/4096-D Vectors)** ซึ่งไม่สามารถย้อนกลับมาเป็นภาพใบหน้าเดิมได้ 100% ช่วยเพิ่มความปลอดภัยให้กับข้อมูลชีวมาตรของผู้ใช้งาน

---
Developed with ❤️ by **Jitwisut Thobut** *Computer Engineering, Rangsit University*
