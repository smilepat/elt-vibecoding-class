---
project: elt-vibecoding-class
status: active
progress: 98
updated: 2026-06-10
pc: home-desktop
---

# elt-vibecoding-class — STATUS

## 🎯 한 줄 상태
영어교사 바이브코딩 슬라이드 2덱 + 데모·데이터·강의안까지 완성, GitHub public 배포 완료. 슬라이드 세부 다듬기 단계.

## 📦 결과물 (레포 구성)
- **슬라이드 2덱** (slides/) — 더블클릭/Chrome으로 실행, ←→·Space 이동·F 전체화면
  - `teacher_training.html` — 연수 덱 26장 (단어장 Part1 / 지문 Part2 6단계 실습 + 재사용 틀)
  - `new-workshop_생성AI_영어학습앱.html` — 3시간 워크샵 덱 **34장** (세션0~5 + 씨앗 3항목, 화면 목업 다수)
- **강의안 원천 md** (docs/) — 워크숍·강의안·WORKSHOP_생성AI 3종
- **동작 데모** (demos/) — 01_flashcard, 02_passage_vocab
- **데이터** (data/) — 어휘 CSV 2 + 지문 md + 표 뷰어 2
- **슬라이드 자산** — slides/mockups/(화면 목업 소스), slides/img/(스크린샷 PNG), slides/index_structure.html

## 📊 진행 체크리스트
- [x] 강의안·워크숍 자료(md 3종) 작성 + docs/ 정리
- [x] 실습 데이터 (어휘 CSV·지문) + 표 뷰어
- [x] 동작 HTML 데모 2종
- [x] 연수 덱(teacher_training) — 루프·6단계 실습·재사용 틀·메모장/저장 화면
- [x] 워크샵 덱(new-workshop) — 6세션 + 화면 목업(코드생성·메모장·저장·더블클릭·Netlify·구글시트·그래프DB)
- [x] 단어목록/CSV 다운로드·기획서 프롬프트·index.html 구조 시각화 등 세부 슬라이드
- [x] GitHub public 배포
- [ ] 실제 연수 진행 → 교사 피드백 반영 개정  ← 다음 위치

## ⏭️ 다음에 할 일 (Next Actions)
1. 남은 세션(특히 세션2 콘텐츠 생성·구글시트 붙여넣기)에 화면 목업 추가 검토
2. 실제 연수 진행 후 막힌 지점 기반으로 슬라이드/프롬프트 개정
3. (선택) GitHub Pages 켜서 슬라이드를 링크 클릭만으로 재생되게

## 🛠️ 다른 PC에서 이어서 작업하기
```bash
git clone https://github.com/smilepat/elt-vibecoding-class.git
cd elt-vibecoding-class
```
- **빌드 불필요** — 슬라이드는 단일 HTML. `slides/*.html`을 브라우저로 열면 끝.
- 슬라이드 편집: `slides/new-workshop_생성AI_영어학습앱.html` 또는 `teacher_training.html` 직접 수정.
- 화면 목업 추가/수정: `slides/mockups/*.html` 편집 → 헤드리스 브라우저로 `slides/img/*.png` 재캡처
  (예: `msedge --headless=new --screenshot=out.png --window-size=W,H file:///...`).
- ⚠️ PowerShell의 `Get-Content/Set-Content`로 슬라이드(UTF-8 BOM없음 한글)를 다루면 깨질 수 있음 → **Edit 도구/에디터로 직접 수정**.
- 작업 후: `git add -A && git commit && git push`.

## 🔗 Claude Code 재개 프롬프트
"STATUS.md 읽고 new-workshop 슬라이드 이어서 다듬자. (현재 34장, 세션0~5+씨앗 완성)"
