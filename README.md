# Hi, I'm Gyan 👋

**Fullstack engineer** building field-service, geolocation, and real-time systems at production scale — and self-hosted products on the side.

I spent my first years deep in **React / React Native / TypeScript**, and now own systems end to end: FastAPI and Django backends, PostgreSQL/PostGIS and Redis data layers, Docker infrastructure, and the mobile and web frontends on top of them.

---

## 🔭 What I work on

**End-to-end geolocation pipelines** — I work across the full chain: GPS capture on device (`react-native-background-geolocation`), high-throughput ingestion into FastAPI backends via Redis Gears and Redis Streams, configurable sanitization and multi-detector anomaly pipelines, and on-read distance-recomputation architectures whose output drives real business processes like dispatch and per-km reimbursement — at a scale of **millions of location events a day**.

**GPS data trust & billing-grade correction** — Led a drift-elimination program end to end, from planning through implementation: quantified **~14 km of phantom distance per 8-hour stationary shift**, designed a stop/move state machine with hysteresis and moving-segment-only map matching (Valhalla), and built statistical audit tooling comparing distance methods across hundreds of engineer-days of data — down to per-person payout impact.

**Live tracking & geospatial UIs** — Real-time map dashboards in React (Leaflet/MapLibre) streaming live positions over WebSockets backed by Redis Streams, rendering at production territory scale; territory-management and work-area mapping tooling across thousands of geographic regions; utilization, capacity, and allocation views for large operations teams.

**Geospatial allocation platforms** — Founding engineer on a workforce-allocation platform: bootstrapped both the FastAPI backend and the React 19 frontend in the project's first week and drive both since. Pluggable geospatial allocation strategies, distance computation, load balancing, and route optimization on **PostgreSQL + PostGIS with graph storage (Apache AGE)**, plus the production Docker topology behind it (pgbouncer, a dedicated WebSocket container, multiple Celery worker pools and a beat scheduler) — allocating **thousands of jobs a day**.

**Field-service mobile at scale** — Founding mobile engineer of a React Native app used by **thousands of people** in the field every day. I own OTA release engineering end to end, including fail-closed channel-switching infrastructure with safety gates that guarantee an update can never interrupt someone mid-task.

**Real-time distributed delivery** — Built a service-request broadcast system end to end across backend and mobile: token-authenticated WebSockets with Redis pub/sub fan-out, a Celery-driven offer lifecycle (iteration, expiry, withdrawal, re-broadcast), a transactional notification outbox with an FCM fallback channel, race-safe accepts via Redis `SET NX` claims with Lua compare-and-swap release, and idempotent delivery acks where the first channel to confirm wins.

---

## 🚀 Projects

### [Skinsire](https://skinsire.in) — self-hosted learning platform
Designed, built, and launched a complete LMS for a dermatology-education creator in ~6 months of part-time work, and operate it in production solo.

- **FastAPI** backend with **194 endpoints**, **TanStack Start** frontend, HLS video streaming with per-segment token protection, PDF watermarking, and dual-gateway payments (Razorpay + PayPal) with idempotent webhook handling and scheduled reconciliation
- Engineered for minimal cost: **~280 users and ~500 videos** served from a single **2-core/8 GB VPS (~$10/month)** via resource-capped services, caching, and a tuned nginx layer
- Real production ownership: monitoring, capacity and connection-pool tuning, and performance debugging under concurrent playback load

### [sketchia](https://github.com/gyanbhartip/sketchia) — canvas & signature-capture library
A sketching library built on `@shopify/react-native-skia` — smooth cubic/quadratic stroke rendering, signature and highlighter modes, PNG/JPEG/WEBP export. Runs in production inside an app used by thousands of people daily.

Also: a 20-component React Native design system consumed in production since day one, distributed through a private npm registry (Verdaccio) I planned and deployed.

---

## 🛠️ How I build

- **Fail-closed by default** — safety gates, idempotency keys, discriminated unions that make illegal states unrepresentable, races fixed before release
- **Spec-first, high velocity** — I ship from idea to production through spec- and plan-driven design and **agentic AI development workflows** (Claude Code, custom skills and commands), owning every stage from design through release and production support, with correctness held by test gates
- **Production ownership** — I diagnose what I ship: performance and memory profiling on multi-hundred-gigabyte tables, transport and protocol debugging across WebSocket and HTTP layers, and preventive hardening caught before release

## 🧰 Stack

`TypeScript` `Python` `React` `React Native` `Expo/EAS` `TanStack` `FastAPI` `Django` `SQLAlchemy` `Celery` `PostgreSQL/PostGIS` `Redis (Streams/Gears)` `Docker` `nginx` `WebSockets` `FCM` `HLS/FFmpeg` `Valhalla` `Leaflet/MapLibre` `Playwright` `pytest` `Vitest`

Currently going deeper on: **PostgreSQL internals** and **async Python patterns**.

---

## 📫 Connect

 · [LinkedIn](https://linkedin.com/in/gyanbhartip) · 
