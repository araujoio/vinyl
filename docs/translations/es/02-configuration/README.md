# configuración

Cómo configurar variables de entorno e integraciones de servicios para Vinyl.

### Configuración del entorno

Crea un archivo `.env` en el directorio raíz y agrega esta variable:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Obtención de una clave de API de YouTube

1. Ve a [Google Cloud Console](https://console.cloud.google.com/) y dirígete a **APIs y servicios**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. En el menú lateral izquierdo, haz clic en **Biblioteca**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Busca **YouTube Data API v3**, selecciónala en el catálogo y haz clic en **Habilitar**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Una vez habilitada la API, ve a **Credenciales** en el menú lateral, haz clic en **+ Crear credenciales** y elige **Clave de API**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. En el panel **Crear clave de API**, configura las opciones y haz clic en **Crear**:
   - **Nombre:** Ingresa un nombre identificable (ej: `vinyl-key`).
   - **APIs accesibles con esta clave:** Selecciona **YouTube Data API v3** en las restricciones de API.
   - **Restricciones de aplicación:** Mantén en **Ninguna**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Copia la clave generada y asígnala a `YOUTUBE_API_KEY` en tu archivo `.env`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud proporciona una cuota diaria gratuita para la API de YouTube Data que es más que suficiente para el desarrollo local y uso personal.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Anterior: Instalación</strong></a>
</div>

---

*Aviso Legal: Este documento fue traducido mediante un proceso interno automatizado de IA y puede contener imprecisiones o errores. La documentación original en inglés es la fuente oficial de referencia.*
