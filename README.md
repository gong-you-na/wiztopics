# WizTopics — 위즈덤투스 데일리 토픽 보드

매일 07:00 KST 전에 예약 작업이 `data/YYYY-MM-DD.json`을 만들어 푸시하고, Netlify가 자동 배포합니다. (https://wiztopics.netlify.app)

- `index.html` / `app.js` / `style.css` — 페이지(토스증권 UI 톤). `data/*.json`을 읽어 렌더. 예약 작업은 수정하지 않음.
- `data/index.json` — 날짜 목록. `data/latest.json` — 최신 하루치. `data/YYYY-MM-DD.json` — 하루치(스키마는 `AUTOMATION.md`).
- `assets/` — 서명 로고.
- 시세·학습기업 실적 데이터는 [market-calendar(WizView)](https://github.com/gong-you-na/market-calendar) 저장소의 `data/*.json`을 읽기 전용으로 재사용.

로컬 확인: `python3 -m http.server 8787` → http://localhost:8787
