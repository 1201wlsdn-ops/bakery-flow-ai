BAKERY FLOW AI 무료 배포 안내 (GitHub Pages)
================================================

포함 파일
- index.html             기존 앱 + 음성 알림 + PWA 연결
- manifest.webmanifest   휴대폰 홈 화면 설치 정보
- service-worker.js      오프라인 앱 화면 캐시
- icon.svg               앱 아이콘

무료 공개 방법
1. GitHub 계정에 로그인합니다.
2. New repository를 누릅니다.
3. Repository name에 bakery-flow-ai 를 입력합니다.
4. Public을 선택하고 Create repository를 누릅니다.
5. Add file > Upload files를 선택합니다.
6. 이 폴더 안의 파일 4개(index.html, manifest.webmanifest,
   service-worker.js, icon.svg)를 업로드하고 Commit changes를 누릅니다.
7. 저장소의 Settings > Pages로 이동합니다.
8. Build and deployment에서 Deploy from a branch를 선택합니다.
9. Branch는 main, 폴더는 /(root)를 선택하고 Save를 누릅니다.
10. 잠시 후 https://계정이름.github.io/bakery-flow-ai/ 주소가 생성됩니다.

QR 만들기
- 위 주소가 실제로 공개된 뒤에만 QR을 생성해야 합니다.
- QR에 저장할 주소는 반드시 https://계정이름.github.io/bakery-flow-ai/ 입니다.
- 배포 URL을 확인한 뒤 QR 이미지로 만들 수 있습니다.

휴대폰 설치
- iPhone: Safari로 주소 접속 > 공유 > 홈 화면에 추가
- Android: Chrome으로 주소 접속 > 메뉴 > 앱 설치 또는 홈 화면에 추가
- 첫 실행 후 화면을 한 번 터치하고 설정에서 음성 알림을 켜고 테스트하세요.

중요한 제한
- GitHub Pages는 정적 웹 호스팅입니다. 앱 데이터는 각 기기의 브라우저에 저장됩니다.
  서로 다른 휴대폰/직원 간 업무 데이터가 자동 공유되지는 않습니다.
- 데이터 공유가 필요하면 Firebase 등 별도 DB와 사용자 인증 연동이 필요합니다.
- 음성 알림은 앱이 실행 중이고 브라우저가 동작하는 동안의 기능입니다.
  모바일 OS가 앱을 백그라운드에서 정지하거나 기기가 절전/잠금 상태이면
  정해진 시각의 음성 재생을 보장할 수 없습니다.
- 음성 합성은 브라우저 정책상 최초 사용자 터치가 필요할 수 있습니다.
