<h2 align="center">Alon Perlin</h2>

<p align="center">
Backend-leaning Full-Stack Developer · Tel Aviv  
</p>

<p align="center">
Focused on building <strong>production-grade web systems</strong> with real-world concerns:
asynchronous workloads, idempotency, fault tolerance, security, and CI/CD.
</p>

<p align="center">· · ·</p>

## 🚀 Primary Project

### ChatSVG — AI-Powered SVG Generation Platform (Beta · v0.2.0)

**ChatSVG** is a production-oriented SaaS for generating structured, sanitized SVG assets from text prompts.

This is my main ongoing project. It is **not a demo** — it is designed and built as a real system with background processing, retries, idempotency guarantees, and production deployment practices.

> Status: **Live, production-ready core**, actively evolving (Beta).

---

### Why this project matters

This project was intentionally built to demonstrate how I approach **real backend systems**, including:

- async job processing
- correctness under retries
- race-condition safety
- credit accounting & refunds
- API reliability under failure

---

### Core architecture highlights

**Asynchronous processing**
- SVG generation handled via **BullMQ workers**
- Dedicated worker service deployed separately from the API
- Supports retries, exponential backoff, and failure isolation

**Idempotency & correctness**
- Idempotent request handling using client-supplied keys
- Request hashing to prevent key reuse with different payloads
- Safe job claiming (`QUEUED → RUNNING`) to prevent double execution

**Credit accounting**
- Atomic credit charging after job claim
- Guaranteed refunds on permanent failure
- Refunds protected against double-execution via database guards

**Robust job lifecycle**
- Explicit job states (`QUEUED`, `RUNNING`, `SUCCEEDED`, `FAILED`)
- Retry-aware state transitions
- Final failure handling separated from transient errors

---

### Security & API discipline

- JWT authentication with rotating refresh tokens
- Refresh token reuse detection
- CSRF protection for authenticated requests
- Input sanitization and prompt validation
- Strict CORS and header allowlists
- Rate limiting and daily usage caps

---

### Observability & reliability

- Centralized structured logging (Pino)
- Error tracking with Sentry
- CI pipelines enforcing test and build health
- End-to-end tests spinning up frontend, backend, and database

---

### Deployment

- **Frontend**: Vercel  
- **Backend API**: Render  
- **Worker service**: Render (separate process)  
- **Database**: PostgreSQL (Neon)  
- **Queue & cache**: Redis

---

### Tech stack

**Backend**
- TypeScript
- Node.js, Express
- Prisma ORM
- PostgreSQL (Neon)
- BullMQ + Redis

**Frontend**
- React
- Vite
- TypeScript

**Quality & Delivery**
- Jest (unit / integration)
- Playwright (E2E)
- GitHub Actions (CI/CD)
- Vercel & Render

---

### Links

- **Repository**: https://github.com/APerlinx/svg-saas-client  
- **Live (Beta)**: https://chatsvg-three.vercel.app/

<p align="center">· · ·</p>

## 🏗️ Additional Production Work

- **Herman Architects** — real production website for an architecture firm  
  https://hermanarchitects.com

- **The Wild Oasis** — full-stack Next.js application (demo)  
  https://the-wild-oasis-website-vert-five.vercel.app

<p align="center">· · ·</p>

## 🎯 What I’m looking for

- Backend or full-stack roles
- Ownership over real systems, not just UI features
- Teams that value correctness, observability, and long-term maintainability

<p align="center">· · ·</p>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=APerlinx&style=flat-square)

[![Tech](https://skillicons.dev/icons?i=ts,nodejs,express,postgres,prisma,react,nextjs,githubactions&perline=8)](https://skillicons.dev)

<a href="https://www.linkedin.com/in/alonperlin/">LinkedIn</a> ·
<a href="mailto:alonperinx@gmail.com">Email</a>

</div>
