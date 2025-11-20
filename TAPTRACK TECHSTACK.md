# 🚀 TapTrack Tech Stack

> **Enterprise-grade NFC time-tracking & tour management platform** built with modern full-stack technologies

---

## 📊 Stack Overview

![TypeScript](https://img.shields.io/badge/TypeScript-100%25-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Monorepo](https://img.shields.io/badge/Monorepo-Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![Lines](https://img.shields.io/badge/Lines_of_Code-~347K+-success?style=for-the-badge)

---

## 🎨 Frontend & UI

### **Next.js 15** (App Router)
![Next.js](https://img.shields.io/badge/Next.js-15.3-000000?style=flat-square&logo=next.js&logoColor=white)
- ✅ Server Components with streaming SSR
- ✅ tRPC integration for type-safe API calls
- ✅ Advanced caching strategies with React Query

### **React 19** (Concurrent Features)
![React](https://img.shields.io/badge/React-19.1-61DAFB?style=flat-square&logo=react&logoColor=black)
- ✅ Server Actions for form submissions
- ✅ Suspense boundaries for loading states
- ✅ Custom hooks ecosystem (`useNFC`, `useFormValidation`, etc.)

### **Tailwind CSS 3.4**
![Tailwind](https://img.shields.io/badge/Tailwind-3.4-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
- ✅ Custom design system with CSS variables
- ✅ Dark mode support via `next-themes`
- ✅ Responsive mobile-first design patterns

### **shadcn/ui + Radix UI**
![shadcn](https://img.shields.io/badge/shadcn%2Fui-Latest-000000?style=flat-square)
- ✅ 60+ production-ready accessible components
- ✅ Custom form system with React Hook Form integration
- ✅ Class Variance Authority for component variants

### **Recharts**
![Recharts](https://img.shields.io/badge/Recharts-2.15-8884D8?style=flat-square)
- ✅ Interactive employee timeline visualizations
- ✅ Overtime tracking with custom bar charts
- ✅ Real-time data updates with tRPC subscriptions

---

## 🔧 Backend & API

### **tRPC 11**
![tRPC](https://img.shields.io/badge/tRPC-11.4-2596BE?style=flat-square&logo=trpc&logoColor=white)
- ✅ 14+ routers with role-based procedures (`protectedProcedure`, `adminProcedure`, `superAdminProcedure`)
- ✅ End-to-end type safety from database to UI
- ✅ React Query integration for optimistic updates & caching
- ✅ Custom middleware for authentication & authorization

### **Prisma 6**
![Prisma](https://img.shields.io/badge/Prisma-6.8-2D3748?style=flat-square&logo=prisma&logoColor=white)
- ✅ 20+ models with complex relations (tours, checkpoints, time entries, NFC tags)
- ✅ Soft deletes with `deletedAt` timestamp pattern
- ✅ Extensive indexing strategy for query optimization
- ✅ Type-safe queries (no `include`, all `select` for performance)

### **Supabase** (PostgreSQL + Auth)
![Supabase](https://img.shields.io/badge/Supabase-Postgres_17-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
- ✅ PostgreSQL 17 with Prisma ORM
- ✅ Supabase Auth for email/password + magic links
- ✅ Cookie-based SSR auth with `@supabase/ssr`
- ✅ JWT validation in tRPC context for both web & mobile

### **Zod** (Runtime Validation)
![Zod](https://img.shields.io/badge/Zod-3.25-3E67B1?style=flat-square)
- ✅ 80+ shared validation schemas in monorepo package (`@acme/all`)
- ✅ Type inference with `z.infer` for forms & API contracts
- ✅ Custom refinements (field validation, form-level validation)
- ✅ Zero duplication between frontend & backend validation

---

## 📱 Mobile (React Native)

### **Expo 54**
![Expo](https://img.shields.io/badge/Expo-54-000020?style=flat-square&logo=expo&logoColor=white)
- ✅ EAS Build for iOS & Android
- ✅ Expo Router for file-based navigation
- ✅ Expo Dev Client for custom native modules

### **React Native 0.81**
![React Native](https://img.shields.io/badge/React_Native-0.81-61DAFB?style=flat-square&logo=react&logoColor=black)
- ✅ Native NFC reading/writing (`react-native-nfc-manager`)
- ✅ Image/video capture with verification forms
- ✅ Offline-first architecture with AsyncStorage
- ✅ Reanimated 4 for smooth animations

### **NativeWind 4**
![NativeWind](https://img.shields.io/badge/NativeWind-4.1-38B2AC?style=flat-square)
- ✅ Tailwind CSS for React Native
- ✅ Shared design tokens with web app
- ✅ Dark mode support

---

## 🔐 Integrations & Services

### **AWS S3**
![AWS](https://img.shields.io/badge/AWS_S3-S3-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
- ✅ Direct uploads from web & mobile via presigned URLs
- ✅ Image/video storage for verification forms
- ✅ Profile picture uploads with `@aws-sdk/client-s3`

### **Gusto API** (Payroll Integration)
![Gusto](https://img.shields.io/badge/Gusto_API-OAuth_2.0-3B5998?style=flat-square)
- ✅ OAuth 2.0 flow with automatic token refresh
- ✅ Employee sync (bi-directional with Prisma)
- ✅ Time entry creation & clock in/out
- ✅ Company management & admin privileges

---

## 🏗️ Infrastructure & Tooling

### **Turborepo**
![Turborepo](https://img.shields.io/badge/Turborepo-2.5-EF4444?style=flat-square&logo=turborepo&logoColor=white)
- ✅ 3 apps (`nextjs`, `expo`, workspace packages)
- ✅ 5 tooling packages (ESLint, Prettier, TypeScript configs)
- ✅ Task caching for builds, lints, and type checks
- ✅ Parallel execution with dependency graph

### **pnpm 10**
![pnpm](https://img.shields.io/badge/pnpm-10.11-F69220?style=flat-square&logo=pnpm&logoColor=white)
- ✅ Workspace protocol for monorepo packages
- ✅ Catalog feature for unified dependency versions
- ✅ Automatic deduplication & hoisting

### **ESLint 9 + Prettier**
- ✅ Flat config format with custom rules
- ✅ Import sorting with `@ianvs/prettier-plugin-sort-imports`
- ✅ TypeScript-aware linting with `@typescript-eslint`

### **TypeScript 5.9** (Strict Mode)
![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178C6?style=flat-square&logo=typescript&logoColor=white)
- ✅ 100% TypeScript codebase (zero `.js` files)
- ✅ Strict null checks & no implicit any
- ✅ Shared `tsconfig` for consistency across packages
- ✅ Type-safe environment variables with `@t3-oss/env-nextjs`

---

## 📦 Architecture Highlights

### **Monorepo Structure**
```
tap-track/
├── apps/
│   ├── nextjs/         # Next.js 15 web app (tRPC server + client)
│   └── expo/           # React Native mobile app (tRPC client)
├── packages/
│   └── all/            # Shared Zod schemas, validators, types
└── tooling/
    ├── eslint/         # Shared ESLint configs
    ├── prettier/       # Shared Prettier config
    ├── tailwind/       # Shared Tailwind configs (web + native)
    └── typescript/     # Shared TypeScript configs
```

### **Key Features**
- 🏷️ **NFC Tag Management**: Read/write NDEF records, hex ID parsing, multi-technology support
- ⏱️ **Time Tracking**: Clock in/out via NFC, GPS location tracking, Gusto sync
- 🚶 **Tour System**: Checkpoints with dynamic verification forms (text, images, video)
- 📊 **Reporting**: Interactive employee timelines with Recharts
- 👥 **Multi-tenancy**: Organization-based access control with RLS patterns
- 🔐 **RBAC**: Super admin, admin, and employee roles with tRPC middleware

---

## 📈 Project Stats

| Metric | Value |
|--------|-------|
| **Total Lines of Code** | ~347,000+ (tracked via git log --numstat) |
| **TypeScript Coverage** | 100% |
| **tRPC Routers** | 14 |
| **Prisma Models** | 20 |
| **UI Components** | 60+ (shadcn/ui) |
| **Zod Schemas** | 80+ |
| **Apps in Monorepo** | 2 (Next.js + Expo) |
| **Shared Packages** | 5 |

---

## 🎯 Why This Stack?

✅ **Type Safety**: End-to-end TypeScript from database to UI (Prisma → tRPC → Zod → React)
✅ **Developer Experience**: Auto-completion, refactoring, instant error feedback
✅ **Performance**: Server Components, React Query caching, Prisma connection pooling
✅ **Scalability**: Monorepo with shared code, modular architecture, horizontal scaling ready
✅ **Modern**: Latest stable versions of all major dependencies (React 19, Next 15, Expo 54)

---

**Built with ❤️ using cutting-edge web & mobile technologies**
