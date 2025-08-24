
---
layout: default
title: Portfolio
---

# Cybersecurity & Java Portfolio

Welcome! This site showcases compact, working projects that demonstrate API design, incident response skills, and practical automation.

> **Certifications**: Security+ • CySA+ • AWS Cloud Practitioner
> **Focus**: SOC Analyst • IT Audit • Risk/Compliance • Blue Team

---

## 🔹 Project 1 — Chat API (Single-File Java)

A tiny Java HTTP API that demonstrates REST endpoints, request parsing, JSON responses, and in-memory data structures — **all in one file** (no frameworks).

**Endpoints**
- `GET /health`
- `POST /createUser` — body: `{ "userName": "..." }`
- `POST /createDeposit` — body: `{ "userId": "...", "amount": 50 }`
- `GET /getTransactions?userId=...`

**How to Run**
```bash
javac ChatPortfolioServer.java
java ChatPortfolioServer
# Server: http://localhost:8080
