# 🛠️ Tech Stack – GreaseMoto

> Full-stack motorcycle parts e-commerce platform • 100% TypeScript monorepo • ~2.0M+ LOC tracked

---

## 🎨 Frontend

![Next.js](https://img.shields.io/badge/Next.js_15.4-black?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

**Next.js 15 + React 19**
- Server-side rendering with full-stack cookie-based auth context passing
- App router with dynamic routes & nested layouts (`app/product/[id]/page.tsx`)
- Server actions for form handling with progressive enhancement

**tRPC + React Query**
- End-to-end type-safe APIs without code generation
- Custom middleware for automatic JWT refresh & error handling with SuperJSON serialization
- Client-side proxy wrapper for tuple-based error handling `[error, data]`

**Tailwind CSS + Radix UI**
- 18+ custom UI components (Dialog, Modal, Card, Table, Dropdown, etc.)
- Class Variance Authority for type-safe variant composition
- Fully accessible with ARIA labels & keyboard navigation

**Framer Motion**
- Animated dropdowns, page transitions, and interactive product carousels
- Physics-based spring animations for smooth UX

---

## ⚙️ Backend / Database

![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=for-the-badge&logo=trpc&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_S3+SES-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)

**Express.js + tRPC**
- Type-safe RPC layer with custom context (userId, sessionId, IP tracking)
- Automatic error logging to database for 500 errors
- WebSocket integration via Socket.io for real-time session management

**Prisma ORM**
- 30+ models with complex relations (Products, Orders, Fitments, etc.)
- Custom enums for order statuses, tracking states, shipping carriers
- Automatic migrations with seeding scripts for ~50K+ motorcycle parts

**PostgreSQL**
- Full-text search on product descriptions with GIN indexes
- JSONB fields for flexible fitment data & shipping exclusion zones
- Row-level tracking for order statuses, payments, returns

**Authentication**
- JWT access tokens (short-lived) + refresh tokens (2-year expiry)
- HttpOnly cookies with SameSite=Strict & domain-aware cookie setting
- Admin role verification via IP whitelist + 2FA with TOTP

**AWS S3 + SES**
- S3 for product image storage with presigned URLs
- SES for transactional emails (payment confirmations, shipping notifications)
- Multi-part uploads for large CSV/ZIP processing

**Stripe Payments**
- Payment intents with automatic webhook verification
- Stripe checkout sessions with custom success/cancel URLs
- Refund processing with automatic inventory restoration

**USPS Integration**
- OAuth token management with automatic refresh stored in DB
- Real-time address verification with standardization
- Zip+4 validation for accurate shipping calculations

**Cron Job System**
- Custom scheduler with AbortController support for cancellation
- Orphaned order cleanup (5-min timeout), image processing, SSL renewal
- Per-user job tracking with progress updates via Socket.io

---

## 📦 Infrastructure / DevOps

![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)

**Turborepo Monorepo**
- pnpm workspaces with shared tooling packages (`@acme/shared`, `@acme/testing`)
- Parallel task execution with intelligent caching
- Shared ESLint, Prettier, Tailwind, and TypeScript configs

**Docker Multi-Stage Builds**
- Production image with Prisma client generation
- Alpine Linux base (~80MB final image)
- Nginx + Certbot for SSL/TLS with Let's Encrypt

**Nginx Reverse Proxy**
- SSL termination with TLS 1.2/1.3
- WebSocket proxy upgrade support
- 50MB client_max_body_size for bulk uploads

**Vitest + Testing Library**
- Custom test factories for mocking Prisma, JWT, and fetch
- Happy-DOM for fast React component tests
- Pre-push hooks with `pnpm test:ai` for non-interactive CI

**Shared Validators**
- Zod schemas shared between frontend & backend
- Single source of truth for API contracts
- Address validation matching USPS state codes

---

## 📱 Mobile (WIP)

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)

**React Native**
- NativeWind (Tailwind for React Native)
- Expo-compatible architecture
- Shared tRPC hooks with web client

---

## 📊 Project Stats

- **135 TypeScript/TSX files** across client & server
- **~2.0M+ lines of code** tracked via git log --numstat (135 TypeScript/TSX files in current codebase)
- **100% TypeScript** – zero `.js` files in production code
- **30+ Prisma models** managing 50K+ motorcycle parts
- **18 custom UI components** with full accessibility
- **10+ tRPC routers** (auth, shop, admin, stripe, users, etc.)
- **Monorepo with 5 internal packages** + 3 apps (client, server, mobile)

---

## 🔗 Key Technical Achievements

✅ **Type-safe full-stack** – tRPC ensures zero API contract drift  
✅ **Complex domain modeling** – Vehicle fitments with hierarchical subcommodities  
✅ **Real-time updates** – Socket.io for live order tracking & admin notifications  
✅ **Production-ready auth** – JWT refresh flow with automatic token rotation  
✅ **Payment processing** – Stripe webhooks with idempotent order fulfillment  
✅ **Address validation** – USPS API integration with token caching  
✅ **Scheduled jobs** – Custom cron system with graceful cancellation  
✅ **Multi-tenant admin** – Row-level permissions with IP-based 2FA  
✅ **Deployment automation** – Docker + Nginx + SSL auto-renewal  
✅ **Comprehensive testing** – Vitest with mocked external dependencies  

---

*Built with modern web standards and a focus on developer experience, type safety, and scalability.*

