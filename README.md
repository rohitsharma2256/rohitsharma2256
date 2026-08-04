# 👋 Hi, I'm Rohit Sharma

**Java backend developer** building production Spring Boot systems — and increasingly, the part of backend that's getting interesting: connecting AI agents to real systems.

I work mostly with **Java + Spring Boot**, and I've been going hands-on with **Model Context Protocol (MCP)** and **Spring AI** — letting LLM agents safely execute real backend operations instead of just answering questions. It's an area most backend devs haven't touched yet, and I find it genuinely fun.

🚀 **Currently live:** [ComplianceIQ](https://compliance-iq.co.in) — a multi-tenant AI SaaS on AWS EC2, automating Indian payroll compliance for CA firms.

---

## 🛠️ What I work with

**Core** &nbsp;·&nbsp; Java (8–21) · Spring Boot · Spring MVC · Spring Data JPA · Hibernate · Spring Security · REST API Design · JWT

**Data** &nbsp;·&nbsp; PostgreSQL · Relational Schema Design · Transactions & Concurrency Control · PGVector

**AI / Agentic** &nbsp;·&nbsp; Spring AI · Model Context Protocol (MCP) · RAG · LLM Tool Integration

**Infra** &nbsp;·&nbsp; AWS (EC2, RDS) · Docker (multi-stage builds, Compose) · Nginx · Linux · Git · GitHub Actions (CI/CD)

**Core CS** &nbsp;·&nbsp; DSA (200+ solved in Java) · OOP · Multithreading & Concurrency · Low-Level Design · DBMS & OS

Currently going deeper on system design, distributed systems, and getting AI-agent backends production-ready (RAG, evals, observability).

---

## 📂 Projects I'd point you to first

### 🧾 [ComplianceIQ — AI Payroll Compliance SaaS](https://github.com/rohitsharma2256/complianceiq-showcase) &nbsp; [`🔴 Live Demo`](https://compliance-iq.co.in)
A **live, multi-tenant SaaS** on AWS EC2 automating Indian payroll compliance (EPF, ESI, TDS, PT) across **30+ REST APIs** — cutting a chartered accountant's 2–3 hour Excel workflow to under 2 minutes.

- **Agentic AI assistant** (Spring AI + MCP) where the LLM autonomously invokes 6 server-side tools to run compliance checks, surface violations with fixes, and generate audit reports
- **RAG pipeline** on PGVector (384-dim MiniLM, HNSW cosine search) serving citation-backed answers from statutory documents, with an instant knowledge-update API — new rules live for all tenants, zero redeployment
- Stateless JWT + BCrypt + per-IP rate limiting (Bucket4j) + tenant-scoped isolation across 7 PostgreSQL entities
- Multi-stage Docker builds (450 MB → 250 MB), Nginx-proxied React frontend, and a production OOM crash resolved via JVM heap tuning + swap provisioning for stable 24/7 uptime

`Java 21` `Spring Boot` `Spring AI` `MCP` `RAG` `PGVector` `PostgreSQL` `React` `Docker` `AWS`

---

### 🛒 [NextGenCommerce — Agentic AI E-commerce Backend](https://github.com/rohitsharma2256)
An AI-integrated shopping backend built on MCP, exposing cart operations as agentic tools (`addToCart`, `getCartTotal`, etc.) so LLM agents can drive real workflows against live services. Tested end-to-end with Claude Desktop as the MCP client.

`Java` `Spring Boot` `MCP` `Spring AI`

---

### 📅 [Global Class Booking System](https://github.com/rohitsharma2256/global-class-offering-booking-system)
Scalable booking backend across 15+ REST endpoints with slot-level conflict detection and transactional integrity to prevent double-booking under concurrent requests, plus a timezone-aware scheduling engine using the Java Time API.

`Java 21` `Spring Boot` `PostgreSQL` `Docker`

---

### 🎫 [AI-Driven Ticketing System](https://github.com/rohitsharma2256/AI-Ticketing-System)
Self-service helpdesk backend running the full ticket lifecycle — automatic priority detection, team routing, resolution built with a pluggable classification layer so LLM-based categorization drops in without touching core services.

`Java 21` `Spring Boot` `Spring AI` `PostgreSQL`

---

## 📫 Reach me

- 🌐 **Portfolio** — [rohit-portfolio-nine-azure.vercel.app](https://rohit-portfolio-nine-azure.vercel.app/)
- 📧 **Email** — [rohitsharma250602@gmail.com](mailto:rohitsharma250602@gmail.com)
- 💼 **LinkedIn** — [rohit-sharma-14aab6293](https://www.linkedin.com/in/rohit-sharma-14aab6293/)
- 🧩 **LeetCode** — [rohitsharma250602](https://leetcode.com/u/rohitsharma250602/)

---

*Currently building toward production-grade AI-agent backends. Open to backend roles and interesting problems.*
