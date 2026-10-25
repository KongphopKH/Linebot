# LineBot

LINE Chatbot พัฒนาด้วย Python (Flask) และ LINE Messaging API

## ความสามารถ
- ตอบทักทายเมื่อพิมพ์ "สวัสดี"
- พิมพ์ "ช่วยเหลือ" เพื่อดูวิธีใช้
- ข้อความอื่น ๆ บอทจะตอบกลับข้อความเดิม (Echo)

## ไฟล์ในโปรเจกต์
- `app.py` — โค้ดหลักของบอท รับ Webhook จาก LINE ที่ `/callback`
- `requirements.txt` — ไลบรารีที่ใช้

## การติดตั้ง
1. ตั้งค่า Environment Variables
   - `CHANNEL_ACCESS_TOKEN`
   - `CHANNEL_SECRET`
2. ติดตั้งไลบรารี: `pip install -r requirements.txt`
3. รันเซิร์ฟเวอร์: `gunicorn app:app`
4. ตั้ง Webhook URL ใน LINE Developers เป็น `https://<your-domain>/callback`
