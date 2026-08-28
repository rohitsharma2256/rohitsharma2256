# 👋 Hi, I'm Rohit Sharma

**Java backend engineer** who ships production Spring Boot systems — and works on the part of backend that's getting genuinely interesting right now: **giving LLM agents safe, deterministic control over real backend operations.**

Most of my time goes into **Java + Spring Boot**, and I go deep on **Model Context Protocol (MCP)** and **Spring AI** — architecting systems where an agent *selects* the action but the server *owns execution*, so business logic stays deterministic and auditable instead of hallucinated. It's a design problem more than a prompt problem, and that's what makes it fun.

🚀 **Live in production:** [ComplianceIQ](https://compliance-iq.co.in) — a multi-tenant AI SaaS on AWS automating Indian payroll compliance for CA firms.

---

## 🧠 How I think about engineering

I care less about *using* a framework and more about the decisions underneath it:

- **Correctness under concurrency** — transactional integrity and race-condition-safe writes, not just happy-path CRUD.
- **Determinism at the AI boundary** — the model never computes a monetary figure; it calls a tool, the server computes, the result is auditable.
- **Failure is a first-class case** — I've debugged a live production OOM down to heap behaviour and fixed it with JVM tuning + swap provisioning, not a restart-and-pray.
- **Multi-tenancy done at the service layer** — tenant isolation enforced in code, not hoped for in queries.

Currently going deeper on **system design, distributed systems, and production-grade AI-agent backends** (RAG evaluation, observability, and safe tool execution).

---

## 🛠️ Tech I work with

| | |
|---|---|
| **Core** | Java (8–21) · Spring Boot · Spring MVC · Spring Data JPA · Hibernate · Spring Security · REST API Design · JWT |
| **Data** | PostgreSQL · Relational Schema Design · Transactions & Concurrency Control · PGVector |
| **AI / Agentic** | Spring AI · Model Context Protocol (MCP) · RAG · LLM Tool Integration |
| **Infra & DevOps** | AWS (EC2, RDS) · Docker (multi-stage, Compose) · Kubernetes · Nginx · Linux · Git · GitHub Actions (CI/CD) |
| **Core CS** | DSA (Java) · OOP · Multithreading & Concurrency · Low-Level Design · DBMS · OS . CN|

---

## 📂 Projects worth your precious time

### 🧾 [ComplianceIQ — AI Payroll Compliance SaaS](https://github.com/rohitsharma2256/complianceiq-showcase) &nbsp; [`🔴 Live Demo`](https://compliance-iq.co.in)

A **live, multi-tenant SaaS** on AWS automating Indian statutory payroll compliance (EPF, ESI, TDS, PT) across **30+ REST APIs** — collapsing a chartered accountant's 2–3 hour Excel workflow into **under 2 minutes**.

**The engineering that matters here:**
- **Agentic AI layer (Spring AI + MCP)** — the LLM autonomously invokes 6 server-side tools to run compliance checks, surface violations with fixes, and generate audit reports. The model orchestrates; the server executes and owns every number — so output is deterministic and auditable.
- **RAG pipeline on PGVector** — 384-dim MiniLM embeddings with HNSW approximate-nearest-neighbour cosine search, serving citation-backed answers from statutory documents. An instant knowledge-update API pushes new rules live to all tenants with **zero redeployment**.
- **Security & isolation** — stateless JWT + BCrypt, per-IP token-bucket rate limiting (Bucket4j), and tenant-scoped isolation enforced across 7 PostgreSQL entities.
- **Production hardening** — multi-stage Docker builds (450 MB → 250 MB), Nginx-proxied React frontend, and a **live OOM crash diagnosed and resolved via JVM heap tuning + swap provisioning** for stable 24/7 uptime.

`Java 21` `Spring Boot` `Spring AI` `MCP` `RAG` `PGVector` `PostgreSQL` `React` `Docker` `AWS`

---

### 🛒 [NextGenCommerce — Agentic AI E-commerce Backend](https://github.com/rohitsharma2256)

An AI-integrated shopping backend on MCP that exposes cart operations (`addToCart`, `getCartTotal`, …) as **agentic tools**, so an LLM agent can drive real workflows against live services — with the server enforcing correctness, not the model. Tested end-to-end with Claude Desktop as the MCP client.

`Java` `Spring Boot` `MCP` `Spring AI` `PostgreSQL`

---

### 📅 [Global Class Booking System](https://github.com/rohitsharma2256/global-class-offering-booking-system)

Scalable booking backend across 15+ REST endpoints. The interesting part is **correctness under concurrency**: slot-level conflict detection with transactional integrity that prevents double-booking under simultaneous requests, plus a timezone-aware scheduling engine built on the Java Time API.

`Java 21` `Spring Boot` `PostgreSQL` `Docker`

---

### 🎫 [AI-Driven Ticketing System](https://github.com/rohitsharma2256/AI-Ticketing-System)

Self-Service helpdesk backend running the full ticket lifecycle — automatic priority detection, team routing, resolution — built with a **pluggable classification layer** so LLM-based categorization drops in without touching core services. Extensibility as a design decision, not an afterthought.

`Java 21` `Spring Boot` `Spring AI` `PostgreSQL`

---

## 📫 Reach me

🌐 [Portfolio](https://rohit-portfolio-nine-azure.vercel.app/) &nbsp;·&nbsp; 📧 [Email](mailto:rohitsharma250602@gmail.com) &nbsp;·&nbsp; 💼 [LinkedIn](https://www.linkedin.com/in/rohit-sharma-14aab6293/) &nbsp;·&nbsp; 🧩 [LeetCode](https://leetcode.com/u/rohitsharma250602/)

---

*Building toward production-grade AI-agent backends. Open to backend roles and hard problems.*
