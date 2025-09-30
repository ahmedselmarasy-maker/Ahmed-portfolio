# تعليمات نشر الموقع على Netlify

## المشاكل المحتملة وحلولها:

### 1. مشكلة اختفاء الصور
**السبب**: مسارات الصور غير صحيحة أو الملفات غير مرفوعة

**الحل**:
- تأكد من رفع جميع الملفات في المجلدات الصحيحة:
  - `project-images/` - صور المشاريع
  - `certificates/` - صور الشهادات
  - `profile-image.jpg` - الصورة الشخصية

### 2. خطوات النشر الصحيحة:

1. **ارفع جميع الملفات**:
   ```
   portfolio/
   ├── index.html
   ├── styles.css
   ├── script.js
   ├── profile-image.jpg
   ├── project-images/
   │   ├── heart-disease-app.jpg
   │   ├── neonatal-prediction.jpg
   │   ├── Summer Training.jpg
   │   ├── robot-arm-design.jpg
   │   ├── elevator-system.jpg
   │   └── mechanical-vibrations.jpg
   ├── certificates/
   │   ├── microsoft-certificate.jpg
   │   └── summer-training.jpg
   ├── _redirects
   ├── netlify.toml
   └── favicon.ico
   ```

2. **في Netlify**:
   - اذهب إلى "Sites"
   - اضغط "New site from Git" أو "Deploy manually"
   - اسحب وأفلت جميع الملفات
   - تأكد من أن "Publish directory" فارغ (.)

### 3. إعدادات إضافية:

- **Custom domain**: يمكنك ربط دومين خاص بك
- **HTTPS**: Netlify يوفر SSL تلقائياً
- **Form handling**: النموذج يعمل مع Formspree

### 4. اختبار الموقع:

بعد النشر، تأكد من:
- ✅ جميع الصور تظهر بشكل صحيح
- ✅ النموذج يعمل (Formspree)
- ✅ الروابط تعمل
- ✅ الموقع responsive على الموبايل

### 5. إذا استمرت المشكلة:

1. تحقق من Console في المتصفح (F12)
2. تأكد من أن جميع الملفات مرفوعة
3. جرب مسح cache المتصفح
4. تأكد من أن أسماء الملفات لا تحتوي على مسافات أو أحرف خاصة

## ملاحظات مهمة:

- الملفات `_redirects` و `netlify.toml` تساعد في تحسين الأداء
- تأكد من أن جميع الصور محسنة للويب (حجم صغير)
- النموذج يعمل مع Formspree بدون إعدادات إضافية
