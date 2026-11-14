# installation

Hur du klonar arkivet, installerar beroenden och kör Vinyl lokalt.

> [!NOTE]
> Docker-stöd är för närvarande under utveckling. Följ de lokala installationsanvisningarna nedan tills vidare.

### Förutsättningar

Innan du börjar, kontrollera att följande är installerat:

- **Node.js** (v20 eller senare)
- **Git**
- **npm** (eller ditt val: `pnpm`, `yarn`, `bun`)

---

### 1. Klona arkivet

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. Installera beroenden

Kör följande kommando i projektets rotkatalog:

```bash
npm install
```

### 3. Starta utvecklingsservern

```bash
npm run dev
```

När den har startat, öppna [http://localhost:3000](http://localhost:3000) i webbläsaren för att se Vinyl.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← Föregående: Snabbstart</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>Nästa: Konfiguration →</strong></a>
</div>

---

*Friskrivningsklausul: Detta dokument översattes via en intern automatiserad AI-process och kan innehålla felaktigheter eller misstag. Den engelska originaldokumentationen är den officiella referenskällan.*
