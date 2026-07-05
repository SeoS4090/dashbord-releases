<div align="center">

# 🧩 Dashbord

**나만의 윈도우 데스크톱 대시보드 위젯 앱**

시계·달력·날씨·출퇴근·미디어·블루투스·주식/코인/환율·Claude 사용량·게임 정보까지,
바탕화면에 **Rainmeter 스타일로 떠 있는 위젯**으로 모아 봅니다.

<br>

[![release](https://img.shields.io/github/v/release/SeoS4090/dashbord-releases?style=flat-square&color=6d28d9&label=release)](https://github.com/SeoS4090/dashbord-releases/releases/latest)
[![downloads](https://img.shields.io/github/downloads/SeoS4090/dashbord-releases/total?style=flat-square&color=059669&label=downloads)](https://github.com/SeoS4090/dashbord-releases/releases)
![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?style=flat-square&logo=windows&logoColor=white)
![Tauri 2](https://img.shields.io/badge/Tauri-2-24C8DB?style=flat-square&logo=tauri&logoColor=white)

</div>

<!--
  💡 스크린샷을 넣으면 Home이 훨씬 살아납니다.
  이 저장소에 assets/screenshot.png 를 올린 뒤 아래 한 줄의 주석을 풀어 주세요:
  <p align="center"><img src="assets/screenshot.png" alt="Dashbord 미리보기" width="820"></p>
-->

---

## ✨ 한눈에

- **떠 있는 오버레이** — 각 위젯은 테두리 없는 투명 창. 바탕화면 위에 자연스럽게 얹히고, 평소엔 조작 UI가 숨어 방해되지 않습니다.
- **카테고리** — 위젯은 **LIFE(생활) · GAME(게임) · DEV(개발)** 로 나뉩니다.
- **한국 중심** — 버스 도착·공휴일·미세먼지(공공데이터포털), 주식/환율(네이버·하나은행 고시), 코인(업비트), 로또(동행복권) 등 **국내 실시간 데이터** 위주.
- **트레이 상주** — 메인 창은 숨겨져 있고 작업 표시줄 트레이로 동작. 창을 모두 닫아도 앱은 트레이에 남습니다.

> 코드 서명이 없는 **개인용 앱**입니다. 회사 배포용이 아니며, 데이터는 모두 내 PC에만 저장됩니다 ([데이터 저장](guide/데이터-저장.md) 참고).

---

## 🚀 설치 (30초)

1. [**Releases**](https://github.com/SeoS4090/dashbord-releases/releases) 에서 `dashbord_X.Y.Z_x64-setup.exe` 를 받아 실행합니다.
2. **"Windows의 PC 보호(SmartScreen)"** 경고가 뜨면 → `추가 정보` → `실행`. (서명 없는 개인용 앱이라 처음 한 번만)
3. 트레이에 아이콘이 뜨면 끝. **더블클릭 → 설정**에서 원하는 위젯을 켜세요.

> 업데이트는 앱 안에서 자동으로 처리됩니다. · 자세한 안내는 **[설치 및 시작](guide/설치-및-시작.md)** 참고.

---

## 🧩 위젯 한눈에

> ✅ 바로 사용 · 🔑 공공데이터포털 키 · 🔗 계정/OAuth 연결

| 카테고리 | 위젯 |
|---|---|
| **LIFE** | 대시보드 · 시계 · 타이머 · 캘린더 · 출퇴근 · 버스 도착 · 날씨 · 메모 · D-Day · 런처 · 코인 · 뉴스(RSS) · 주식 · 로또 · 환율 · 사운드 믹서 · 미디어 · 블루투스 · YouTube · YouTube Music · X |
| **GAME** | Tarkov · 치지직 · Steam(특가·가격·뉴스·동접) · 데스크톱 펫 |
| **DEV** | 사용량(Claude) · 시스템 · Jira 칸반 · Idle Game · GitHub 트렌딩 · Hacker News |

전체 설명과 필요한 연동은 **[위젯 카탈로그](guide/위젯-카탈로그.md)** 에서 확인하세요.

---

## 📖 문서

| 문서 | 내용 |
|---|---|
| 🚀 **[설치 및 시작](guide/설치-및-시작.md)** | 다운로드·설치·5분 시작 가이드·기본 사용법(편집 모드·단축키·대시보드·트레이) |
| 🧩 **[위젯 카탈로그](guide/위젯-카탈로그.md)** | LIFE·GAME·DEV 전체 위젯과 각자 필요한 연동 |
| 🔌 **[연동 설정](guide/연동-설정.md)** | 공공데이터포털 · Google 캘린더 · Jira · 계정 로그인 · Claude 사용량 |
| 🔒 **[데이터 저장](guide/데이터-저장.md)** | 무엇이 어디에 저장되는지 · 개인정보 · 보안 |
| ❓ **[FAQ / 문제 해결](guide/FAQ.md)** | 자주 묻는 질문과 해결 방법 |

---

## 🛠️ 개발자 / 소스

Tauri 2 (Rust) + React + TypeScript + Vite + Tailwind 로 만들어졌습니다.

- **소스 코드**(빌드·실행·아키텍처·기여): 비공개 저장소 [`SeoS4090/dashbord`](https://github.com/SeoS4090/dashbord)
- **설치본 · `latest.json`(자동 업데이트)**: 이 공개 저장소의 [Releases](https://github.com/SeoS4090/dashbord-releases/releases). 소스에서 버전 태그를 푸시하면 GitHub Actions가 빌드·배포하고, 이 README와 `guide/` 문서도 함께 동기화합니다.

---

<div align="center">
<sub>Dashbord · Windows 데스크톱 위젯 대시보드 · 1인 개인 프로젝트</sub>
</div>
