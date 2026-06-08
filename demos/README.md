# 🖥️ demos — 동작하는 예제 앱

강사 시연 및 참가 교사 "정답 코드 스냅샷"용 예제 앱입니다.
**설치 불필요** — 파일을 더블클릭하면 브라우저에서 바로 동작합니다.

| 파일 | 연계 자료 | 기능 |
|------|-----------|------|
| [01_flashcard.html](01_flashcard.html) | 워크숍(단어장 기반) | 플래시카드 플립 · 4지선다 퀴즈 · 간격반복 복습(localStorage) |
| [02_passage_vocab.html](02_passage_vocab.html) | 강의안(지문 기반) | 원문/빈칸 토글 · 채점 · 힌트 · 문맥추론 · 복습카드 |

## 사용법
1. 파일을 더블클릭 → 브라우저에서 열림
2. 그대로 학생에게 보여주거나, **Netlify Drop**에 올려 링크로 배포

## 데이터 교체 방법 (강의 핵심)
두 파일 모두 `<script>` 안에 **`⬇⬇⬇ 여기만 바꾸면 ⬇⬇⬇`** 주석으로 표시된 구역이 있습니다.
- `01_flashcard.html` → `VOCAB` 배열 (단어·뜻·예문)
- `02_passage_vocab.html` → `PASSAGES` 배열 (지문 text의 `**단어**` 가 빈칸이 됨)

원본 데이터는 [`../data/`](../data/) 폴더 참고:
- [sample_vocab_40.csv](../data/sample_vocab_40.csv) — 단어장 황금표준 40단어
- [sample_passages.md](../data/sample_passages.md) — 지문 3편(원문→빈칸→Word Bank→타겟)
