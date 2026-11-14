# yapılandırma

Vinyl için ortam değişkenleri ve servis entegrasyonlarını yapılandırma.

### Ortam Kurulumu

Proje kök dizininde bir `.env` dosyası oluşturun ve şu değişkeni ekleyin:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### YouTube API Anahtarı Alma

1. [Google Cloud Console](https://console.cloud.google.com/) adresine gidin ve **APIs & Services** bölümünü açın.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. Sol kenar çubuğundan **Library** (Kitaplık) seçeneğine tıklayın.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. **YouTube Data API v3** aramasını yapın, katalogdan seçin ve **Enable** (Etkinleştir) butonuna tıklayın.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. API etkinleştirildikten sonra sol menüdeki **Credentials** (Kimlik Bilgileri) bölümüne gidin, **+ Create Credentials** butonuna basıp **API Key** seçeneğini seçin.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. **Create API key** panelinde ayarları yapın ve **Create** butonuna tıklayın:
   - **Name:** Tanımlayıcı bir ad girin (ör. `vinyl-key`).
   - **API restrictions:** **YouTube Data API v3** seçeneğini işaretleyin.
   - **Application restrictions:** **None** (Yok) olarak bırakın.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Oluşturulan API anahtarını kopyalayın ve `.env` dosyanıza `YOUTUBE_API_KEY` olarak ekleyin:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud, YouTube Data API için yerel geliştirme ve kişisel kullanım için fazlasıyla yeterli ücretsiz günlük kota sağlamaktadır.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Geri: Kurulum</strong></a>
</div>

---

*Sorumluluk Reddi: Bu belge dahili bir yapay zeka otomasyon süreciyle çevrilmiştir ve hatalar veya yanlışlıklar içerebileceğini lütfen unutmayın. İngilizce orijinal belge resmi referans kaynağıdır.*
