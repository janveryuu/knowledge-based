---
title: Engineering Knowledge Base & Projects Dashboard
type: dashboard-moc
updated: 2026-09-05
author: Janver Yu
status: Active
tags:
  - dashboard
  - moc
  - portfolio
  - architecture
---

# Engineering Knowledge Base & Projects Dashboard

> [!NOTE] **Mission & Architecture Philosophy**
> A central knowledge repository documenting full-stack, AI-native companion applications built by **Janver Yu**. Focused on **offline-first resilience**, **mascot-driven user interfaces**, **defensive AI guardrails**, and **native mobile packaging**.

---

## Active Applications (The Mascot Companion Ecosystem)

| Project | Mascot & Theme | Core Tech Stack | Status | Documentation & Quick Links |
| :--- | :--- | :--- | :---: | :--- |
| **Pawi Financial Tracker** | Pawi the Pawikan (*Slow & steady compounding*) | Next.js 16, Supabase, Groq/Gemini, Android TWA | `v2.0.1 Active` | [[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi Documentation]]<br>[GitHub Repo](https://github.com/janveryuu/pawi-financial-tracker) · [APK Release](https://github.com/janveryuu/pawi-financial-tracker) |
| **Capy Mood & Travel** | Capy the Capybara (*Calm, grounding wellness*) | Next.js 16, React 19, Prisma, PostgreSQL, Gemini | `v1.0.0 Active` | [[Capy — Deep Project Architecture & System|Capy Documentation]]<br>[GitHub Repo](https://github.com/janveryuu/capy-app) · [Web App](https://capy-app-fawn.vercel.app/) |
| **Dormosaur Campus Companion** | Dormosaur the Dino (*Smart campus living, extinct stress*) | Next.js 16, Supabase, Gemini 3.6 Flash, Groq, Web Push | `v0.1.0 Active` | [[Dormosaur — AI-Powered Student Campus & Dorm Companion — Complete Project Architecture & Knowledge Base|Dormosaur Documentation]]<br>[GitHub Repo](https://github.com/janveryuu/dormosaur) · [Web App](https://dormosaur.vercel.app/) |

---

## Shared Technology Ecosystem

```mermaid
graph TD
    Dashboard([Home Dashboard]) --> Pawi[Pawi Financial Tracker]
    Dashboard --> Capy[Capy Mood & Travel]
    Dashboard --> Dorm[Dormosaur Campus Companion]
    
    Pawi --> NextJS[[Next.js]]
    Capy --> NextJS
    Dorm --> NextJS
    
    Pawi --> PG[[PostgreSQL]]
    Capy --> PG
    Dorm --> PG
    
    Pawi --> AI[[Artificial Intelligence & LLMs]]
    Capy --> AI
    Dorm --> AI
    
    Pawi --> Mobile[[Mobile Applications & TWA]]
    Capy --> Mobile
    Dorm --> Mobile
    
    Pawi --> Tailwind[[Tailwind CSS]]
    Capy --> Tailwind
    Dorm --> Tailwind
```

### Knowledge Hubs
- [[Next.js]] — App Router, Server Components, Route Handlers & Serverless architecture
- [[PostgreSQL]] — Supabase RLS, Prisma ORM, transactional ledger consistency
- [[Artificial Intelligence & LLMs]] — Tiered Groq / Gemini fallbacks, multimodal OCR, deterministic prompt injection guardrails
- [[Mobile Applications & TWA]] — Trusted Web Activities, Gradle build scripts, camera and sensor bridges, Web Push
- [[Tailwind CSS]] — Design systems, responsive layouts, color tokens, and SVG icon standards

---

## Interactive Visual Canvas
- [[Pawi Architecture.canvas|Open Pawi Visual Canvas Board]] — Infinite whiteboard with architecture blocks, database topologies, and QA checklists.

---

## Global Repository Synchronization
* **Knowledge Vault**: [janveryuu/knowledge-based](https://github.com/janveryuu/knowledge-based) (Auto-synced via Obsidian Git)
* **Pawi Repository**: [janveryuu/pawi-financial-tracker](https://github.com/janveryuu/pawi-financial-tracker)
* **Capy Repository**: [janveryuu/capy-app](https://github.com/janveryuu/capy-app)
* **Dormosaur Repository**: [janveryuu/dormosaur](https://github.com/janveryuu/dormosaur)
