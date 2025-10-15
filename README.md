# Technology Requirements for Evon

> 🌐 **[Versión en Español](./README.es.md)**

## Overview
This document outlines the technical skills and knowledge required to work effectively on Evon, a conversion-focused CRM built as a monorepo.

---

## Core Technologies

### Runtime & Language
- **Node.js** (v20+) - Server-side JavaScript runtime
- **TypeScript** (v5.7+) - Typed superset of JavaScript
- **pnpm** (v9.12+) - Fast, disk space efficient package manager

### Framework & Build Tools
- **Next.js 15** - React framework with App Router and Server Components
- **React 19** - UI library with latest features
- **Turbo** (Turborepo) - High-performance build system for monorepos
- **Turbopack** - Next-generation bundler for development

---

## Frontend Development

### UI & Styling
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Unstyled, accessible component primitives
- **Shadcn/ui** - Re-usable components built with Radix UI and Tailwind
- **Framer Motion** - Animation library
- **Lucide React** - Icon library
- **PostCSS** & **Autoprefixer** - CSS processing tools

### State Management & Forms
- **React Hook Form** - Performant form management
- **Zod** - TypeScript-first schema validation
- **TanStack Table** - Headless table library
- **@dnd-kit** - Drag and drop toolkit
- **nuqs** - Type-safe URL state management

### Advanced UI Features
- **Lexical** - Extensible text editor framework
- **Recharts** - Composable charting library
- **React Image Crop** - Image cropping component
- **React Day Picker** - Date picker component
- **Sonner** - Toast notifications

---

## Backend Development

### Database
- **PostgreSQL** - Primary relational database
- **Prisma** (v6.10+) - Next-generation ORM with type safety
- **Prisma Client** - Auto-generated database client
- **Prisma Migrate** - Database migration tool

### Authentication & Authorization
- **NextAuth.js v5** (Auth.js beta) - Authentication for Next.js
- **@auth/prisma-adapter** - Prisma adapter for Auth.js
- **bcryptjs** - Password hashing
- **otplib** - One-time password generation
- **OAuth Providers**: Google, Microsoft Entra ID

### API Development
- **Next.js API Routes** - Serverless API endpoints
- **next-safe-action** - Type-safe server actions
- **Swagger/OpenAPI** - API documentation
- **next-swagger-doc** - Auto-generate API docs

---

## Third-Party Integrations

### Payment Processing
- **Stripe** - Payment gateway and subscription management
- **@stripe/stripe-js** - Stripe JavaScript SDK

### Email Services
- **Nodemailer** - SMTP email sending
- **Resend** - Modern email API
- **React Email** - Email templates with React

### AI & ML
- **Vercel AI SDK** - Building AI-powered applications
- **OpenAI SDK** (@ai-sdk/openai) - OpenAI integration

### Analytics & Monitoring
- **Sentry** - Error tracking and performance monitoring
- **Google Analytics** - Web analytics
- **PostHog** - Product analytics
- **Umami** - Privacy-focused analytics

---

## DevOps & Infrastructure

### Containerization
- **Docker** - Container platform
- **Docker Compose** - Multi-container orchestration
- **PostgreSQL 16 Alpine** - Database container

### Deployment
- **Railway** - Cloud deployment platform
- **Next.js Production Build** - Optimized production builds
- **Environment Variables Management** - Multi-environment configuration

### Version Control
- **Git** - Distributed version control
- **GitHub Actions** - CI/CD workflows

---

## Development Tools & Practices

### Code Quality
- **ESLint** - JavaScript/TypeScript linter
- **Prettier** - Code formatter
- **TypeScript Compiler** - Type checking
- **Syncpack** - Dependency version management in monorepo

### Testing
- **Cypress** - End-to-end testing framework

### Utilities
- **date-fns** - Modern date utility library
- **uuid** & **cuid2** - Unique ID generation
- **clsx** & **tailwind-merge** - Conditional class name utilities
- **ExcelJS** - Excel file manipulation
- **file-saver** - Client-side file saving

---

## Monorepo Architecture

### Workspace Structure
Understanding of:
- **Monorepo patterns** with multiple apps and shared packages
- **pnpm workspaces** for dependency management
- **Turborepo tasks** and caching strategies
- **Package exports** and internal package references

### Key Packages
- `@workspace/ui` - Shared UI components
- `@workspace/database` - Database layer with Prisma
- `@workspace/auth` - Authentication logic
- `@workspace/email` - Email templates and sending
- `@workspace/billing` - Payment and subscription logic
- `@workspace/api-keys` - API key management
- `@workspace/analytics` - Analytics integration
- `@workspace/monitoring` - Error tracking
- `@workspace/i18n` - Internationalization
- `@workspace/webhooks` - Webhook handling
- `@workspace/rate-limit` - Rate limiting
- `@workspace/image-processing` - Image manipulation

---

## Key Concepts & Skills

### Required Knowledge
- **Monorepo architecture** and workspace management
- **Server-side rendering** (SSR) and **Static Site Generation** (SSG)
- **React Server Components** and **Server Actions**
- **Type-safe API development** with TypeScript
- **Database schema design** and migrations
- **OAuth 2.0** and authentication flows
- **Stripe webhooks** and subscription management
- **Email delivery** and template rendering
- **Container orchestration** with Docker
- **Environment-based configuration**

### Best Practices
- **Type safety first** approach with TypeScript
- **Component-driven development** with reusable UI components
- **API-first design** with proper documentation
- **Security best practices** (password hashing, secure headers, rate limiting)
- **Performance optimization** (code splitting, lazy loading, caching)
- **Internationalization** (i18n) with next-intl
- **Error monitoring** and logging
- **Responsive design** and accessibility

---

## Additional Skills

### Nice to Have
- Experience with **SaaS architecture** patterns
- **Subscription billing** implementation
- **Multi-tenancy** patterns
- **Real-time features** with webhooks
- **SEO optimization** for Next.js
- **Performance monitoring** and optimization
- **Cloud deployment** platforms (Railway, Vercel)
- **PostgreSQL optimization** and query tuning

---

## Development Environment

### Required Tools
- **VS Code** (or similar IDE with TypeScript support)
- **Node.js 20+**
- **pnpm 9+**
- **Docker** & **Docker Compose**
- **PostgreSQL** (local or containerized)
- **Git**

### Optional Tools
- **Prisma Studio** - Visual database editor
- **Mailhog** - Local email testing
- **Railway CLI** - Deployment tool

---

## License

MIT

## Contributing

This is a living document. If you notice any missing technologies or have suggestions, please open an issue or submit a pull request.
