<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=3000&pause=1200&color=58A6FF&center=true&vCenter=true&width=580&lines=Vishwanath+Biradar;Backend+Engineer+%7C+SDE;Building+systems+that+scale)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vishwanath-biradar-582b502a9/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vishwanathsbiradar1@gmail.com)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/Vishwanath_Birdr)

</div>

---

Backend Engineer building systems that handle real load. I work primarily in **Java and Python**, focusing on API design, concurrent systems, and applied AI/ML integrations. I care about correctness, performance, and writing code that others can maintain.

Open to **Backend Developer**, **SDE**, and **AI/LLM Engineering** roles at product-based companies.

---

## What I work on

- **Backend systems** — REST APIs, WebSocket servers, async I/O, event-driven architecture
- **Concurrency & performance** — thread pools, LRU caching, rate limiting, load testing, JVM internals
- **Applied AI/ML** — generative pipelines, language model integrations, NLP, data processing
- **System design** — practicing CAP theorem, consistent hashing, partitioning, and replication patterns daily

---

## Stack

| Domain | Technologies |
|---|---|
| **Languages** | Java · Python · JavaScript |
| **Backend** | FastAPI · Spring Boot · Spring Security · Django · WebSockets · JWT · RabbitMQ |
| **Databases & Cache** | PostgreSQL · MySQL · MongoDB · Redis |
| **AI / ML** | PyTorch · TensorFlow · NumPy · Pandas |
| **Infra & Tooling** | Docker · Git · Alembic · Swagger · Postman |

---

## Projects

### [Multithreaded HTTP Proxy Server](https://github.com/vishwanath090/multithreaded-http-proxy-server) — `Java`

A from-scratch HTTP proxy server that acts as an intermediary between clients and upstream servers. The design goal was correctness under high concurrency, not just a working prototype.

**Engineering decisions:**
- Thread pool via `ExecutorService` — decoupled connection acceptance from request handling
- LRU cache with TTL using `LinkedHashMap` — eviction on both access order and staleness
- Sliding window rate limiter per client IP — prevents a single client from exhausting the pool
- `/metrics` endpoint exposing live cache stats, throughput, and rate-limit counters

**Results under load testing:**

| Metric | Result |
|---|---|
| Throughput | ~600 requests/sec |
| Average Latency | ~14 ms |
| Cache Efficiency | ~96.6% |

---

### [WalletPay — Digital Wallet + Real-time Messaging](https://github.com/vishwanath090/payment-wallet-chat-backend) — `Python · FastAPI · PostgreSQL` — **[Live](https://payment-wallet-chat-frontend.vercel.app)**

A production-deployed financial platform combining wallet transactions and real-time messaging. Backend is fully live on Render with a managed PostgreSQL instance on Neon and frontend on Vercel.

**Backend architecture:**
- Layered structure: `api/` → `services/` → `crud/` → `models/` — clean separation of concerns
- Async SQLAlchemy ORM with Alembic migrations for schema version control
- JWT access + refresh token flow with PIN-verified transaction endpoints
- WebSocket router with presence tracking, delivery/read receipts, and pending message delivery on reconnect
- Gunicorn + Uvicorn workers for async production serving

**API surface:** Authentication · Wallet (add, transfer, paginated history) · Realtime messaging · User presence  
**Deployed:** Vercel (frontend) · Render (backend) · Neon (PostgreSQL)

---

### [AI Story Generator](https://github.com/vishwanath090/Ai_Story_Generator-) — `Python · NLP`

Generative pipeline that produces coherent multi-paragraph narratives using language model APIs and structured prompt engineering. Explores context management and output conditioning — foundational work toward RAG and LLM-integrated backends.

---

### [Decentralised Identity Verification](https://github.com/vishwanath090/Decentralised-Identity-Verification) — `JavaScript`

An identity verification system exploring decentralised trust models. Applies cryptographic principles from Web3 to rethink how authentication can work without a central authority.

---

## Currently exploring

```
→  RAG pipelines — chunking strategies, embedding models, vector store integrations
→  LLM-integrated backends — serving model inference behind REST APIs, structured outputs
→  Distributed systems — Kafka, eventual consistency, distributed tracing
→  Java NIO — non-blocking I/O as a follow-up to the proxy server's blocking architecture
→  System design depth — practicing HLD/LLD for product-scale problems
```

---

## GitHub

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Vishwanath090&show_icons=true&theme=github_dark&hide_border=true&rank_icon=github&include_all_commits=true&count_private=true" height="165"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vishwanath090&layout=compact&theme=github_dark&hide_border=true&langs_count=6" height="165"/>

<br/>

<img src="https://streak-stats.demolab.com?user=Vishwanath090&theme=github-dark-blue&hide_border=true" height="150"/>

</div>

---

<div align="center">
<sub>
  <a href="https://www.linkedin.com/in/vishwanath-biradar-582b502a9/">LinkedIn</a> ·
  <a href="mailto:vishwanathsbiradar1@gmail.com">Email</a> ·
  <a href="https://x.com/Vishwanath_Birdr">X</a>
</sub>
</div>
