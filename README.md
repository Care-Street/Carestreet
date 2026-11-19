# Care Street 프로토타입 (GitHub Pages)

GitHub Pages 배포용 정적 웹사이트입니다.

## 업로드 방법
1. GitHub에서 새 저장소(Repository)를 만들고 `Public`으로 설정합니다.
2. 이 ZIP을 컴퓨터에서 압축 해제합니다.
3. 압축 해제 폴더 안의 `index.html`, `assets` 폴더, `.nojekyll`, `README.md`를 저장소 최상위(root)에 업로드합니다. ZIP 파일 자체를 사이트 파일로 올리는 것이 아닙니다.
4. 저장소의 **Settings → Pages**에서 **Deploy from a branch**를 선택합니다.
5. Branch는 `main`, Folder는 `/(root)`로 지정하고 **Save**를 누릅니다.
6. Pages 설정 화면에 표시되는 공개 주소로 접속합니다.

## 구성
- `index.html`: 프로토타입과 인터랙션
- `assets/images/`: 화면 이미지 및 그래픽(WebP)
- `assets/fonts/`: SUIT 글꼴
- `.nojekyll`: GitHub Pages 정적 파일 처리 설정

이미지는 WebP 품질 86으로 변환했으며, 원본 픽셀 크기는 유지했습니다.
