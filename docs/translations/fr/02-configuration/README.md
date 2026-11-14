# configuration

Comment configurer les variables d'environnement et les intégrations de services pour Vinyl.

### Configuration de l'environnement

Créez un fichier `.env` à la racine du projet et ajoutez cette variable :

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Obtenir une clé d'API YouTube

1. Rendez-vous sur la [Google Cloud Console](https://console.cloud.google.com/) et ouvrez **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. Dans le menu latéral gauche, cliquez sur **Bibliothèque**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Recherchez **YouTube Data API v3**, sélectionnez-la dans le catalogue et cliquez sur **Activer**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Une fois l'API activée, rendez-vous dans **Identifiants** dans le menu latéral, cliquez sur **+ Créer des identifiants** et choisissez **Clé API**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. Dans le panneau **Créer une clé API**, configurez les options et cliquez sur **Créer** :
   - **Nom :** Saisissez un nom reconnaissable (ex. : `vinyl-key`).
   - **APIs accessibles :** Cochez **YouTube Data API v3** dans les restrictions d'API.
   - **Restrictions d'application :** Laissez sur **Aucune**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Copiez la clé générée et collez-la dans votre fichier `.env` en tant que `YOUTUBE_API_KEY` :

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud propose un quota quotidien gratuit pour l'API YouTube Data, largement suffisant pour le développement local et un usage personnel.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Précédent : Installation</strong></a>
</div>

---

*Avertissement: Ce document a été traduit par un processus interne automatisé d'IA et peut contenir des erreurs ou des inexactitudes. La documentation originale en anglais constitue la source de référence officielle.*
