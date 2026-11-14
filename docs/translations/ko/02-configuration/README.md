# 환경 설정

Vinyl의 환경 변수 및 외부 서비스 연동 설정 방법.

### 환경 변수 설정

프로젝트 루트 디렉터리에 `.env` 파일을 생성하고 다음 변수를 추가합니다:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### YouTube API 키 발급 방법

1. [Google Cloud Console](https://console.cloud.google.com/)에 접속하여 **API 및 서비스**로 이동합니다.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. 왼쪽 사이드바 메뉴에서 **라이브러리**를 클릭합니다.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. **YouTube Data API v3**를 검색하고 카탈로그에서 선택한 후 **사용 설정**을 클릭합니다.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. API가 활성화되면 왼쪽 메뉴의 **사용자 인증 정보**로 이동하여 **+ 사용자 인증 정보 만들기**를 누르고 **API 키**를 선택합니다.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. **API 키 만들기** 패널에서 설정을 구성하고 **만들기**를 클릭합니다:
   - **이름:** 식별하기 쉬운 이름 입력 (예: `vinyl-key`).
   - **키로 액세스할 수 있는 API:** API 제한사항에서 **YouTube Data API v3**를 선택합니다.
   - **애플리케이션 제한사항:** **없음**으로 유지합니다.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. 생성된 API 키를 복사하여 `.env` 파일의 `YOUTUBE_API_KEY`에 입력합니다:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud는 YouTube Data API에 대해 로컬 개발 및 개인 용도로 충분한 일일 무료 할당량을 제공합니다.

<div align="left">
  <a href="../01-installation/README.md"><strong>← 이전: 설치</strong></a>
</div>

---

*면책 조항: 이 문서는 내부 AI 자동화 프로세스를 통해 번역되었으며 오류나 부정확한 내용이 포함될 수 있습니다. 영어로 작성된 원본 문서가 공식 참조 기준입니다.*
