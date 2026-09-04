---
title: Next.js Architecture & Ecosystem
type: technology-hub
category: frontend-framework
tags:
  - tech/nextjs
  - tech/react
  - frontend/fullstack
projects:
  - "[[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi Financial Tracker]]"
  - "[[Capy — Deep Project Architecture & System|Capy Mood & Travel Companion]]"
---

# Next.js Full-Stack Architecture

> [!INFO] **Technology Overview**
> **Next.js** serves as the unified React application framework powering the frontend, serverless API routes, and progressive web application (PWA) infrastructure across the engineering portfolio.

---

## Core Capabilities Utilized

### 1. App Router & Server Components (RSC)
- High-speed server-side rendering (SSR) and dynamic client routing.
- Segmented layouts with nested hydration boundaries for rapid initial page paints.
- Server Actions and route handlers (pp/api/*) for backend API operations without dedicated Node.js microservices.

### 2. Progressive Web App (PWA) Integration
- Offline caching and service worker lifecycle management.
- Web app manifest orchestration enabling native-like installation on Android and iOS.
- Seamless bridge to Android Trusted Web Activities (TWA).

### 3. API Route Architecture
- **Pawi**: /api/chat (streaming AI counselor with rate limits), /api/receipt-scan (OCR & image classification).
- **Capy**: /api/journal, /api/breathe, /api/chat (Gemini-driven empathetic companion).

---

## Projects Implementing Next.js
- [[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi: AI-Powered Personal Finance Tracker]] (Next.js 16 App Router)
- [[Capy — Deep Project Architecture & System|Capy: Cozy AI Mood & Travel Companion]] (Next.js 16 App Router + React 19)

---

## Related Hubs
- [[PostgreSQL]]
- [[Artificial Intelligence & LLMs]]
- [[Mobile Applications & TWA]]
- [[Tailwind CSS]]
- [[Home|Projects Dashboard]]
