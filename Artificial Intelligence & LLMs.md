---
title: Artificial Intelligence & Large Language Model Architecture
type: technology-hub
category: artificial-intelligence
tags:
  - tech/ai
  - tech/llm
  - tech/gemini
  - tech/groq
  - security/guardrails
projects:
  - "[[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi Financial Tracker]]"
  - "[[Capy — Deep Project Architecture & System|Capy Mood & Travel Companion]]"
---

# Artificial Intelligence & LLM Architecture

> [!INFO] **AI Core Philosophy**
> Both applications utilize context-aware, empathetic, and hardened conversational AI agents designed to provide domain-specific assistance while resisting prompt injection, jailbreaks, and cost abuse.

---

## AI Routing & Resilience Matrix

`mermaid
flowchart TD
    UserQuery([User Input]) --> Guardrail[Deterministic Pre-flight Filter]
    Guardrail -- Off-Topic / Jailbreak --> Deflection[Deterministic Mascot Refusal]
    Guardrail -- Valid Query --> RateLimit[Token Bucket Rate Limiter]
    RateLimit -- Limit Exceeded --> WaitMsg[429 Rate Limit Cooldown]
    RateLimit -- Pass --> PrimaryLLM{Tier 1: High-Speed LLM}
    
    PrimaryLLM -- Success --> StreamOut[Stream Response to User]
    PrimaryLLM -- Timeout / Failure --> SecondaryLLM{Tier 2: High-Capability LLM}
    SecondaryLLM -- Success --> StreamOut
    SecondaryLLM -- Failure --> LocalFallback[Tier 3: Local Deterministic Engine]
    LocalFallback --> StreamOut
`

---

## Comparative Implementations

| Feature Dimension | **Pawi Financial Tracker** | **Capy Companion** |
| :--- | :--- | :--- |
| **Agent Persona** | Pawi the Sea Turtle (Cautious, disciplined, compounding mentor) | Capy the Capybara (Calm, grounding, emotionally validating friend) |
| **Primary Engine** | Groq (LLaMA 3.3 70B / Qwen 2.5 32B) | Google Gemini 3.7 / 2.5 Flash |
| **Fallback Tier** | xAI Grok ➔ Google Gemini ➔ Local Regex NLP | Fallback Deterministic Reflection Engine |
| **Guardrails** | Strict financial scope; rejects cooking recipes, jailbreaks, roleplay | Mood validation, mental health de-escalation, mindful boundary enforcement |
| **Rate Limiting** | 20 requests / hour / user | Session-based throttling |

---

## Projects Implementing AI
- [[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi: AI-Powered Personal Finance Tracker]]
- [[Capy — Deep Project Architecture & System|Capy: Cozy AI Mood & Travel Companion]]

---

## Related Hubs
- [[Next.js]]
- [[PostgreSQL]]
- [[Home|Projects Dashboard]]
