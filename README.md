# 🌿 GasPi-Check Showcase V9.5

### *Collective intelligence against food waste.*

![Version](https://img.shields.io/badge/version-9.5-4CAF50?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Android%20%7C%20iOS-blue?style=flat-square)
![Stack](https://img.shields.io/badge/stack-React%20Native%20%2F%20Firebase-orange?style=flat-square)
![Architecture](https://img.shields.io/badge/architecture-Local%20First%20Cloud%20Sync-purple?style=flat-square)
![License](https://img.shields.io/badge/license-Proprietary-red?style=flat-square)
![Commits](https://img.shields.io/badge/commits-95-lightgrey?style=flat-square)

> Every gram of food saved is a gram of CO₂ that never existed.
> GasPi-Check turns your fridge into a behavioral data engine — and makes sustainability a multiplayer game.

---

## 📱 Interface — V9.5

| Login | Product Scanner | My Fridge |
| :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/a79fcb8a-c4e3-42f8-8f78-b8ecf5a8cb50" width="220"/> | <img src="https://github.com/user-attachments/assets/eb6b6485-be70-4a44-a56c-548092bf4e2b" width="220"/> | <img src="https://github.com/user-attachments/assets/c4241179-694a-4db6-ab60-9ed519d907b9" width="220"/> |

&nbsp;

| Personal Statistics | Shared Family Fridge | Live Community Stats |
| :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/4e9402a0-4751-4c9d-bd40-274ce84f5ba3" width="220"/> | <img src="https://github.com/user-attachments/assets/77d47d61-9c89-4591-a45e-32d252bbd0d7" width="220"/> | <img src="https://github.com/user-attachments/assets/e8b96b15-3faa-4c69-a65a-16a20712f3cf" width="220"/> |

---

## 🚀 What it does

GasPi-Check is a **React Native app** that tracks household food consumption in real time, scores eco-responsible behavior, and aggregates anonymous waste data at scale.

Not a reminder app. Not a shopping list.
A **behavioral change engine** — with hardcore gamification, family sync, and a data pipeline that no market research firm can replicate.

---

## ⚙️ Tech Stack

| Layer | Technology |
|---|---|
| Mobile | React Native · Expo · TypeScript |
| Auth | Firebase Auth · Google Sign-In (V9.5) |
| Database | Firestore (real-time onSnapshot) |
| Local Cache | AsyncStorage — Local First architecture |
| Barcode | Open Food Facts API · EAN global index |
| CO₂ Engine | Hybrid model — Agribalyse + per-category fallback |
| Analytics | Custom pipeline → Firestore → BigQuery (ready) |
| Privacy | Rotating anonymous IDs · GDPR Kill-Switch |

---

## 💎 Core Features — V9.5

### 1. 🎮 Hardcore Gamification Engine *(Zen-Eco)*
The reward system is built around a real effort economy — no XP for buying, only for acting responsibly.

- **+50 XP** per GREEN consumption · **+20 XP** per ORANGE consumption
- **−200 XP** voluntary waste penalty (with confirmation modal)
- **−100 XP** automatic expiry penalty — applied once, on first detection
- **10 prestige grades**: *"Stock Novice"* → *"Eternal Legion"* → *"Immortal"*
- **Power Cards** system for engagement spikes (Turbo XP, Reset, Streak Shield)
- **Streak multiplier**: ≥7 days clean → ×1.5 XP on all actions
- Weekly recap notification every Monday — personalized CO₂ impact message

### 2. 👨‍👩‍👧 Family Fridge Sync
Waste reduction is a team sport.

- Real-time inventory sharing across **up to 6 family members** via Firestore `onSnapshot`
- Shared family XP counter — every action visible to the group
- "Added by [name]" attribution on every food card
- Anti-bruteforce invite code system (5 attempts → 10 min lockout)
- Correct logout flow: `unsubscribeFamilyRef` called synchronously **before** `signOut` — zero `permission-denied` errors

### 3. 🔐 Privacy-First Architecture *("Silicon Valley" Standard)*
Trust is non-negotiable.

- **GDPR Kill-Switch**: full data wipe — cloud + local — in one tap
- **Zero nominal tracking**: rotating anonymous IDs regenerated every 4 weeks
- Data minimization by design: no GPS, no email in analytics, no product photo in Firestore
- Consent-gated analytics: behavioral data only sent when user explicitly opts in
- Household size field: optional, never mandatory

### 4. 📊 Barcode Analytics V2 — The Data Moat
Every scan is an event. Every event is intelligence.

- EAN-level product indexing: brand, nutriscore, ecoscore, NOVA score, organic label, format
- Behavioral enrichment: meal slot (breakfast/lunch/snack/dinner), days-to-waste, household size
- Auto-computed aggregates per product: `wasteRate`, `avgDaysFromAddToConsume`, `byMealSlot`, `byDayOfWeek`
- Fully GDPR-compliant: EAN data is not personal data — no additional consent required
- Pipeline ready for BigQuery export (1-click Firebase extension)

### 5. 🏗️ Local First, Cloud Sync Architecture
Inspired by Notion, Linear, and Figma.

- **Every write hits AsyncStorage first** — zero perceived latency
- **Firestore write is fire-and-forget** in the background
- Cold start on empty device → pulls from Firestore → fills AsyncStorage → renders
- Offline mode: full app functionality, auto-sync on reconnect
- Last-write-wins conflict resolution with `serverTimestamp()`

---

## 📈 Data Moat — The Business Angle

GasPi-Check captures something no company can buy elsewhere:
**real behavioral data on food waste — at the exact moment it happens, inside real fridges.**

Nielsen and Kantar run panels of 2,000 people max, with declarative data.
GasPi-Check is behavioral, real-scale, EAN-level, timestamped.

| Metric | Projection (5K active users) |
|---|---|
| Events / month | ~780,000 |
| One-shot brand report | €20K – €300K |
| Annual monitoring deal | up to €500K |
| Target clients | Danone · Nestlé · Carrefour · ADEME · WWF |

---

## 🗺️ Roadmap

| Version | Status | Highlights |
|---|---|---|
| V1.0 → V2.9 | ✅ Done | Core gamification, barcode scanner, statistics engine |
| V3.5 → V4.5 | ✅ Done | Streak system, trophies, Power Cards, CO₂ hybrid engine |
| V5.0 → V6.5 | ✅ Done | Push notifications sentinel, splash screen, Android adaptive icons |
| V7.0 | ✅ Done | Firebase Auth, profile screen, CO₂ badges, GDPR consent |
| V8.0 | ✅ Done | Local First Cloud Sync — multi-device, persistent sessions |
| V8.5 | ✅ Done | Barcode Analytics V2 pipeline · Family Fridge (6 members) |
| **V9.5** | ✅ **Done** | **Google Sign-In · GDPR Kill-Switch · Community Impact screen** |
| V10.0 | 🔜 Planned | Landing page · App Store submission · RSE data export |

---

## 👤 Author

**Darkden64** — Solo builder · 95 commits · 0 burnout.

*Built with React Native, Firebase, and an unreasonable amount of conviction.*
