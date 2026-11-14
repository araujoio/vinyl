# конфигурация

Настройка переменных окружения и интеграций для Vinyl.

### Настройка окружения

Создайте файл `.env` в корневой директории и добавьте следующую переменную:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Получение ключа YouTube API

1. Перейдите в [Google Cloud Console](https://console.cloud.google.com/) в раздел **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. В левом боковом меню выберите **Library** (Библиотека).

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Найдите **YouTube Data API v3**, выберите его и нажмите **Enable** (Включить).

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. После включения перейдите в **Credentials** (Учётные данные), нажмите **+ Create Credentials** и выберите **API Key**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. В панели **Create API key** настройте параметры и нажмите **Create**:
   - **Name:** Введите понятное имя (например, `vinyl-key`).
   - **API restrictions:** Выберите **YouTube Data API v3**.
   - **Application restrictions:** Оставьте **None** (Нет).

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Скопируйте созданный ключ и добавьте его в `.env` как `YOUTUBE_API_KEY`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud предоставляет бесплатную ежедневную квоту для YouTube Data API, которой более чем достаточно для локальной разработки и личного использования.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Назад: Установка</strong></a>
</div>

---

*Отказ от ответственности: Этот документ был переведен с помощью внутреннего автоматизированного процесса ИИ и может содержать неточности или ошибки. Официальным источником является оригинальная документация на английском языке.*
