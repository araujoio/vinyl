# 설치 가이드

리포지토리 클론, 종속성 설치 및 Vinyl 로컬 실행 방법.

> [!NOTE]
> Docker 컨테이너 지원은 현재 개발 중입니다. 당분간은 아래의 로컬 설정 안내를 따라주세요.

### 사전 요구사항

시작하기 전에 다음 항목이 설치되어 있는지 확인하세요:

- **Node.js** (v20 이상 권장)
- **Git**
- **npm** (또는 선호하는 패키지 관리자: `pnpm`, `yarn`, `bun`)

---

### 1. 리포지토리 클론

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. 종속성 설치

프로젝트 루트 디렉터리에서 다음 명령어를 실행합니다:

```bash
npm install
```

### 3. 개발 서버 실행

```bash
npm run dev
```

실행 후 브라우저에서 [http://localhost:3000](http://localhost:3000)으로 접속하여 Vinyl을 확인하세요.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← 이전: 빠른 시작</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>다음: 환경 설정 →</strong></a>
</div>

---

*면책 조항: 이 문서는 내부 AI 자동화 프로세스를 통해 번역되었으며 오류나 부정확한 내용이 포함될 수 있습니다. 영어로 작성된 원본 문서가 공식 참조 기준입니다.*
