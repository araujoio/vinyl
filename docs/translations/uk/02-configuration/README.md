# конфігурація

Налаштування змінних середовища та інтеграцій для Vinyl.

### Налаштування середовища

Створіть файл `.env` у кореневому каталозі та додайте цю змінну:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Отримання ключа YouTube API

1. Перейдіть до [Google Cloud Console](https://console.cloud.google.com/) та відкрийте **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. У лівому меню оберіть **Library** (Бібліотека).

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Знайдіть **YouTube Data API v3**, виберіть його та натисніть **Enable** (Увімкнути).

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Після активації перейдіть до **Credentials** у меню ліворуч, натисніть **+ Create Credentials** та виберіть **API Key**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. У вікні **Create API key** налаштуйте параметри та натисніть **Create**:
   - **Name:** Введіть зрозумілу назву (наприклад, `vinyl-key`).
   - **API restrictions:** Оберіть **YouTube Data API v3**.
   - **Application restrictions:** Залиште **None** (Немає).

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Скопіюйте згенерований ключ і вкажіть його у файлі `.env` як `YOUTUBE_API_KEY`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud надає безкоштовну щоденну квоту для YouTube Data API, якої більш ніж достатньо для локальної розробки та особистого використання.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Назад: Встановлення</strong></a>
</div>

---

*Відмова від відповідальності: Цей документ перекладено за допомогою внутрішнього автоматизованого процесу штучного інтелекту і він може містити неточності або помилки. Офіційним джерелом є оригінальна документація англійською мовою.*
