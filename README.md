# win-mini-agent 배포판

**이용 약관:** [약관.md](%EC%95%BD%EA%B4%80.md) (한국어, 우선) · **Terms of Use:** [TERMS.en.md](TERMS.en.md) (English translation; the Korean version prevails). 프로그램을 쓰기 전에 읽어 주세요.

회사 Windows PC에서 쓰는 작은 에이전트 도구의 **실행 파일 배포용** 저장소입니다. 소스 코드는 이곳에 없습니다.

- `win-mini-agent.exe` — API판 (API 키 사용)
- `win-mini-agent-codex.exe` — Codex판 (PC에 Codex CLI 설치와 `codex login` 필요)
- `release.json`, `release.json.minisig` — 파일 크기·SHA-256 목록과 그 서명. 프로그램의 업데이트 기능은 서명과 SHA-256이 모두 맞을 때만 설치합니다.
- `THIRD_PARTY_NOTICES.txt` — 함께 들어 있는 오픈소스 구성요소의 라이선스 전문
- `THIRD_PARTY_SKILLS.md` — 기본 스킬에 쓰인 제3자 글의 출처와 라이선스
- `약관.md`, `TERMS.en.md` — 이용 약관 (릴리스에는 `TERMS.ko.md`라는 이름으로 첨부: 내용은 `약관.md`와 같습니다)

설치는 없습니다. 원하는 폴더에 exe를 두고 실행합니다. 코드 서명 인증서가 없어 Windows가 경고를 띄울 수 있습니다.

**이용 조건:** 프로그램은 [약관.md](%EC%95%BD%EA%B4%80.md)에 따라 무료로 이용할 수 있습니다. 약관이 허락하지 않는 복제·재배포·수정은 할 수 없습니다. 오픈소스 구성요소는 각자의 라이선스를 따릅니다(`THIRD_PARTY_NOTICES.txt`, `THIRD_PARTY_SKILLS.md`).
