# configuration

How to configure environment variables and service integrations for Vinyl.

### Environment Setup

Create a `.env` file in the root directory and add this variable:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Obtaining a YouTube API Key

1. Go to the [Google Cloud Console](https://console.cloud.google.com/) and navigate to **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. In the left sidebar menu, click on **Library**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Search for **YouTube Data API v3**, select it from the catalog, and click **Enable**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Once the API is enabled, navigate to **Credentials** in the left sidebar, click **+ Create Credentials**, and choose **API Key**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. In the **Create API key** panel, configure the key options and click **Create**:
   - **Name:** Enter a recognizable name (e.g., `vinyl-key`).
   - **APIs that can be accessed using this key:** Select **YouTube Data API v3** under API restrictions.
   - **Application restrictions:** Keep as **None**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Copy the generated API key and assign it to `YOUTUBE_API_KEY` in your `.env` file:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```


> [!TIP]
> Google Cloud provides a free daily quota for the YouTube Data API that is more than sufficient for local development and personal use.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Previous: Installation</strong></a>
</div>
