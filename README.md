<h2 align="center">Alon Perlin</h2>

<p align="center">
Backend-leaning Full-Stack Developer · Tel Aviv
</p>

<p align="center">
I build <strong>production-oriented web systems</strong> with attention to real-world concerns:
asynchronous workloads, reliability, security, and long-term maintainability.
</p>

<p align="center">· · ·</p>

## Primary Project

### ChatSVG — AI-powered SVG generation platform (Beta · v0.2.0)

**ChatSVG** is my main ongoing project — a production-oriented SaaS for generating structured, sanitized SVG assets from text prompts.

This is not a demo project. It was intentionally designed to resemble how real backend systems behave in production:  
requests enqueue work, background workers process jobs asynchronously, failures are retried safely, and clients observe job state.

**Status:** Live, deployed, and actively evolving (Beta).

---

### What this project demonstrates

- Asynchronous job processing using background workers
- API correctness under retries and failures
- Safe idempotent request handling
- Credit-based usage limits and refunds
- Clear separation between API, worker, and infrastructure
- Production deployment with CI/CD and observability

I treat this project as a long-lived system, not a throwaway exercise.

---

### Tech highlights

**Backend**
- TypeScript, Node.js, Express
- PostgreSQL (Neon) + Prisma
- Redis + BullMQ (background jobs)

**Frontend**
- React, Vite, TypeScript

**Quality & Delivery**
- Jest (unit & integration tests)
- Playwright (end-to-end tests)
- Docker (local development & CI test environments)
- GitHub Actions (CI/CD)
- Deployed on Vercel & Render

---

### Links

- **Backend & Frontend repos:**  
  https://github.com/APerlinx/svg-saas-server  
  https://github.com/APerlinx/svg-saas-client

- **Live (Beta):**  
  https://chatsvg-three.vercel.app

<p align="center">· · ·</p>

## Additional Work

- **Herman Architects** — real production website for an architecture firm  
  https://hermanarchitects.com

- **The Wild Oasis** — full-stack Next.js demo application  
  https://the-wild-oasis-website-vert-five.vercel.app

<p align="center">· · ·</p>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=APerlinx&style=flat-square)

[![Tech](https://skillicons.dev/icons?i=ts,nodejs,express,postgres,prisma,react,nextjs,githubactions&perline=8)](https://skillicons.dev)

<a href="https://www.linkedin.com/in/alonperlin/">LinkedIn</a> ·
<a href="mailto:alonperinx@gmail.com">Email</a>

</div>
