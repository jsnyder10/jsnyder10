LINK#D TECHSTACK.md
## 🚀 Tech Stack

### 🎨 Frontend & UI
![Next.js](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)
![React](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.x-38B2AC?style=for-the-badge&logo=tailwind-css)

- **Next.js 15** – Server-side rendering, dynamic routing (`/tag/[tagId]`, `/event/[eventId]`), API routes with tRPC integration
- **React 18** – Context providers (Auth, Theme, User, Preferences), custom hooks (`useAuth`, `useTheme`, `useLink`), performance optimization with memo/useCallback
- **Tailwind CSS** – Custom design system with CSS variables for theme-aware components, dark mode support, responsive layouts
- **React Query** – Advanced caching strategies, automatic refetch on focus, optimistic updates for 27+ query hooks
- **Socket.io Client** – Real-time messaging, live notifications, session management with auto-reconnect

### 📱 Mobile & Native
![React Native](https://img.shields.io/badge/React_Native-0.76-20232A?style=for-the-badge&logo=react)
![Expo](https://img.shields.io/badge/Expo-SDK_52-000020?style=for-the-badge&logo=expo)

- **React Native 0.76** – Custom theme system (`useTheme` hook), StyleSheet-based architecture, cross-platform components
- **NFC Manager** – Write/read NFC tags, NDEF message formatting, UUID generation for tag identification
- **Expo Push Notifications** – Server-side push notification orchestration via `expo-server-sdk`, device token management
- **AsyncStorage** – Secure token persistence, offline-first architecture

### ⚡ Backend & API
![Node.js](https://img.shields.io/badge/Node.js-20.9-339933?style=for-the-badge&logo=node.js)
![tRPC](https://img.shields.io/badge/tRPC-11-2596BE?style=for-the-badge&logo=trpc)
![Express](https://img.shields.io/badge/Express-4.18-000000?style=for-the-badge&logo=express)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-336791?style=for-the-badge&logo=postgresql)
![Prisma](https://img.shields.io/badge/Prisma-5.x-2D3748?style=for-the-badge&logo=prisma)

- **tRPC 11** – End-to-end type safety with 126+ procedures across 15 routers, custom middleware for auth, tuple-based error handling `[error, data]`
- **Prisma ORM** – 30+ models with complex relations, custom migrations, seeding scripts, full-text search with indexes
- **PostgreSQL** – Row-level constraints, UUIDs for distributed IDs, complex joins for social graph queries, materialized views
- **Express** – Middleware pipeline with Helmet (security headers), Morgan (request logging), CORS with dynamic origin validation
- **Socket.io** – Real-time bidirectional communication, room-based messaging, session-socketId association for live updates

### 🔗 Integrations & Services
![Stripe](https://img.shields.io/badge/Stripe-API-008CDD?style=for-the-badge&logo=stripe)
![AWS](https://img.shields.io/badge/AWS-S3_+_SES-FF9900?style=for-the-badge&logo=amazon-aws)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-412991?style=for-the-badge&logo=openai)

- **Stripe** – Webhook signature verification, subscription lifecycle management (`checkout.session.completed`), payment intent tracking, customer portal
- **AWS S3** – Multipart uploads for images/videos, signed URL generation, CloudFront integration
- **AWS SES** – Transactional emails, event tracking, bounce/complaint handling
- **OpenAI API** – Token usage tracking per user, cost accounting in µUSD, rate limiting (per-user and premium tiers)
- **Twilio** – SMS OTP for 2FA, phone verification flows

### 🏗️ DevOps & Infrastructure
![Docker](https://img.shields.io/badge/Docker-Multi--stage-2496ED?style=for-the-badge&logo=docker)
![Turborepo](https://img.shields.io/badge/Turborepo-2.3-EF4444?style=for-the-badge&logo=turborepo)
![pnpm](https://img.shields.io/badge/pnpm-9.14-F69220?style=for-the-badge&logo=pnpm)

- **Docker** – Multi-stage builds for optimized production images (Alpine-based), health checks, volume management for Prisma migrations
- **Turborepo** – Monorepo task orchestration, incremental builds with cache, parallel execution for `dev`/`build`/`test`
- **pnpm Workspaces** – Shared internal packages (`@shared/utils`, `@shared/all`), workspace protocol dependencies, centralized tooling configs
- **Jest** – Unit + integration tests, custom setup for Puppeteer E2E, `ts-jest` for TypeScript, coverage reporting

### 🔒 Security & Validation
![Zod](https://img.shields.io/badge/Zod-3.x-3E67B1?style=for-the-badge&logo=zod)
![JWT](https://img.shields.io/badge/JWT-Auth-000000?style=for-the-badge&logo=json-web-tokens)

- **Zod** – Runtime schema validation on all tRPC endpoints, type inference for request/response payloads
- **JWT** – Access/refresh token rotation, automatic refresh logic, httpOnly cookies (web), secure AsyncStorage (mobile)
- **Helmet** – Security headers (CSP, HSTS, X-Frame-Options), XSS protection
- **bcryptjs** – Password hashing with configurable rounds, constant-time comparison

---

### 📊 Project Stats
- **~523,000+ LOC** tracked via git log --numstat (300+ TypeScript files in current codebase)
- **100% TypeScript monorepo** – Zero JavaScript files in application code
- **15 tRPC routers** with type-safe client generation
- **30+ Prisma models** with complex relational schema
- **3 applications** (Web, Mobile, Server) sharing logic via workspaces
- **Zero `any` types** – Strict TypeScript configuration enforced

> Built with modern TypeScript, fully type-safe from database to UI, with real-time features and cross-platform capabilities.