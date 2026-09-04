---
title: Mobile Applications & Trusted Web Activity (TWA)
type: technology-hub
category: mobile-engineering
tags:
  - mobile/android
  - mobile/twa
  - mobile/pwa
  - build/gradle
projects:
  - "[[Pawi — AI-Powered Personal Finance Tracker — Complete Project Architecture & Knowledge Base|Pawi Financial Tracker]]"
  - "[[Capy — Deep Project Architecture & System|Capy Mood & Travel Companion]]"
---

# Mobile Applications & TWA Engineering

> [!INFO] **Mobile Architecture Overview**
> Rather than maintaining separate React Native or Flutter codebases that drift out of sync with web features, both platforms leverage **Trusted Web Activity (TWA)** and Progressive Web App (PWA) standards to package Next.js production builds directly into native Android APKs.

---

## Native Bridge & TWA Pipeline

`mermaid
graph LR
    NextJS[Next.js PWA Build] --> Bubblewrap[Android TWA Wrapper]
    Bubblewrap --> Gradle[Gradle 8.4 Build Engine]
    Gradle --> Keystore[Android Release Keystore]
    Keystore --> APK[Signed Android Release APK]
    APK --> Device[Android Mobile Device]
    
    Device -. Hardware Access .-> Hardware[Camera / Biometrics / Notifications]
    Hardware -. Web API .-> NextJS
`

---

## Key Hardware Capabilities Bridged
1. **Live Camera Video Streams**: BarcodeDetector and getUserMedia for real-time QR code decoding and receipt capture.
2. **Push Notifications**: Web Push API synchronized with Android notification channels.
3. **Offline Caching**: IndexedDB local storage combined with Service Workers for offline-first resilience.
4. **Digital Asset Links**: Cryptographic SHA-256 fingerprint verification ensuring seamless fullscreen execution without browser URL bars.

---

## Active Mobile Binaries
- **Pawi**: Pawi-V2.apk (Signed Release Build, Gradle 8.4, TWA Android 14 compatible)
- **Capy**: Web-to-mobile PWA (capy-app-wtj1.vercel.app/login)

---

## Related Hubs
- [[Next.js]]
- [[Home|Projects Dashboard]]
