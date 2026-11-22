# configurazione

Come configurare le variabili d'ambiente e le integrazioni di servizi per Vinyl.

### Configurazione dell'ambiente

Crea un file `.env` nella directory principale e aggiungi questa variabile:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Come ottenere una chiave API di YouTube

1. Accedi a [Google Cloud Console](https://console.cloud.google.com/) e vai su **API e servizi**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. Nel menu laterale sinistro, clicca su **Libreria**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Cerca **YouTube Data API v3**, selezionala dal catalogo e clicca su **Abilita**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Dopo aver abilitato l'API, vai su **Credenziali** nel menu laterale, clicca su **+ Crea credenziali** e seleziona **Chiave API**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. Nel pannello **Crea chiave API**, configura le opzioni e clicca su **Crea**:
   - **Nome:** Inserisci un nome descrittivo (es. `vinyl-key`).
   - **API accessibili:** Seleziona **YouTube Data API v3** sotto le restrizioni API.
   - **Restrizioni applicative:** Mantieni su **Nessuna**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Copia la chiave generata e inseriscila come `YOUTUBE_API_KEY` nel tuo file `.env`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud offre una quota giornaliera gratuita per l'API YouTube Data ampiamente sufficiente per lo sviluppo locale e l'uso personale.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Precedente: Installazione</strong></a>
</div>

---

*Dichiarazione di non responsabilità: Questo documento è stato tradotto tramite un processo interno automatizzato di IA e potrebbe contenere inesattezze o errori. La documentazione originale in inglese rappresenta la fonte ufficiale di riferimento.*
