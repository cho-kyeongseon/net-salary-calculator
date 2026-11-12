# CLAUDE.md

## 작업 규칙

- 작업 폴더는 USB이고, GitHub는 백업과 Vercel 배포용이다.
  - 저장소: https://github.com/cho-kyeongseon/net-salary-calculator
  - 배포: https://net-salary-calculator-opal.vercel.app (`main`에 푸시하면 자동 배포)
- 기본 작업 브랜치는 `main`. 다른 브랜치는 요청할 때만 쓴다.
- 작업이 한 단락 끝나면 `HANDOFF.md`를 업데이트한다.

## 프로젝트 메모

- 앱은 `index.html` 한 파일(HTML·CSS·JS, 간이세액표 데이터 내장)이다. 외부 파일을 읽지 않으므로 드라이브 문자와 무관하게 동작한다.
- 앞으로 원본 자료 파일을 읽게 되면 반드시 작업 폴더 기준 상대 경로(예: `./data/...`)를 쓰고, `E:\` 같은 절대 경로를 쓰지 않는다.
- 원본 자료와 큰 파일은 `.gitignore`로 GitHub에 올리지 않는다.
