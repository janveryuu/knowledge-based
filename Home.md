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
> A central knowledge repository documenting full-stack, AI-native applications built by **Janver Yu**. Focused on **offline-first resilience**, **mascot-driven user interfaces**, **defensive AI guardrails**, and **native mobile packaging**.

---

## Active Applications

| Project | Mascot & Theme | Core Tech Stack | Status | Documentation & Quick Links |
| :--- | :--- | :--- | :---: | :--- |
| **Pawi Financial Tracker** | Pawi the Pawikan (*Slow & steady compounding*) | Next.js 16, Supabase, Groq/Gemini, Android TWA | 2.0.1 Active | [[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base\|Pawi Documentation]]<br>[GitHub Repo](https://github.com/janveryuu/pawi-financial-tracker) · [APK Release](https://github.com/janveryuu/pawi-financial-tracker) |
| **Capy Mood & Travel** | Capy the Capybara (*Calm, grounding wellness*) | Next.js 16, React 19, Prisma, PostgreSQL, Gemini | 1.0 Active | [[Capy — Deep Project Architecture & System\|Capy Documentation]]<br>[GitHub Repo](https://github.com/janveryuu/capy-app) · [Web App](https://capy-app-fawn.vercel.app/) |

---

## Shared Technology Ecosystem

`mermaid
graph TD
    Dashboard([Home Dashboard]) --> Pawi[Pawi Financial Tracker]
    Dashboard --> Capy[Capy Companion]
    
    Pawi --> NextJS[[Next.js]]
    Capy --> NextJS
    
    Pawi --> PG[[PostgreSQL]]
    Capy --> PG
    
    Pawi --> AI[[Artificial Intelligence & LLMs]]
    Capy --> AI
    
    Pawi --> Mobile[[Mobile Applications & TWA]]
    Capy --> Mobile
    
    Pawi --> Tailwind[[Tailwind CSS]]
    Capy --> Tailwind
`

### Knowledge Hubs
- [[Next.js]] — App Router, Server Components, Route Handlers & Serverless architecture
- [[PostgreSQL]] — Supabase RLS, Prisma ORM, transactional ledger consistency
- [[Artificial Intelligence & LLMs]] — Tiered Groq / Gemini fallbacks, deterministic prompt injection guardrails
- [[Mobile Applications & TWA]] — Trusted Web Activities, Gradle build scripts, camera and sensor bridges
- [[Tailwind CSS]] — Design systems, responsive layouts, color tokens, and SVG icon standards

---

## Interactive Visual Canvas
- [[Pawi Architecture.canvas|Open Pawi Visual Canvas Board]] — Infinite whiteboard with architecture blocks, database topologies, and QA checklists.

---

## Global Repository Synchronization
* **Knowledge Vault**: [janveryuu/knowledge-based](https://github.com/janveryuu/knowledge-based) (Auto-synced via Obsidian Git)
* **Pawi Repository**: [janveryuu/pawi-financial-tracker](https://github.com/janveryuu/pawi-financial-tracker)
* **Capy Repository**: [janveryuu/capy-app](https://github.com/janveryuu/capy-app)
