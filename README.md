# Care Street · GitHub Pages 배포 파일

이 폴더는 GitHub Pages에서 바로 실행할 수 있도록 구성된 정적 웹사이트입니다.

## 포함 파일

- `index.html`: Care Street 프로토타입 메인 페이지
- `assets/images/`: 화면 이미지 및 그래픽(WebP)
- `assets/fonts/SUIT.woff2`: SUIT 글꼴
- `.nojekyll`: GitHub Pages의 기본 Jekyll 처리를 비활성화

## 기존 GitHub 저장소에 적용하기

1. 이 ZIP 파일의 압축을 풉니다.
2. 폴더 안의 `index.html`, `assets` 폴더, `.nojekyll`, `README.md`를 기존 `Carestreet` 저장소의 최상위(root)에 업로드합니다.
3. 기존 파일은 새 파일로 교체하고, `assets` 폴더도 함께 유지합니다.
4. `Commit changes`를 눌러 저장합니다.
5. 저장소의 **Settings → Pages**에서 `Deploy from a branch` / `main` / `/(root)` 설정을 확인합니다.

공개 주소: `https://care-street.github.io/Carestreet/`

## 로딩 개선

- 화면 이동 전에 해당 화면에서 사용할 주요 이미지를 미리 불러오고 디코딩합니다.
- 다음 화면이 준비되는 동안 현재 화면을 유지해 탭 전환 시 흰 화면이 먼저 나타나는 현상을 줄입니다.
- 화면에 필요한 이미지(기본 화면, 하단 메뉴, 연결된 후속 화면, 홈 화면 템플릿 등)를 함께 준비합니다.
- 이미 불러온 이미지는 브라우저 내 캐시를 재사용합니다.
- 이미지 픽셀 크기는 유지하고 WebP로 변환해 전송 용량을 줄였습니다.

## 참고

이 프로토타입의 시연 기록은 브라우저 로컬 저장소에 저장됩니다. 실제 계정, 의료 데이터 연동, 푸시 알림 등은 별도 서비스와 연결되어 있지 않습니다.
