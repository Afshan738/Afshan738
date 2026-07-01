# Afshan Qasim

I build distributed, production-grade systems - not just web apps.
Currently focused on cloud-native backend engineering: event-driven
architectures, container orchestration, and systems that survive
real-world failure conditions.

📍 Islamabad, Pakistan · BS-IT @ University of Chakwal (Jun 2026)
🏅 **NSCT'26 — Top 3.3% Nationally** · Ranked 96.7th percentile in the
National Skill Competency Test by HEC, PSEB & P@SHA


## Projects

### [Sentinel-SRE](https://github.com/Afshan738/Sentinel-SRE) · Distributed Uptime Monitor

Production-grade distributed system monitoring website health at scale.

- **Zero data loss under worker failure** — RabbitMQ Manual ACKs + Dead Letter Queues + Exponential Backoff
- **Sub-millisecond status lookups** — Redis caching layer cuts PostgreSQL read I/O dramatically  
- **Full observability** — Prometheus + Grafana dashboards tracking P99 latency per endpoint
- **Load verified** — k6 stress tested at concurrent user load to identify breaking points before production

`Go` `Node.js` `RabbitMQ` `Redis` `PostgreSQL` `Prometheus` `Grafana` `Docker` `k6`

### [Pulse_Queue](https://github.com/Afshan738/pulse-Queue) ·  production-grade idempotent job queue built with Node.js, Express, PostgreSQL, and Redis.

- **Exactly-once processing** — PostgreSQL advisory locks let workers claim jobs non-blockingly, so no two workers ever process the same job concurrently
- **Request-level idempotency** — SHA-256 request fingerprinting + 24-hour Redis TTL cache returns the original response to retried requests without re-executing side effects
- **Self-healing job recovery** — a stale `updated_at` on a job stuck in "processing" signals a crashed worker, and the scheduler resets it to pending automatically
- **Scalable pagination** — cursor-based `(created_at, id)` navigation backed by a matching composite index keeps query performance constant regardless of page depth

`Node.js` `Express` `PostgreSQL` `Redis` `Docker` `worker_threads` `pg_try_advisory_lock`

### [Link Vault](https://github.com/Afshan738/link-vault) · Kubernetes-Orchestrated Asset Manager

DevOps-first MERN application built for production-grade Kubernetes deployment.

- **Self-healing infrastructure** — Kubernetes automated pod recovery and restart policies
- **Config decoupling** — Kubernetes Secrets + ConfigMaps for clean credential isolation
- **Optimized images** — multi-stage Dockerfiles for lightweight production containers
- **Live monitoring** — Prometheus + cAdvisor + Grafana dashboards for real-time resource visibility

`React` `Node.js` `MongoDB` `Docker` `Kubernetes` `Prometheus` `Grafana` `cAdvisor`



## Stack

```
Languages     Go · JavaScript/TypeScript · Python
Backend       Node.js · Express.js · FastAPI
Frontend      React · Vite · TailwindCSS
Databases     PostgreSQL · MongoDB · Redis · MySQL
Messaging     RabbitMQ · BullMQ
Infra         Docker · Kubernetes · GitHub Actions
Observability Prometheus · Grafana · k6
```



## Community & Recognition
- **Open Source**
   SigNoz contributor — feat(components): add Skeleton (PR #230)
   +712 lines · 18 review comments · merged May 2026
   github.com/SigNoz/components/pull/230

- **NSCT'26** — Top 3.3% nationally (96.7th percentile) — National Skill
  Competency Test by HEC, PSEB & P@SHA
- **Dev Connect Hub** — Founded a 100+ member developer community,
  university-recognized, Islamabad

## Writing:
### LinkedIn
**858x Faster: What I Learned Optimising 500,000 PostgreSQL Rows**
https://www.linkedin.com/posts/afshan-qasim-998917300_postgresql-databaseperformance-queryoptimization-share-7463599947624611841-L436/?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAE0FscQB0wnD66Ar3MdwCW-l06nUW95fayw

**Your index is not a fix. It is a ticking clock.**
https://www.linkedin.com/posts/afshan-qasim-998917300_postgresql-backendengineering-sre-share-7464246699239239680-D-1G/?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAE0FscQB0wnD66Ar3MdwCW-l06nUW95fayw

### Dev Community|| Dev.to
**1,820x Faster: What I Learned Optimizing 500,000 PostgreSQL Rows**
 [Read the full article on dev.to](https://dev.to/afshanqasim/1820x-faster-what-i-learned-optimizing-500000-postgresql-rows-43in)

## Currently

- Contributing to open source - [SigNoz](https://github.com/SigNoz/signoz)
  observability platform (React · Go)
- Deepening Kubernetes operator patterns and Go concurrency internals



[afshanqasim349@gmail.com](mailto:afshanqasim349@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/afshan-qasim-998917300)
