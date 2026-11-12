# HANDOFF

## 2026-11-12 USB 폴더 ↔ GitHub 연동 점검

- USB 폴더는 이미 `origin = cho-kyeongseon/net-salary-calculator`, 브랜치 `main`으로 연결돼 있음.
- GitHub `main`이 2커밋 앞서 있음(README.md 추가, PR #1). `index.html` 내용은 줄바꿈(CRLF/LF) 차이 외에 동일.
- 이 PC에 Git 2.56 설치(winget). USB는 소유권 기록이 없는 파일 시스템이라 `safe.directory`에 이 폴더를 등록함.
- `git pull --ff-only`로 README.md 받음 → 로컬 `main` = `origin/main`.
- 추가한 파일: `.gitignore`, `CLAUDE.md`, `HANDOFF.md` → 커밋 후 `main`에 푸시.
- Vercel: 이미 연결돼 있음(GitHub 커밋 상태에 Vercel success). 사이트 https://net-salary-calculator-opal.vercel.app 응답 200 확인.

### 참고
- 다른 PC에서 이 USB로 작업할 때 Git이 없으면 설치하고, "dubious ownership" 오류가 나면
  `git config --global --add safe.directory "<이 폴더 경로>"`를 한 번 실행한다.
