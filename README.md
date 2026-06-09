<div align="center">

# Prerna Khanna

### Full-Stack Developer · MCA '26 · Building things that ship

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/codergirlprerna/)
[![CricSense](https://img.shields.io/badge/CricSense-Live-brightgreen?style=flat-square)](https://cricsense.in)
![Profile Views](https://komarev.com/ghpvc/?username=codergirlprerna&style=flat-square&color=blue)

</div>

---

## About

I build full-stack products end-to-end — from schema design to deployment. Currently shipping **[CricSense](https://cricsense.in)**, an AI-powered IPL prediction and live score platform running live through IPL 2026.

I think about data pipelines, real-time architecture, and system design — not just features. When things break in production, I debug them.

---

## 🚀 Projects

| Project | Description | Stack | Status |
|--------|-------------|-------|--------|
| [CricSense](https://cricsense.in) | AI-powered IPL prediction & live score platform. Real-time ball-by-ball delivery, Gemini match narratives, H2H records, venue analytics, weather-aware predictions. 30 REST endpoints. | React · Spring Boot · MySQL · Firebase · Gemini · Cricbuzz API · Railway + Vercel | 🟢 Live |
| VantageRoute | Monte Carlo freight route risk simulator. 143 seeded Indian routes, probabilistic risk scoring, interactive visualizations. | Spring Boot · Apache Commons Math · React · Recharts | ✅ Complete |
| PricePulse | Dynamic Pricing Engine using Strategy Pattern. Embedded Redis, Spring Events, WebSocket/STOMP real-time updates. Built to demonstrate production-grade backend architecture. | Spring Boot · Redis · WebSocket · React | ✅ Complete |
| SachCheck | AI fake news verifier for Indian WhatsApp misinformation. Bilingual Hindi/English verdicts powered by Llama 3. | Spring Boot · Groq · Llama 3 · React | ✅ Complete |
| T20 World Cup Predictor | ICC qualification formula simulator with Firebase Realtime Database and live bracket updates. | Spring Boot · React · Firebase | ✅ Complete |
| CortexOS | Autonomous work intelligence system. Phase 1 frontend completed. | React · Vite · Tailwind · Groq | 🔧 WIP |
| PromptForge | Prompt structuring and evaluation tool with Firebase Auth. | Spring Boot · Gemini · Firebase · MySQL | 🔧 WIP |

---

## 🛠 Tech Stack

### Languages
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

### Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring JPA](https://img.shields.io/badge/Spring_JPA-6DB33F?style=flat-square&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FF6B35?style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat-square)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22B5BF?style=flat-square)

### Databases & Cloud
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)

### AI & APIs
![Gemini](https://img.shields.io/badge/Gemini_AI-4285F4?style=flat-square&logo=google&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)
![RapidAPI](https://img.shields.io/badge/RapidAPI-0055DA?style=flat-square&logo=rapid&logoColor=white)
![Resend](https://img.shields.io/badge/Resend-000000?style=flat-square)

---

## 🔧 In the Trenches

Real problems solved in production — not tutorials.

- **JPQL `LocalDateTime` range bug** — `findTodaysMatches` was silently returning no matches because of a date-only comparison on a datetime column. Rewrote the query to use explicit `LocalDateTime` range parameters. Schedulers started firing correctly.

- **Firebase miniscore backtracking** — Live score updates were writing stale data over fresh data during rapid polling. Fixed by introducing a `lastSavedTimestamp` guard in `LiveDataScheduler` — only writes if the incoming delivery timestamp is newer than what's stored.

- **Railway deployment failure from stale bean references** — Backend builds were failing silently due to a `PredictionContext` bean reference that no longer existed post-refactor. Traced through Railway build logs, found the broken wiring in `GeminiServiceImpl.java`, fixed the injection chain.

- **Scheduler thread starvation** — Multiple scheduled tasks were queuing behind each other under load because the thread pool was undersized. Diagnosed from timing logs, increased pool size, tasks now run independently on time.

---

## 📊 GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=codergirlprerna&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true)

![Streak](https://github-readme-streak-stats.herokuapp.com/?user=codergirlprerna&theme=tokyonight&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=codergirlprerna&theme=tokyonight&hide_border=true&layout=compact&langs_count=8)

</div>

---

<div align="center">

*Building in public · Shipping real products · Debugging real bugs*

</div>
