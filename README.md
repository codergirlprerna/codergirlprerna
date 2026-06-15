<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=6366f1&height=130&section=header&text=Prerna%20Khanna&fontSize=46&fontColor=ffffff&fontAlignY=65&desc=Full-Stack%20Developer%20·%20MCA%20%2726%20·%20757%20contributions%20this%20year&descAlignY=85&descSize=14" width="100%"/>
</div>

<p align="center">
  <a href="https://linkedin.com/in/codergirlprerna">
    <img src="https://img.shields.io/badge/LinkedIn-codergirlprerna-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://cricsense.in">
    <img src="https://img.shields.io/badge/CricSense-🟢 Live-22c55e?style=for-the-badge"/>
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=codergirlprerna&style=for-the-badge&color=6366f1&label=PROFILE+VIEWS"/>
</p>

---

## About Me

Full-stack developer building complete products — schema to deployment. Currently in my second year of MCA and running **[CricSense](https://cricsense.in)** live in production: an AI-powered cricket platform with real-time ball-by-ball scoring, Gemini match narratives, and weather-aware predictions across 30 REST endpoints.

I work across the entire stack — Spring Boot APIs, React frontends, Firebase real-time sync, Redis caching, and Railway/Vercel deployment. When things break in production, I debug them.

> 757 contributions in 2026 · 33 commits across 11 repositories in June alone

---

## 🚀 Featured — [CricSense](https://cricsense.in) &nbsp; `🟢 Live`

AI-powered IPL prediction & live score platform — running through IPL 2026.

- Real-time ball-by-ball delivery via a 4-layer scheduling architecture
- Gemini AI integration for dynamic match narratives and pre-match predictions
- H2H records, venue analytics, weather-aware win probability
- **30 REST endpoints** · Firebase live score sync · Railway + Vercel

`React` `Spring Boot` `MySQL` `Firebase` `Gemini API` `Cricbuzz API`

---

## 🛠 Tech Stack

### Languages
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring JPA](https://img.shields.io/badge/Spring_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socketdotio&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FF6B35?style=for-the-badge)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22B5BF?style=for-the-badge)

### Databases & Cloud
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

### AI & Integrations
![Gemini](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Groq](https://img.shields.io/badge/Groq%20%2F%20Llama3-F55036?style=for-the-badge)
![RapidAPI](https://img.shields.io/badge/RapidAPI-0055DA?style=for-the-badge&logo=rapid&logoColor=white)

---

## 📦 Projects

| Project | Description | Stack | Status |
|--------|-------------|-------|--------|
| [CricSense](https://cricsense.in) | AI-powered IPL live scores + predictions. 30 endpoints, Gemini narratives, real-time Firebase sync. | React · Spring Boot · MySQL · Firebase · Gemini | 🟢 Live |
| VantageRoute | Monte Carlo freight route risk simulator across 143 seeded Indian routes with probabilistic scoring. | Spring Boot · Apache Commons Math · React | ✅ Done |
| PricePulse | Dynamic Pricing Engine — Strategy Pattern, embedded Redis, WebSocket/STOMP real-time updates. | Spring Boot · Redis · WebSocket · React | ✅ Done |
| SachCheck | AI fake news verifier for Indian WhatsApp misinformation. Bilingual verdicts via Llama 3. | Spring Boot · Groq · Llama 3 · React | ✅ Done |
| T20 World Cup Predictor | ICC qualification simulator with Firebase live bracket updates. | Spring Boot · React · Firebase | ✅ Done |
| CortexOS | Autonomous work intelligence system — Phase 1 frontend complete. | React · Vite · Tailwind · Groq | 🔧 WIP |
| PromptForge | Prompt structuring & evaluation tool with Firebase Auth. | Spring Boot · Gemini · Firebase · MySQL | 🔧 WIP |

---

## 🐛 Production Bugs I've Actually Fixed

**JPQL `LocalDateTime` range bug** — `findTodaysMatches` silently returned nothing because a datetime column was compared against a date-only value. Rewrote with explicit `LocalDateTime` range parameters.

**Firebase miniscore backtracking** — Rapid polling overwrote fresh score data with stale payloads. Introduced a `lastSavedTimestamp` guard in `LiveDataScheduler` — writes only if the incoming timestamp is newer.

**Silent Railway build failure** — Builds failed with no output. Traced to a stale `PredictionContext` bean in `GeminiServiceImpl.java` left from a refactor. Fixed the injection chain.

**Scheduler thread starvation** — Multiple `@Scheduled` tasks queued under load. Default thread pool too small. Configured a larger pool — tasks now run independently.

---

## 📊 GitHub Stats

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=codergirlprerna&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"/>
  &nbsp;
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=codergirlprerna&theme=tokyonight&hide_border=true&layout=compact&langs_count=6&hide=html,css,makefile,blade,dart,php"/>
</div>

---

> 💡 **Note:** The stats card may undercount commits — it only reads default branches of public repos. My actual contribution graph shows **757 contributions** in the last year.

---

<div align="center">
  <sub>Building in public · Shipping real products · Debugging real bugs</sub>
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=6366f1&height=80&section=footer" width="100%"/>
</div>
