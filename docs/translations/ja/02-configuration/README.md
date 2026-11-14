# 環境設定

Vinyl の環境変数と外部サービス連携の設定方法。

### 環境設定手順

プロジェクトのルートディレクトリに `.env` ファイルを作成し、次の変数を追加します：

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### YouTube API キーの取得

1. [Google Cloud Console](https://console.cloud.google.com/) にアクセスし、**API とサービス** を開きます。

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. 左側のサイドバーメニューから **ライブラリ** をクリックします。

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. **YouTube Data API v3** を検索し、カタログから選択して **有効にする** をクリックします。

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. API が有効になったら、左側メニューの **認証情報** に進み、**+ 認証情報を作成** をクリックして **API キー** を選択します。

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. **API キーの作成** パネルで各項目を設定し、**作成** をクリックします：
   - **名前:** わかりやすい名前を入力します（例: `vinyl-key`）。
   - **キーで使用可能な API:** API の制限で **YouTube Data API v3** を選択します。
   - **アプリケーションの制限:** **なし** のままにします。

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. 生成された API キーをコピーし、`.env` ファイルの `YOUTUBE_API_KEY` に設定します：

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud は YouTube Data API に十分な無料枠を提供しており、ローカル開発や個人利用には十分対応できます。

<div align="left">
  <a href="../01-installation/README.md"><strong>← 前へ: インストール</strong></a>
</div>

---

*免責事項: このドキュメントは社内のAI自動翻訳プロセスを使用して翻訳されており、誤りや不正確な表現が含まれている場合があります。英語版のオリジナルドキュメントが公式の参照元となります。*
