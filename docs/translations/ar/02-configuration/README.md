# الإعدادات

كيفية إعداد المتغيرات البيئية والتكامل مع الخدمات الخارجية لتطبيق Vinyl.

### إعداد بيئة التشغيل

أنشئ ملف `.env` في المجلد الرئيسي للمشروع وأضف المتغير التالي:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### الحصول على مفتاح واجهة برمجة تطبيقات YouTube

1. انتقل إلى [Google Cloud Console](https://console.cloud.google.com/) وافتح **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. من القائمة الجانبية اليسرى، انقر على **Library** (المكتبة).

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. ابحث عن **YouTube Data API v3** واخترها من الدليل ثم انقر فوق **Enable** (تفعيل).

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. بعد تفعيل الواجهة، انتقل إلى **Credentials** (بيانات الاعتماد) في القائمة الجانبية، ثم انقر فوق **+ Create Credentials** واختر **API Key**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. في نافذة **Create API key**، اضبط الخيارات التالية ثم اضغط **Create**:
   - **Name:** أدخل اسماً توضيحياً (مثل `vinyl-key`).
   - **قيود الواجهة (API restrictions):** حدد **YouTube Data API v3**.
   - **قيود التطبيق (Application restrictions):** اتركها على **None**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. انسخ المفتاح الذي تم إنشاؤه وأضفه كقيمة للمتغير `YOUTUBE_API_KEY` داخل ملف `.env`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> توفر منصة Google Cloud حصة استخدام يومية مجانية كافية جداً للتطوير المحلي والاستخدام الشخصي.

<div align="left">
  <a href="../01-installation/README.md"><strong>→ السابق: التثبيت</strong></a>
</div>

---

*إخلاء مسؤولية: تمت ترجمة هذه الوثيقة عبر عملية ذكاء اصطناعي آلية داخلية وقد تحتوي على أخطاء أو عدم دقة. تعد الوثائق الأصلية باللغة الإنجليزية هي المصدر المرجعي المعتمد.*
