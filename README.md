# SMS API Server

سيرفر API لاستقبال الرسائل النصية وأكواد التحقق (OTP)

## 🚀 التثبيت السريع

1. ارفع الملفات للسيرفر
2. شغل `install.php`
3. استخدم API Key للاتصال

## 📡 نقاط النهاية (Endpoints)

| المسار | الطريقة | الوصف |
|--------|---------|-------|
| `/get_codes` | GET | جلب الأكواد الجديدة |
| `/add_number` | POST | إضافة رقم جديد |
| `/delete_number` | POST | حذف رقم |
| `/receive_sms` | POST | استقبال رسالة جديدة |
| `/stats` | GET | إحصائيات |

## 🔑 التوثيق

استخدم Header: `X-API-Key: your-api-key`

## 🐳 التشغيل مع Docker

```bash
docker build -t sms-api .
docker run -p 80:80 sms-api