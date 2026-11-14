# インストール

リポジトリのクローン、依存関係のインストール、Vinyl のローカル実行手順。

> [!NOTE]
> Dockerコンテナ対応は現在開発中です。現時点では以下のローカルセットアップ手順をご利用ください。

### 前提条件

始める前に、以下の環境がインストールされていることを確認してください：

- **Node.js** (v20 以降推奨)
- **Git**
- **npm** (またはお好みのパッケージマネージャー: `pnpm`, `yarn`, `bun`)

---

### 1. リポジトリをクローンする

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. 依存関係をインストールする

プロジェクトのルートディレクトリで次のコマンドを実行します：

```bash
npm install
```

### 3. 開発サーバーを起動する

```bash
npm run dev
```

起動後、ブラウザで [http://localhost:3000](http://localhost:3000) を開くと Vinyl が表示されます。

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← 前へ: クイックスタート</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>次へ: 環境設定 →</strong></a>
</div>

---

*免責事項: このドキュメントは社内のAI自動翻訳プロセスを使用して翻訳されており、誤りや不正確な表現が含まれている場合があります。英語版のオリジナルドキュメントが公式の参照元となります。*
