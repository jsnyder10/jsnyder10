<div align="center">

# Jon Snyder

**Full-Stack Engineer • U.S. Air Force Veteran (2011–2023) • Self-Taught → Production-Ready in <5 years**

*Building production systems that scale while serving on Active Duty + raising a family*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jonathan_Snyder-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jonathan-snyder-b37b0598/)
[![Email](https://img.shields.io/badge/Email-jsnyder10%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jsnyder10@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-jsnyder10-181717?style=for-the-badge&logo=github)](https://github.com/jsnyder10)
[![DeepSource Profile](https://deepsource.com/u/jsnyder10/badge/dark.svg)](https://deepsource.com/u/jsnyder10) <!-- Live once first analysis completes -->

</div>

---

## ✅ Code Verification

All repositories are verified via **[DeepSource](https://deepsource.com/u/jsnyder10)** to confirm code ownership and contribution authenticity.


---

## 🚀 What I've Built

Solo architected and deployed **4 production full-stack applications** serving real users:

| Project | Description | Live Site | Tech Highlights |
|---------|-------------|-----------|-----------------|
| **Factiii** | AI-powered social platform with 3D globe visualization | [factiii.com](https://factiii.com) | Cesium.js, WebRTC P2P sync, React Native mobile, 50+ DB models |
| **GreaseMoto** | Motorcycle parts e-commerce (150K+ SKUs) | [greasemoto.com](https://greasemoto.com) | Stripe payments, USPS API, full-text search, inventory system |
| **Link3D** | NFC-based social networking platform | [link3d.io](https://link3d.io) | Native NFC read/write, real-time messaging, cross-platform mobile |
| **TapTrack** | Enterprise NFC time-tracking + payroll | [taptrack.io](https://taptrack.io) | Gusto OAuth integration, tour management, RBAC system |

---

## 📊 Quantified Impact

```
• 5,428,178+ lines of code shipped to production (tracked via git log --numstat)
• 150+ database models across 4 full-stack TypeScript monorepos
• 73+ type-safe tRPC API routers with zero code generation
• 100% TypeScript codebases (zero .js files in production)
• Built 3D WebGL globe engine from scratch with Cesium.js (1000+ LOC)
• Implemented local-first sync architecture with IndexedDB + Supabase RLS
• Solo maintained 4 production apps while Active Duty Air Force (2011–2023)
• Architected P2P WebRTC sync with data channels for offline-first mobile app
```

---

## 🛠️ Tech Stack

### Core Languages & Frameworks
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js_15-black?style=for-the-badge&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js_23-339933?style=for-the-badge&logo=node.js&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)

### Backend & Database
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=for-the-badge&logo=trpc&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)

### DevOps & Infrastructure
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

### Specialized Tech
![Cesium](https://img.shields.io/badge/Cesium.js-65CFFF?style=for-the-badge)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.io&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=for-the-badge&logo=stripe&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

---

## 📈 Contribution Breakdown

**Total lines contributed:** ~5.0M across 4 production repositories

| Repository | Your Contribution | Lines | Technical Scope |
|------------|-------------------|-------|-----------------|
| **greasemoto.com** | 90.14% | 1,842,624 | E-commerce platform with USPS + Stripe integration |
| **factiii.com** | 58.33% | 1,465,940 | Social platform with AI bots + 3D globe + mobile app |
| **link3d.io** | 83.27% | 436,166 | NFC social network with real-time messaging |
| **taptrack.io** | 66.88% | 232,037 | Enterprise time-tracking with Gusto payroll API |

<sub>*Measured via `git log --all --numstat` (additions + deletions per author)*</sub>

---

## 🎯 Technical Highlights

### **Architecture & Design**
- ✅ Built 4 end-to-end type-safe monorepos with shared validation layers (Zod schemas)
- ✅ Designed offline-first mobile architecture with IndexedDB (WatermelonDB) + Supabase sync
- ✅ Implemented JWT refresh token rotation with automatic retry middleware across all apps

### **Advanced Features**
- ✅ Custom 3D globe renderer with Cesium.js (imagery providers, terrain, OSM buildings)
- ✅ WebRTC peer-to-peer data channels for cross-device sync (ICE candidate buffering, signaling)
- ✅ Native NFC tag reading/writing in React Native (`react-native-nfc-manager`)
- ✅ Real-time systems with Socket.io (room-based messaging, live presence tracking)

### **Integrations & APIs**
- ✅ Stripe webhooks (subscriptions, refunds, invoice handling) with idempotent processing
- ✅ USPS OAuth token management + address verification + Zip+4 validation
- ✅ Gusto payroll API (OAuth 2.0 flow, employee sync, time entry creation)
- ✅ OpenAI GPT-4 function calling with token usage tracking (8+ personality bots)

### **DevOps & Testing**
- ✅ Docker multi-stage builds with Alpine Linux (Nginx + Certbot for SSL auto-renewal)
- ✅ Turborepo monorepos with pnpm workspaces (shared configs, parallel task execution)
- ✅ 73+ integration tests with Jest + Supertest (Prisma mocking, API contract testing)

---

## 💼 Background

**U.S. Air Force** (2011–2023)  
Served on Active Duty while self-teaching modern web development and shipping production code nights/weekends.

**Self-Taught Developer** (2018–Present)  
Learned TypeScript, React, Node.js, and full-stack architecture through building real products for real users.

**Full-Stack Generalist**  
Comfortable across the entire stack: database design, API architecture, UI/UX implementation, DevOps, and mobile development.

---

## 🔍 What I'm Looking For

**Open to Senior/Staff Engineer roles at missions that move humanity forward.**

Excited by companies building:
- 🚀 Aerospace & space technology (SpaceX, Relativity, etc.)
- 🛡️ Defense & autonomy (Anduril, Shield AI, etc.)
- ⚡ Energy & climate solutions (Tesla, Watershed, etc.)
- 🏗️ Developer tools & infrastructure (Vercel, Linear, etc.)

I thrive in environments that value:
- Shipping fast without sacrificing quality
- End-to-end ownership and accountability
- Deep technical challenges with real-world impact
- Small, high-trust teams building ambitious products

---

## 📬 Let's Connect

**LinkedIn:** [linkedin.com/in/jonathan-snyder-b37b0598](https://www.linkedin.com/in/jonathan-snyder-b37b0598/)  
**Email:** [jsnyder10@gmail.com](mailto:jsnyder10@gmail.com)

*Currently based in the U.S. • Open to remote or relocation for the right mission*

---

<div align="center">

*"Build things that matter, ship them fast, and never stop learning."*

</div>

