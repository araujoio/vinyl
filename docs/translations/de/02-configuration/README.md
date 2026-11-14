# konfiguration

So konfigurieren Sie Umgebungsvariablen und Dienste für Vinyl.

### Umgebungseinrichtung

Erstellen Sie eine `.env`-Datei im Stammverzeichnis und fügen Sie diese Variable hinzu:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Abrufen eines YouTube-API-Schlüssels

1. Öffnen Sie die [Google Cloud Console](https://console.cloud.google.com/) und navigieren Sie zu **APIs & Dienste**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. Klicken Sie im linken Menü auf **Bibliothek**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Suchen Sie nach **YouTube Data API v3**, wählen Sie den Eintrag aus und klicken Sie auf **Aktivieren**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Wechseln Sie nach der Aktivierung im linken Menü zu **Anmeldedaten**, klicken Sie auf **+ Anmeldedaten erstellen** und wählen Sie **API-Schlüssel**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. Konfigurieren Sie im Bereich **API-Schlüssel erstellen** die Optionen und klicken Sie auf **Erstellen**:
   - **Name:** Geben Sie einen eindeutigen Namen ein (z. B. `vinyl-key`).
   - **Zugängliche APIs:** Wählen Sie unter API-Einschränkungen **YouTube Data API v3** aus.
   - **Anwendungseinschränkungen:** Auf **Keine** belassen.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Kopieren Sie den generierten Schlüssel und tragen Sie ihn als `YOUTUBE_API_KEY` in Ihre `.env`-Datei ein:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud bietet ein kostenloses tägliches Kontingent für die YouTube Data API, das für lokale Entwicklung und private Nutzung völlig ausreicht.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Zurück: Installation</strong></a>
</div>

---

*Haftungsausschluss: Dieses Dokument wurde durch einen internen automatisierten KI-Prozess übersetzt und kann Ungenauigkeiten oder Fehler enthalten. Die englische Originaldokumentation ist die verbindliche Referenzquelle.*
