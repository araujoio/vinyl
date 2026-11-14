# การกำหนดค่า

วิธีกำหนดค่าตัวแปรสภาพแวดล้อมและการเชื่อมต่อบริการภายนอกสำหรับ Vinyl

### การตั้งค่าสภาพแวดล้อม

สร้างไฟล์ `.env` ในไดเรกทอรีรากและเพิ่มตัวแปรนี้:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### การขอรับคีย์ YouTube API

1. ไปที่ [Google Cloud Console](https://console.cloud.google.com/) แล้วเข้าไปที่ **APIs & Services**

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. ที่เมนูด้านซ้าย ให้คลิกที่ **Library** (คลังไลบรารี)

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. ค้นหา **YouTube Data API v3** เลือกรายการแล้วคลิก **Enable** (เปิดใช้งาน)

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. เมื่อเปิดใช้งานแล้ว ให้ไปที่ **Credentials** ที่เมนูด้านซ้าย คลิก **+ Create Credentials** แล้วเลือก **API Key**

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. ในหน้าต่าง **Create API key** ให้กำหนดค่าตัวเลือกแล้วคลิก **Create**:
   - **Name:** ป้อนชื่อที่จดจำง่าย (เช่น `vinyl-key`)
   - **API restrictions:** เลือก **YouTube Data API v3**
   - **Application restrictions:** ปล่อยไว้เป็น **None**

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. คัดลอกคีย์ API ที่สร้างขึ้นแล้วนำไปใส่ในไฟล์ `.env` ของคุณเป็น `YOUTUBE_API_KEY`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud มีโควต้ารายวันฟรีสำหรับ YouTube Data API ซึ่งเพียงพอสำหรับการพัฒนาและใช้งานส่วนตัว

<div align="left">
  <a href="../01-installation/README.md"><strong>← ก่อนหน้า: การติดตั้ง</strong></a>
</div>

---

*ข้อจำกัดความรับผิดชอบ: เอกสารนี้ได้รับการแปลโดยกระบวนการ AI อัตโนมัติภายใน และอาจมีข้อผิดพลาดหรือไม่ถูกต้อง เอกสารต้นฉบับภาษาอังกฤษถือเป็นแหล่งอ้างอิงอย่างเป็นทางการ*
