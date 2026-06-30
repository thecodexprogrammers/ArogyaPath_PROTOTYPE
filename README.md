# ArogyaPath_PROTOTYPE
# ArogyaPath
### Healing India. Teaching India.

**Bharat's AI-powered Health + Education super platform — built for Tier 2/3/4 India.**

🔗 **Live Prototype:** [arogya-path-prototype.vercel.app](https://arogya-path-prototype.vercel.app)
🏆 Built for **Evolothon 1.0** — Round 2, Health & EdTech Track
👥 Team: **TheCodex**

---

## 🩺 The Problem

- **70%** of rural India lacks access to qualified medical advice
- **500M+** citizens remain health-illiterate
- English-only digital health platforms exclude the majority of India's **22+ language speakers**

## 💡 The Solution

ArogyaPath unifies five core modules into a single, vernacular-first, offline-capable platform:

| Module | Description |
|---|---|
| 🤖 **AI Symptom Checker** | Hindi-first conversational triage with escalation logic to teleconsultation |
| 📚 **Adaptive Health Courses** | Micro-learning for the general public and paramedical students |
| 📹 **Tele-Consultation** | Low-bandwidth doctor connect with appointment queueing |
| 📊 **Community Health Dashboard** | Anonymised, village/district-level health insight visualisation |
| 🔄 **Offline-First Sync** | Local-first storage with background sync for intermittent connectivity |

---

## ⚙️ About This Repository

This repo contains the **functional Round 2 prototype** — a single-page, browser-based interactive demo (`index.html`) built to validate the core user flows of ArogyaPath ahead of full-scale development.

**What's real in this prototype:**
- Live, working AI symptom-checker interaction (Hindi triage logic with urgency escalation)
- Functional teleconsultation booking flow
- Interactive course module previews
- Offline → sync simulation
- All logic runs client-side in your browser — no backend required to demo

**What's shown as planned (not yet built):**
The site also documents our **target production architecture** for post-MVP scaling — the full system design (Flutter mobile app, microservices backend, Claude API orchestration layer, Bhashini ASR/TTS, PostgreSQL/Firebase/Redis data layer, AWS infrastructure) we intend to build out as the project moves from prototype to MVP and beyond. This is **roadmap, not current state** — see the [Technical Architecture Report](./Arogyapath__1_.pdf) for full details.

> This is intentionally a lightweight, single-file prototype — built to demonstrate *product thinking and interaction design* within the hackathon timeline, not a production deployment.

---

## 🏗️ Target Production Architecture (Post-MVP)

```
Flutter Mobile App (offline-first) + React Web Dashboard
            ↓ REST / GraphQL
   API Gateway (NGINX / Kong — auth, rate-limit, routing)
            ↓
Identity & Auth · Symptom Checker (AI) · Tele-Consultation
Learning Engine · Community Dashboard
            ↓
AI Orchestration Layer (FastAPI wraps Claude API,
manages prompt templates, logs triage audit trail)
            ↓
PostgreSQL (core records) · Firebase (realtime)
Redis (cache/queue) · Cloudflare R2 (media)
```

**Planned tech stack:** Flutter (Dart) · React + Vite + Tailwind · Node.js (NestJS) / FastAPI · Claude API (Anthropic) · Bhashini + Whisper · WebRTC (Jitsi) · PostgreSQL (Supabase) · Firebase Realtime DB · Redis + BullMQ · AWS (ap-south-1) · Docker + ECS Fargate

**Compliance targets:** ABDM (Ayushman Bharat Digital Mission) · FHIR-compatible schema · DPDP Act 2023

---

## 🗺️ Roadmap

| Phase | Timeline | Target |
|---|---|---|
| MVP Launch | Q3 2027 | Hindi symptom checker, 3 courses, Android beta — 500 beta users |
| Expand | Q4 2027 | 5 languages, tele-consult live, 1 hospital partner |
| Scale | Q1 2028 | EdTech GA, recommendation engine v2 — 10,000 users |
| Bharat Reach | Q3 2028 | B2G pilot via ABDM sandbox, offline-first GA — 1M+ users |

---

## 🚀 Running Locally

This is a static, dependency-free single-page prototype.

```bash
git clone https://github.com/thecodexprogrammers/ArogyaPath_PROTOTYPE.git
cd ArogyaPath_PROTOTYPE
```

Open `index.html` directly in any browser — no build step or server required.

---

## 📄 License

Licensed under the **Apache-2.0 License** — see [LICENSE](./LICENSE) for details.

---

<p align="center"><i>Built for Bharat's Tier 2/3/4 population.</i></p>
