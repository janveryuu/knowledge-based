---
title: PostgreSQL Database Architecture & Security
type: technology-hub
category: database
tags:
  - tech/database
  - tech/postgresql
  - tech/supabase
  - tech/prisma
  - backend/storage
projects:
  - "[[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi Financial Tracker]]"
  - "[[Capy — Deep Project Architecture & System|Capy Mood & Travel Companion]]"
---

# PostgreSQL Database Architecture

> [!INFO] **Database Overview**
> **PostgreSQL** provides the ACID-compliant relational data foundation for both application ecosystems, guaranteeing transactional integrity across financial ledgers and personal mental wellness records.

---

## Architectural Paradigms

`mermaid
graph TD
    User([Client Application]) --> Auth[Authentication Layer]
    Auth --> RLS[Row Level Security / ORM Guard]
    RLS --> PG[(PostgreSQL Database)]
    
    subgraph Pawi Implementation
        PG --> Wallets[(wallets & ledger)]
        PG --> Budgets[(budgets & categories)]
        PG --> Goals[(savings_goals & progress)]
        PG --> Trans[(transactions & receipts)]
    end
    
    subgraph Capy Implementation
        PG --> Users[(users & profiles)]
        PG --> Moods[(mood_logs & streaks)]
        PG --> Journal[(journal_entries & tags)]
        PG --> Breathing[(breathing_sessions)]
    end
`

### 1. Pawi: Managed Supabase PostgreSQL with Row Level Security (RLS)
- Declarative tenant isolation: every query enforces uth.uid() = user_id.
- Real-time subscription pipelines for instant multi-device balance reflections.
- Automated triggers: budget recalculations, savings streak tracking, and ledger balancing.

### 2. Capy: Prisma ORM over PostgreSQL
- Strictly typed database schemas and migration workflows (prisma/schema.prisma).
- Efficient relational queries for mood analytics, streak aggregations, and wellness histories.
- Connection pooling for responsive serverless invocation.

---

## Projects Implementing PostgreSQL
- [[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi: AI-Powered Personal Finance Tracker]] (Supabase PG 15 + RLS)
- [[Capy — Deep Project Architecture & System|Capy: Cozy AI Mood & Travel Companion]] (Prisma ORM + PostgreSQL)

---

## Related Hubs
- [[Next.js]]
- [[Artificial Intelligence & LLMs]]
- [[Home|Projects Dashboard]]
