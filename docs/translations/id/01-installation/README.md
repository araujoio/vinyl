# instalasi

Cara mengkloning repositori, menginstal dependensi, dan menjalankan Vinyl secara lokal.

> [!NOTE]
> Dukungan kontainer Docker sedang dalam pengembangan. Untuk saat ini, ikuti petunjuk konfigurasi lokal di bawah ini.

### Prasyarat

Sebelum memulai, pastikan Anda telah menginstal:

- **Node.js** (v20 atau lebih baru)
- **Git**
- **npm** (atau pengelola paket pilihan Anda: `pnpm`, `yarn`, `bun`)

---

### 1. Kloning repositori

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. Instal dependensi

Jalankan perintah berikut di direktori root proyek:

```bash
npm install
```

### 3. Jalankan server pengembangan

```bash
npm run dev
```

Setelah berjalan, buka [http://localhost:3000](http://localhost:3000) di browser untuk melihat Vinyl.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← Sebelumnya: Panduan Cepat</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>Selanjutnya: Konfigurasi →</strong></a>
</div>

---

*Penafian: Dokumen ini diterjemahkan melalui proses otomatisasi AI internal dan mungkin mengandung kesalahan atau ketidakakuratan. Dokumentasi asli dalam bahasa Inggris adalah sumber referensi resmi.*
