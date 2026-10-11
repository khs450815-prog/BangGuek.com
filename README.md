# 상중하초 처방 찾기 — 웹앱 설치 안내

## 들어 있는 파일
- index.html : 프로그램 본체 (증상 판, 처방 카드, 方極·조문·藥徵 자료 포함)
- cases.json : 의안 자료 (임상 의안, 類聚方新解 치험). 의안만 바꿀 때는 이 파일만 다시 올리면 됩니다.
- manifest.webmanifest : 앱 이름(삼초처방), 아이콘, 색상
- sw.js : 오프라인 실행
- icons/ : 앱 아이콘

다섯 가지를 폴더 구조 그대로 한 곳에 올립니다.

## GitHub Pages에 올리기 (무료)
1. github.com 에서 New repository → 이름 예: `samcho` → Public → Create.
2. "uploading an existing file"을 눌러 압축을 푼 파일과 icons 폴더를 통째로 끌어다 놓고 Commit changes.
3. Settings → Pages → Branch: main, / (root) → Save.
4. 1~2분 뒤 `https://아이디.github.io/samcho/` 주소가 생깁니다.

기존 방극 앱 저장소(`fangji`)와 별개로 올리면 두 앱을 따로 설치해 쓸 수 있습니다.

## 설치
- 안드로이드(크롬): 화면 위 「앱으로 설치」 버튼, 또는 메뉴 ⋮ → 홈 화면에 추가
- 아이폰(사파리): 공유 → 홈 화면에 추가
- PC(크롬·엣지): 주소창 오른쪽 설치 아이콘

처음 한 번 인터넷에 연결된 상태로 열면, 이후에는 오프라인에서도 한자 글꼴까지 작동합니다.

## 내용을 고쳤을 때
1. 새 index.html 을 저장소에 같은 이름으로 다시 올립니다.
2. sw.js 첫 줄의 `samcho-v4` 숫자를 하나 올려 함께 올립니다.
3. 앱을 한두 번 다시 열면 새 버전으로 바뀝니다.
