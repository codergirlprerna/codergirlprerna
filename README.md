<h1 align="center">Prerna Khanna</h1>

<p align="center">
  Full-Stack Developer &nbsp;·&nbsp; MCA '26 &nbsp;·&nbsp; Spring Boot + React
</p>

<p align="center">
  <a href="https://linkedin.com/in/codergirlprerna">
    <img src="https://img.shields.io/badge/LinkedIn-codergirlprerna-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://cricsense.in">
    <img src="https://img.shields.io/badge/CricSense-Live-22c55e?style=flat&logo=spring&logoColor=white" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=codergirlprerna&style=flat&color=6366f1&label=views" />
</p>

---

I build complete products — API design, database schema, deployment pipelines, and everything in between. Currently running **[CricSense](https://cricsense.in)** in production through IPL 2026: a real-time cricket platform handling live ball-by-ball data, AI match narratives, and predictive analytics across 30 REST endpoints.

I care about the things that only matter when things go wrong in production: scheduler thread pools, stale cache writes, broken bean injection chains, and timestamp guards on polling loops. Those are in my commit history.

---

## Featured Project

### [CricSense](https://cricsense.in) &nbsp;—&nbsp; AI-Powered Cricket Platform `🟢 Live`

> Real-time IPL scores, H2H records, venue analytics, weather-aware match predictions, and Gemini-generated match narratives — running live through IPL 2026.

- 30 REST endpoints across match, prediction, and analytics domains
- 4-layer scheduling architecture for live data ingestion and score diffing
- Gemini AI integration for dynamic match commentary and pre-match narratives
- Deployed on Railway (backend) + Vercel (frontend) with Firebase for real-time score sync

**Stack:** `React` `Spring Boot` `MySQL` `Firebase` `Gemini API` `Cricbuzz API` `Railway` `Vercel`

---

## Other Projects

| Project | What it does | Stack |
|---|---|---|
| **VantageRoute** | Monte Carlo freight route risk simulator. 143 seeded Indian routes, probabilistic scoring, interactive risk visualizations. | Spring Boot · Apache Commons Math · React · Recharts |
| **PricePulse** | Dynamic pricing engine using the Strategy Pattern. Embedded Redis, Spring Events, WebSocket/STOMP real-time updates. | Spring Boot · Redis · WebSocket · React |
| **SachCheck** | AI fake news verifier for Indian WhatsApp misinformation. Bilingual Hindi/English verdicts via Llama 3 + Groq. | Spring Boot · Groq · Llama 3 · React |
| **T20 World Cup Predictor** | ICC qualification simulator with live Firebase bracket updates. | Spring Boot · React · Firebase |
| **CortexOS** | Autonomous work intelligence system — Phase 1 frontend complete. | React · Vite · Tailwind · Groq |
| **PromptForge** | Prompt structuring and evaluation tool with Firebase Auth. | Spring Boot · Gemini · Firebase · MySQL |

---

## Skills

**Languages** &nbsp; Java · JavaScript · Python · SQL · HTML · CSS

**Backend** &nbsp; Spring Boot · Spring Data JPA · REST APIs · Redis · WebSocket/STOMP · Spring Scheduler

**Frontend** &nbsp; React · Vite · Tailwind CSS · Recharts

**Databases & Cloud** &nbsp; MySQL · Firebase (Realtime DB + Firestore) · Railway · Vercel

**AI & Integrations** &nbsp; Gemini · Groq (Llama 3) · RapidAPI · Resend

---

## Production Incidents Worth Mentioning

Real bugs from real deployments — not course exercises.

**JPQL datetime range bug** — `findTodaysMatches` returned empty results silently because the query compared a `LocalDateTime` column against a date-only value. Rewrote the query with explicit `LocalDateTime` range bounds. Schedulers fired correctly after.

**Firebase miniscore backtracking** — Rapid polling was overwriting fresh score data with stale payloads. Added a `lastSavedTimestamp` guard in `LiveDataScheduler`: writes only proceed if the incoming delivery timestamp is newer than what's stored.

**Silent Railway build failure** — Backend builds failed without clear error output. A stale `PredictionContext` bean reference in `GeminiServiceImpl.java` — left over from a refactor — broke the injection chain. Traced through Railway logs, fixed the wiring.

**Scheduler thread starvation** — Multiple `@Scheduled` tasks queued behind each other under concurrent load due to an undersized default thread pool. Diagnosed from execution timing, configured a larger pool. Tasks now run independently.

---

## GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=codergirlprerna&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" />
&nbsp;&nbsp;
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=codergirlprerna&theme=tokyonight&hide_border=true&layout=compact&langs_count=6" />

</div>

---

<p align="center">
  <sub>Open to full-stack or backend roles · <a href="https://linkedin.com/in/codergirlprerna">Let's connect</a></sub>
</p>
