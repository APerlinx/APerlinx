<h2 align="center">Alon Perlin</h2>

<p align="center">
Backend-leaning Full-Stack Developer · Tel Aviv/Givatayim
</p>

<p align="center">
I build <strong>production-oriented web systems</strong> focused on backend correctness:
async workloads, security, reliability, and real deployments.
</p>

<p align="center">
Open to junior backend / full-stack roles (Node.js / TypeScript).
</p>

<p align="center">· · ·</p>

## Primary Project

### ChatSVG — AI-powered SVG generation platform (Live Beta · v0.3.0)

A production-oriented SaaS for generating structured, sanitized SVG assets from text prompts.

Not a demo: requests enqueue work, background workers process jobs asynchronously, failures are retried safely, and clients observe job state in real time.

**Live:** https://chatsvg.dev  
**API:** https://api.chatsvg.dev  
**Repos:** https://github.com/APerlinx/svg-saas-server · https://github.com/APerlinx/svg-saas-client

---

### Engineering highlights

- Async job processing: BullMQ workers + retries + failure handling
- Correctness under retries: idempotent requests + credit accounting safety (refunds on failure)
- Auth hardening: JWT in HttpOnly cookies, refresh rotation + reuse detection, CSRF protection
- Real-time updates: WebSockets (Socket.IO) + fallback flows
- Deploy + ops: GitHub Actions CI/CD → AWS ECR → Kubernetes (k3s on EC2), Sentry observability
- Secure artifact delivery: S3 storage + signed download URLs

---

<p align="center">· · ·</p>

## Additional Work

- **Herman Architects** — production website  
  https://hermanarchitects.com

- **The Wild Oasis** — Next.js full-stack demo  
  https://the-wild-oasis-website-vert-five.vercel.app

<p align="center">· · ·</p>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=APerlinx&style=flat-square)

[![Tech](https://skillicons.dev/icons?i=ts,nodejs,express,postgres,prisma,redis,react,nextjs,docker,kubernetes,aws,githubactions&perline=8)](https://skillicons.dev)

<a href="https://www.linkedin.com/in/alonperlin/">LinkedIn</a> ·
<a href="mailto:alonperinx@gmail.com">Email</a>

</div>
