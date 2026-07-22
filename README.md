# Hi, I'm Gyan 👋

**Fullstack engineer** building field-service, geolocation, and real-time systems at production scale — and self-hosted products on the side.

I spent my first years deep in **React / React Native / TypeScript**, and now own systems end to end: FastAPI and Django backends, PostgreSQL/PostGIS and Redis data layers, Docker infrastructure, and the mobile and web frontends on top of them.

---

## 🔭 What I work on

**End-to-end geolocation pipelines** — I build the full chain: GPS capture on device (`react-native-background-geolocation`), high-throughput ingestion into FastAPI backends via Redis Gears and Redis Streams, configurable sanitization and multi-detector anomaly pipelines, and distance-computation architectures whose output drives real business processes like dispatch and reimbursement — at a scale of **millions of location events a day**.

**Live tracking & geospatial UIs** — Real-time map dashboards in React (Leaflet/MapLibre) streaming positions over WebSockets backed by Redis Streams; territory-management tooling spanning thousands of geographic regions; utilization and allocation views for large operations teams.

**Geospatial allocation platforms** — Founding backend work on workforce-allocation systems: pluggable geospatial allocation strategies, distance computation, load balancing, and route optimization on PostgreSQL + PostGIS, serving large operations teams allocating thousands of jobs a day.

**Field-service mobile at scale** — Founding mobile engineer of a React Native app used by **thousands of people** in the field every day. I own OTA release engineering end to end, including fail-closed channel-switching infrastructure with safety gates that guarantee an update can never interrupt someone mid-task.

**Real-time distributed delivery** — Broadcast systems built across backend and mobile: dual racing channels (WebSocket + FCM), atomic Redis claims with compare-and-swap rollback, idempotent fallbacks, and offline queues that drain safely.

---

## 🚀 Projects

### [Skinsire](https://skinsire.in) — self-hosted learning platform
Designed, built, and launched a complete LMS for a dermatology-education creator in ~6 months of part-time work, and operate it in production solo.

- **FastAPI** backend, **TanStack Start** frontend, HLS video streaming with per-segment token protection, PDF watermarking, dual-gateway payments (Razorpay + PayPal) with idempotent webhook handling and scheduled reconciliation
- Engineered for minimal cost: **~280 users and ~500 videos** served from a single **2-core/8 GB VPS (~$10/month)**
- Real production ownership: monitoring, performance debugging, and incident resolution under concurrent playback load

### [sketchia](https://github.com/gyanbhartip/sketchia) — canvas & signature-capture library
A sketching library built on `@shopify/react-native-skia` — smooth cubic/quadratic stroke rendering, signature and highlighter modes, PNG/JPEG/WEBP export. Runs in production inside an app used by thousands of people daily.

Also: a 20-component React Native design system consumed in production since day one, distributed through a private npm registry (Verdaccio) I planned and deployed.

---

## 🛠️ How I build

- **Fail-closed by default** — safety gates, idempotency keys, discriminated unions that make illegal states unrepresentable
- **Spec-first, high velocity** — I ship from idea to production through spec- and plan-driven design and **agentic AI development workflows** (Claude Code, custom skills and commands), owning every stage from design through release and production support, with correctness held by test gates
- **Production ownership** — I diagnose what I ship: event-loop blocking under 100+ GB datasets, WebSocket memory leaks, HTTP proxy framing bugs, mobile race conditions

## 🧰 Stack

`TypeScript` `Python` `React` `React Native` `Expo/EAS` `TanStack` `FastAPI` `Django` `SQLAlchemy` `PostgreSQL/PostGIS` `Redis (Streams/Gears)` `Docker` `nginx` `WebSockets` `FCM` `HLS/FFmpeg` `Valhalla` `Leaflet/MapLibre` `Playwright` `pytest` `Vitest`

Currently going deeper on: **PostgreSQL internals** and **async Python patterns**.

---

## 📫 Connect

 · [LinkedIn](https://linkedin.com/in/gyanbhartip) ·