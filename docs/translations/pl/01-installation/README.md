# instalacja

Jak sklonować repozytorium, zainstalować zależności i uruchomić Vinyl lokalnie.

> [!NOTE]
> Wsparcie dla Dockera jest obecnie w trakcie opracowywania. Na razie skorzystaj z poniższych instrukcji instalacji lokalnej.

### Wymagania wstępne

Przed rozpoczęciem upewnij się, że masz zainstalowane:

- **Node.js** (wersja 20 lub nowsza)
- **Git**
- **npm** (lub preferowany menedżer: `pnpm`, `yarn`, `bun`)

---

### 1. Sklonuj repozytorium

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. Zainstaluj zależności

Uruchom następujące polecenie w katalogu głównym projektu:

```bash
npm install
```

### 3. Uruchom serwer deweloperski

```bash
npm run dev
```

Po uruchomieniu otwórz [http://localhost:3000](http://localhost:3000) w przeglądarce, aby zobaczyć działający Vinyl.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← Wstecz: Szybki start</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>Dalej: Konfiguracja →</strong></a>
</div>

---

*Zastrzeżenie prawne: Niniejszy dokument został przetłumaczony w ramach wewnętrznego zautomatyzowanego procesu SI i może zawierać nieścisłości lub błędy. Oficjalnym źródłem odniesienia jest oryginalna dokumentacja w języku angielskim.*
