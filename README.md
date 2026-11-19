# Care Street · GitHub Pages 배포 파일

이 폴더는 GitHub Pages에서 바로 실행할 수 있도록 구성된 정적 웹사이트입니다.

## 포함 파일

- `index.html`: Care Street 프로토타입 메인 페이지
- `assets/images/`: HTML에서 분리한 화면 이미지 및 그래픽(WebP)
- `assets/fonts/SUIT.woff2`: SUIT 글꼴
- `.nojekyll`: GitHub Pages의 기본 Jekyll 처리를 비활성화

## 기존 GitHub 저장소에 적용하기

1. 이 ZIP 파일의 압축을 풉니다.
2. 압축을 푼 폴더 안의 `index.html`, `assets` 폴더, `.nojekyll`, `README.md`를 기존 `Carestreet` 저장소의 **최상위(root)** 에 업로드합니다.
3. 기존 `index.html`이 있으면 새 파일로 교체하고, `assets` 폴더도 함께 업로드합니다.
4. `Commit changes`를 눌러 저장합니다.
5. 저장소의 **Settings → Pages**에서 배포 설정이 `Deploy from a branch` / `main` / `/(root)`인지 확인합니다.

기존 저장소 주소 형식을 유지하면 공개 주소는 다음과 같습니다.

`https://care-street.github.io/Carestreet/`

## 용량 및 로딩 최적화

- 원본 이미지 픽셀 크기는 유지하고, 전송 효율이 높은 WebP로 변환했습니다.
- 이미지와 글꼴을 별도 파일로 분리해 HTML 자체 크기를 줄였습니다.
- 시작 화면과 다음 안내 화면, 글꼴에 preload 힌트를 추가했습니다.
- 글꼴은 `font-display: swap`으로 설정하고, 시작 화면 자동 전환 대기 시간을 0.8초로 조정했습니다.

## 참고

이 프로토타입의 기록은 기본적으로 사용자의 브라우저 로컬 저장소에 저장되는 시연 데이터입니다. 실제 계정, 의료 데이터 연동, 푸시 알림 등은 별도 서비스와 연결되어 있지 않습니다.
