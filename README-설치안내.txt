술로그 PWA - 갤럭시 S25 설치 안내

중요: ZIP 또는 index.html 파일을 갤럭시에서 직접 여는 것만으로는 PWA 설치 및 오프라인 캐시가 동작하지 않습니다. HTTPS 주소에 파일 전체를 배포해야 합니다.

PC 없이 배포하는 한 가지 방법 (GitHub 웹사이트 이용):
1. 갤럭시 Chrome에서 github.com 접속 후 로그인합니다.
2. 새 PUBLIC 저장소를 만들고, 이 ZIP을 압축 해제한 뒤 index.html, sw.js, manifest.webmanifest, icons 폴더를 저장소 최상위에 업로드합니다. (GitHub 모바일 웹에서 Add file > Upload files 메뉴를 사용; 데스크톱 사이트 보기가 필요할 수 있습니다.)
3. 저장소 Settings > Pages > Build and deployment > Deploy from a branch > main / (root) > Save.
4. GitHub Pages가 배포한 HTTPS 주소(https://사용자명.github.io/저장소명/)를 Chrome에서 방문합니다.
5. Chrome 메뉴(⋮) > 홈 화면에 추가 > 설치(또는 바로가기 추가)를 선택합니다.
6. 온라인 상태에서 한 번 완전히 연 후 비행기 모드에서 재실행해 오프라인 동작을 확인합니다.

주의사항:
- 공개 저장소에는 앱 코드만 올라갑니다. 음주 기록은 브라우저 기기 내부(localStorage)에만 저장되며 GitHub로 업로드되지 않습니다.
- Chrome의 사이트 데이터 삭제, 앱 제거, 브라우저 변경 시 기록이 사라질 수 있습니다. 앱 내 백업 JSON을 정기적으로 다운로드하세요.
- 다른 주소/브라우저에서 만든 이전 기록은 자동으로 이전되지 않습니다. 기존 술로그에서 JSON 백업 후 새 주소에서 가져오세요.
- 홈 화면에 추가 메뉴의 명칭과 위치는 Chrome 버전에 따라 다릅니다.
- GitHub Pages는 배포된 파일을 공개하므로 개인정보나 백업 JSON은 업로드하지 마세요.
