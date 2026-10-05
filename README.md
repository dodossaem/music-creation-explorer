# 중학교 음악 창작 탐색기

Gemini 공유 대화([음악 창작 탐색기](https://gemini.google.com/share/fd40c90aaa1b))를 바탕으로 만든 **교육용 웹앱**입니다.

학생들이 악기 음색·장조/단조·코드 진행을 직접 들어보고, 표현하고 싶은 장면에 맞는 악기와 화성을 고를 수 있습니다.

## 바로 열기 (GitHub Pages)

👉 **https://dodossaem.github.io/music-creation-explorer/**

링크만 공유하면 다른 사람도 바로 사용할 수 있습니다.

## 로컬 실행

브라우저의 `file://` 로 열면 일부 환경에서 로컬 MP3 로딩이 막힐 수 있습니다. 아래처럼 간단 서버를 켜세요.

```bash
cd /Users/rw.ko/music-creation-explorer
python3 -m http.server 8080
```

브라우저에서 [http://localhost:8080](http://localhost:8080) 접속.

## 구성

- `index.html` — 앱 본체
- `vendor/Tone.js` — 오디오 엔진
- `samples/` — Philharmonia Orchestra 계열 로컬 MP3
  - violin, viola, cello, double-bass, flute, clarinet, trumpet, french-horn, guitar
  - 피아노는 Tone.js 합성음으로 재생

## 기능

1. **악기 음색 탐색** — 단음/화음, 짧은 멜로디, 최대 4개 악기 비교 연주
2. **조성·코드 진행 탐색** — C 장조/단조, 대표 코드 진행 듣기
3. **나의 음악 설계 활동지** — 장면·분위기·악기·화성 정리
