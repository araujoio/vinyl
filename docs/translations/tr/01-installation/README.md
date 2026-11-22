# kurulum

Depoyu klonlama, bağımlılıkları yükleme ve Vinyl'i yerel olarak çalıştırma adımları.

> [!NOTE]
> Docker konteyner desteği şu anda geliştirme aşamasındadır. Şimdilik aşağıdaki yerel kurulum adımlarını takip edin.

### Gereksinimler

Başlamadan önce sisteminizde şunların kurulu olduğundan emin olun:

- **Node.js** (v20 veya üzeri önerilir)
- **Git**
- **npm** (veya tercih ettiğiniz paket yöneticisi: `pnpm`, `yarn`, `bun`)

---

### 1. Depoyu klonlayın

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. Bağımlılıkları yükleyin

Proje kök dizininde şu komutu çalıştırın:

```bash
npm install
```

### 3. Geliştirme sunucusunu başlatın

```bash
npm run dev
```

Başlatıldıktan sonra Vinyl'i görüntülemek için tarayıcınızda [http://localhost:3000](http://localhost:3000) adresini açın.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← Geri: Hızlı Başlangıç</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>İleri: Yapılandırma →</strong></a>
</div>

---

*Sorumluluk Reddi: Bu belge dahili bir yapay zeka otomasyon süreciyle çevrilmiştir ve hatalar veya yanlışlıklar içerebileceğini lütfen unutmayın. İngilizce orijinal belge resmi referans kaynağıdır.*
