# 웃는 거북이 개인 홈페이지 예제

Home / About / Project / Publication 메뉴가 있는 단일 페이지입니다.
메뉴를 누르면 같은 페이지 안의 해당 섹션으로 이동합니다.
별도 설치, npm, 빌드, API 키가 필요 없습니다.
첫 화면은 AI로 생성한 웃는 거북이 그림입니다.
소개와 프로젝트, 논문은 모두 교체용 예시입니다.

## 1. 내 컴퓨터에서 확인

압축을 푼 후 index.html을 Chrome 또는 Edge로 여세요.
assets 폴더를 index.html과 같은 폴더에 유지하세요.

## 2. GitHub Pages로 공개

1. GitHub에 로그인합니다.
2. 새 Public 저장소를 만들고 이름을 `portfolio-demo`로 지정합니다. README 추가를 선택하면 main 브랜치가 생성됩니다.
3. 저장소에서 Add file → Upload files를 누릅니다.
4. 압축을 푼 폴더 내부의 index.html, assets 폴더, README.md를 업로드합니다. ZIP 자체나 바깥 github-pages-example 폴더를 올리는 것이 아닙니다.
5. Commit changes를 누릅니다.
6. Settings → Pages → Build and deployment로 이동합니다.
7. Source = Deploy from a branch, Branch = main, Folder = /(root)로 선택하고 Save를 누릅니다.
8. 배포가 끝나면 Pages 화면에 표시되는 주소로 접속합니다. 진행 상태는 Actions에서도 확인할 수 있습니다.

주소 형식: https://GITHUB_ID.github.io/portfolio-demo/
예를 들어 ikwak2 계정의 portfolio-demo 저장소라면 https://ikwak2.github.io/portfolio-demo/ 입니다. 이 주소는 설명용이며 실제 배포된 주소가 아닙니다.

계정의 대표 홈페이지를 처음 만드는 경우에는 저장소 이름을 GITHUB_ID.github.io로 만들 수 있습니다.
이미 대표 홈페이지가 있다면 실습은 portfolio-demo처럼 별도 저장소를 이용하세요.
기존 대표 홈페이지 저장소에 예제 파일을 덮어쓰지 마세요.

## 3. 수정하는 곳

- 이름: index.html의 Your Name을 전체 검색하여 변경
- 소개: id="about" 섹션
- 프로젝트: id="project" 섹션의 article들
- 논문: id="publication" 섹션의 li들
- 배경: assets/turtle-hero.png를 교체하거나 img의 src 경로 수정
- 색상: style 맨 위의 :root 변수
- 그림 설명: img의 alt도 새 그림에 맞게 변경

사진이 세로로 길다면 .hero img의 object-position을 조절하세요.
모바일 화면에서는 사진 일부가 잘리는 것이 정상입니다.
큰 이미지는 배포 전에 용량을 줄이면 로딩이 빨라집니다.

## 4. 수정 내용 반영

GitHub에서 index.html을 열고 연필 버튼으로 수정한 뒤 Commit changes를 누르면 재배포됩니다.
AI에게 파일을 수정하게 한 경우에는 수정된 파일을 같은 경로로 업로드하여 교체합니다.
배포 완료 후에도 이전 화면이 보이면 Ctrl+F5로 새로고침하세요.

## 5. AI에게 수정 요청하는 예시

“첨부한 index.html의 레이아웃과 Home, About, Project, Publication 메뉴는 유지하고,
Your Name을 홍길동으로 바꿔줘. About에는 다음 소개를 넣어줘: [...].
프로젝트 3개는 다음 내용으로 바꿔줘: [...].
GitHub Pages의 하위 경로에서도 사진과 링크가 작동하도록 상대 경로를 유지해줘.
수정된 전체 HTML 파일을 제공해줘.”

## 참고

디자인 참고: https://charlesemogor.com/
원본 사이트의 코드나 사진을 복사하지 않고, 큰 배경과 상단 메뉴 구성을 참고해 만든 예제입니다.
공식 안내: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
