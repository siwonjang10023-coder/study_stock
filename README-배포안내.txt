STUDY STOCK — iPad 설치형 웹앱 파일

포함 파일
- index.html: 공부 기록 웹앱
- manifest.webmanifest: 홈 화면 설치 정보
- service-worker.js: 앱 파일 캐시 및 기본 오프라인 지원
- icon-192.png / icon-512.png: 앱 아이콘

무료 배포 권장: GitHub Pages
1. GitHub 계정으로 로그인하고 새 저장소(repository)를 만듭니다. 예: study-stock
2. 이 압축 파일을 풀고, 안의 파일 5개를 저장소 최상위(root)에 업로드합니다.
3. 저장소 Settings > Pages로 이동합니다.
4. Build and deployment에서 Deploy from a branch를 선택합니다.
5. Branch를 main, 폴더를 /(root)로 선택하고 Save를 누릅니다.
6. 배포가 끝나면 https://사용자이름.github.io/study-stock/ 형태의 주소가 생깁니다.
   실제 주소는 GitHub Pages 화면에 표시된 것을 사용하세요.
7. 아이패드에서 Safari로 그 HTTPS 주소를 엽니다.
8. 공유 버튼 > 홈 화면에 추가 > '웹 앱으로 열기'를 켜고 추가합니다.

기록 저장 방식
- 현재 앱은 localStorage를 사용하므로 기록은 해당 브라우저/기기의 저장 공간에 저장됩니다.
- 앱 파일을 인터넷에 배포하는 것만으로 기기 간 동기화는 되지 않습니다.
- Safari 웹사이트 데이터 삭제 시 기록이 사라질 수 있으므로 앱 안의 CSV 내보내기로 백업하세요.
- 오프라인 캐시는 앱 화면 파일을 저장할 뿐, 기록을 클라우드에 백업하지 않습니다.
- 여러 기기 동기화가 필요하면 이후 Firebase/Supabase 같은 백엔드와 사용자 인증을 별도로 연결해야 합니다.

주의
- 공개 GitHub 저장소에 올리는 것은 앱의 소스 코드가 공개될 수 있다는 뜻입니다. 공부 기록은 HTML 코드에 들어 있지 않고 각 기기의 브라우저 저장 공간에 남지만, 공개 웹사이트에 개인정보를 입력하지 마세요.
- GitHub Pages 배포는 자동으로 즉시 완료된다고 보장할 수 없습니다. GitHub Pages 화면의 배포 상태와 실제 URL을 확인하세요.
