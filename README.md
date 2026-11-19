# win-mini-agent 배포판

회사 Windows PC에서 쓰는 작은 에이전트 도구의 **실행 파일 배포용** 저장소입니다. 소스 코드는 이곳에 없습니다.

- `win-mini-agent.exe` — API판 (API 키 사용)
- `win-mini-agent-codex.exe` — Codex판 (PC에 Codex CLI 설치와 `codex login` 필요)
- `release.json`, `release.json.minisig` — 파일 크기·SHA-256 목록과 그 서명. 프로그램의 업데이트 기능은 서명과 SHA-256이 모두 맞을 때만 설치합니다.
- `THIRD_PARTY_NOTICES.txt` — 함께 들어 있는 오픈소스 구성요소의 라이선스 전문

설치는 없습니다. 원하는 폴더에 exe를 두고 실행합니다. 코드 서명 인증서가 없어 Windows가 경고를 띄울 수 있습니다.

**라이선스 없음:** 이 저장소에는 라이선스 파일이 없습니다. 따라서 저작권법의 기본 규칙에 따라 모든 권리는 저작자에게 있으며, 받은 분은 본인 사용 외에 복제·재배포·수정할 수 없습니다. 오픈소스 구성요소는 각자의 라이선스를 따릅니다(`THIRD_PARTY_NOTICES.txt`).
