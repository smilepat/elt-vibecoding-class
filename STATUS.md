---
project: elt-vibecoding-class
status: active
progress: 99
updated: 2026-06-11
pc: home-desktop
---

# elt-vibecoding-class — STATUS

## 🎯 한 줄 상태
영어교사 바이브코딩 슬라이드 2덱 + 배포 앱(단어가족) + 강의안까지 완성, GitHub public·Netlify 배포 완료. 슬라이드 세부 다듬기 단계.

## 📦 결과물 (레포 구성)
- **슬라이드 2덱** (slides/) — 더블클릭/Chrome 실행, ←→·Space 이동·F 전체화면
  - `teacher_training.html` — 연수 덱 26장 (단어장 Part1 / 지문 Part2 6단계 실습 + 재사용 틀)
  - `new-workshop_생성AI_영어학습앱.html` — 3시간 워크샵 덱 **36장** (세션0~5 + 씨앗 3항목, 화면 목업 다수)
- **배포 앱** (apps/) — `word-family/index.html` 단어가족(굴절어·파생어 구분), Netlify 배포: https://ephemeral-smakager-27ae4e.netlify.app/
- **강의안 원천 md** (docs/) — 워크숍·강의안·WORKSHOP_생성AI 3종
- **동작 데모** (demos/) — 01_flashcard, 02_passage_vocab
- **데이터** (data/) — 어휘 CSV 2 + 지문 md + 표 뷰어 2
- **슬라이드 자산** — slides/mockups/(화면 목업 소스), slides/img/(스크린샷 PNG), slides/index_structure.html

## 📊 진행 체크리스트
- [x] 강의안·워크숍 자료(md 3종) + docs/ 정리
- [x] 연수 덱(teacher_training) 26장
- [x] 워크샵 덱(new-workshop) 36장 — 세션0~5 화면 목업 + 씨앗 3항목
- [x] 세션별 세부 개선: 기획서 프롬프트(자연어)·콘텐츠 3축 프레임워크·구조 시각화·말로 고치기 표·회원가입/배포 화면
- [x] 단어가족 앱 제작 + Netlify 배포
- [x] GitHub public 배포
- [ ] 실제 연수 진행 → 교사 피드백 반영 개정  ← 다음 위치

## ⏭️ 다음에 할 일 (Next Actions)
1. 세션2 "콘텐츠 만들기" 단어 CSV·구글시트 붙여넣기 화면 목업 추가 검토
2. 실제 연수 진행 후 막힌 지점 기반 슬라이드/프롬프트 개정
3. (선택) GitHub Pages 켜서 슬라이드를 링크 클릭만으로 재생

## 🛠️ 다른 PC에서 이어서 작업하기
```bash
git clone https://github.com/smilepat/elt-vibecoding-class.git
cd elt-vibecoding-class
```
- **빌드 불필요** — 슬라이드·앱 모두 단일 HTML. 브라우저로 열면 끝.
- 슬라이드 편집: `slides/new-workshop_생성AI_영어학습앱.html` (현재 36장) 또는 `teacher_training.html` 직접 수정.
- 슬라이드 1장만 검증 캡처: `<script>`의 `show(0)`을 `show(N)`으로 잠깐 바꿔 헤드리스 캡처 → 다시 `show(0)`.
- 화면 목업 추가/수정: `slides/mockups/*.html` 편집 → 헤드리스 브라우저로 `slides/img/*.png` 재캡처
  (`msedge --headless=new --screenshot=out.png --window-size=W,H file:///...`). 한글 깨지면 캡처 높이/창크기 조정.
- ⚠️ PowerShell `Get-Content/Set-Content`로 슬라이드(UTF-8 BOM없음 한글)를 다루면 깨짐 → **Edit 도구/에디터로 직접 수정**.
- 작업 후: `git add -A && git commit && git push`.
- ⚠️ 메모리의 Chrome 경로(`D:\Program Files\...`)는 이 PC 전용 — 다른 PC는 경로 다를 수 있음.

## 🔗 Claude Code 재개 프롬프트
"STATUS.md 읽고 new-workshop 슬라이드(현재 36장) 이어서 다듬자."
