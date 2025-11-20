# 🚀 Factiii Tech Stack

## 🎨 Frontend

![Next.js](https://img.shields.io/badge/Next.js_15-black?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript_5.8-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

- **Next.js 15** – App Router with ISR, SSR + proxy middleware for auth routes, Vercel-optimized builds
- **Cesium.js** – 3D globe rendering with custom imagery providers, ion token integration, OSM buildings, terrain visualization with 1000+ LOC implementation
- **React Query** – Infinite scroll pagination, optimistic updates, auto-retry logic with `queryWrapper` helper
- **Framer Motion** – Advanced animations for modals, page transitions, confetti effects
- **Socket.io Client** – Real-time notifications, live presence tracking, WebRTC signaling for P2P sync

## 📱 Mobile

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo_53-000020?style=for-the-badge&logo=expo&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)

- **Expo 53** – EAS builds, OTA updates, custom native modules (biometric auth, location, push notifications)
- **React Native WebRTC** – P2P device sync via data channels, ICE candidate buffering, full signaling implementation
- **WatermelonDB** – Offline-first local DB with LokiJS adapter, incremental IndexedDB sync, custom migrations
- **Expo IAP** – In-app purchases for iOS/Android with receipt validation
- **React Native Reanimated 3** – 60fps animations with shared values and worklets

## ⚙️ Backend & Database

![Node.js](https://img.shields.io/badge/Node.js_23-339933?style=for-the-badge&logo=node.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma_6-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=for-the-badge&logo=trpc&logoColor=white)

- **tRPC** – End-to-end type-safe APIs with SuperJSON transformer, custom error middleware, auto-retry + token refresh logic, 24+ routers
- **Prisma** – 50+ models with composite indexes, slow query monitoring, connection pooling, 56 migrations
- **PostgreSQL** – Complex queries with CTEs, full-text search, geospatial data (lat/long), enum types
- **Express.js** – REST endpoints for webhooks, Helmet security, Morgan logging, CORS configuration
- **Socket.io Server** – Room-based messaging, WebRTC signaling rooms, real-time scrape status updates, activity tracking

## 💳 Payments & Storage

![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=for-the-badge&logo=stripe&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_S3-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)

- **Stripe** – Webhooks for subscriptions + one-time payments, invoice handling, refund processing, coupon generation
- **AWS S3** – Direct uploads with presigned URLs, CloudFront CDN integration, automatic MIME type detection
- **AWS SES** – Transactional emails with HTML templates

## 🤖 AI & Automation

![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![Puppeteer](https://img.shields.io/badge/Puppeteer-40B5A4?style=for-the-badge&logo=puppeteer&logoColor=white)

- **OpenAI GPT-4** – Function calling for structured outputs, token usage tracking, temperature/max_tokens control, 8+ personality bots
- **Puppeteer** – Headless scraping with Chromium in Docker, article extraction, YouTube transcript fetching
- **Google reCAPTCHA Enterprise** – Bot detection with score thresholds
- **Content Filtering** – Custom profanity filter with 1000+ word dictionary

## 🔧 Infrastructure & DevOps

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm_9-F69220?style=for-the-badge&logo=pnpm&logoColor=white)

- **Turborepo** – Monorepo with shared workspaces (`@shared/all`, `@shared/utils`), parallel task execution, remote caching
- **pnpm Workspaces** – Efficient dependency management with catalog protocol, patches for react-joyride + react-native-charts
- **Docker Compose** – Multi-stage builds, Chromium in Alpine, PostgreSQL dev/test containers with health checks
- **Jest + Supertest** – 66+ server tests, 7+ client tests, API integration testing, Prisma mocking
- **ESLint + Prettier** – Shared configs across packages, custom rules for monorepo

## 🔐 Auth & Security

![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)

- **JWT** – Access + refresh token rotation, httpOnly cookies, session device tracking
- **OAuth 2.0** – Google + Apple Sign-In with native SDKs
- **2FA/TOTP** – Time-based OTP with QR code generation using `totp-generator`
- **Biometric Auth** – Face ID/Touch ID for human verification with timeout enforcement
- **Helmet.js** – Security headers (CSP, HSTS, XSS protection)

## 📊 Additional Tech

- **Zod** – Schema validation in `@shared/all/validators.ts`, tRPC input validation
- **Lucide Icons** – 500+ icons shared across web + mobile
- **Nivo** – Scatterplot charts for data visualization
- **React Virtualization** – `@tanstack/react-virtual` for infinite lists
- **Sentry** – Error tracking with source maps
- **Google Maps API** – Geocoding + location services

---

## 📈 Project Stats

- **~2.5M+ lines of code** tracked via git log --numstat (865+ TypeScript/TSX files in current codebase)
- **100% TypeScript monorepo** with strict type checking
- **50+ Prisma models** with 1200+ LOC schema
- **24+ tRPC routers** with full type inference
- **Zero `any` types** (except error handling, reducers, RN styles per standards)
- **3 apps** (client, mobile, server) + **2 shared packages**
- **56 database migrations** with production-tested rollbacks

---

![TypeScript](https://img.shields.io/badge/100%25_TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Monorepo](https://img.shields.io/badge/Monorepo-000000?style=for-the-badge&logo=turborepo&logoColor=white)
![Lines of Code](https://img.shields.io/badge/2.5M%2B_LOC-black?style=for-the-badge)
