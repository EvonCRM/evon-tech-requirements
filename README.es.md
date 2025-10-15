# Requisitos Tecnológicos para Evon

> 🌐 **[English Version](./README.md)**

## Descripción General
Este documento describe las habilidades técnicas y conocimientos necesarios para trabajar efectivamente en Evon, un CRM enfocado en la conversión construido como monorepo.

---

## Tecnologías Core

### Runtime y Lenguaje
- **Node.js** (v20+) - Runtime de JavaScript del lado del servidor
- **TypeScript** (v5.7+) - Superset tipado de JavaScript
- **pnpm** (v9.12+) - Gestor de paquetes eficiente en espacio de disco

### Framework y Herramientas de Build
- **Next.js 15** - Framework de React con App Router y Server Components
- **React 19** - Biblioteca de UI con las últimas características
- **Turbo** (Turborepo) - Sistema de build de alto rendimiento para monorepos
- **Turbopack** - Bundler de nueva generación para desarrollo

---

## Desarrollo Frontend

### UI y Estilos
- **Tailwind CSS** - Framework CSS utility-first
- **Radix UI** - Primitivos de componentes sin estilos y accesibles
- **Shadcn/ui** - Componentes reutilizables construidos con Radix UI y Tailwind
- **Framer Motion** - Biblioteca de animaciones
- **Lucide React** - Biblioteca de iconos
- **PostCSS** y **Autoprefixer** - Herramientas de procesamiento CSS

### Gestión de Estado y Formularios
- **React Hook Form** - Gestión de formularios de alto rendimiento
- **Zod** - Validación de esquemas TypeScript-first
- **TanStack Table** - Biblioteca de tablas headless
- **@dnd-kit** - Toolkit de drag and drop
- **nuqs** - Gestión de estado URL con type-safety

### Características Avanzadas de UI
- **Lexical** - Framework de editor de texto extensible
- **Recharts** - Biblioteca de gráficos componible
- **React Image Crop** - Componente de recorte de imágenes
- **React Day Picker** - Componente de selector de fechas
- **Sonner** - Notificaciones toast

---

## Desarrollo Backend

### Base de Datos
- **PostgreSQL** - Base de datos relacional principal
- **Prisma** (v6.10+) - ORM de nueva generación con type safety
- **Prisma Client** - Cliente de base de datos auto-generado
- **Prisma Migrate** - Herramienta de migraciones de base de datos

### Autenticación y Autorización
- **NextAuth.js v5** (Auth.js beta) - Autenticación para Next.js
- **@auth/prisma-adapter** - Adaptador de Prisma para Auth.js
- **bcryptjs** - Hashing de contraseñas
- **otplib** - Generación de contraseñas de un solo uso
- **Proveedores OAuth**: Google, Microsoft Entra ID

### Desarrollo de APIs
- **Next.js API Routes** - Endpoints API serverless
- **next-safe-action** - Server actions con type-safety
- **Swagger/OpenAPI** - Documentación de API
- **next-swagger-doc** - Auto-generación de documentación de API

---

## Integraciones de Terceros

### Procesamiento de Pagos
- **Stripe** - Gateway de pagos y gestión de suscripciones
- **@stripe/stripe-js** - SDK de JavaScript para Stripe

### Servicios de Email
- **Nodemailer** - Envío de emails por SMTP
- **Resend** - API moderna de email
- **React Email** - Plantillas de email con React

### IA y ML
- **Vercel AI SDK** - Construcción de aplicaciones con IA
- **OpenAI SDK** (@ai-sdk/openai) - Integración con OpenAI

### Analytics y Monitoreo
- **Sentry** - Seguimiento de errores y monitoreo de rendimiento
- **Google Analytics** - Analítica web
- **PostHog** - Analítica de producto
- **Umami** - Analítica enfocada en privacidad

---

## DevOps e Infraestructura

### Containerización
- **Docker** - Plataforma de contenedores
- **Docker Compose** - Orquestación de múltiples contenedores
- **PostgreSQL 16 Alpine** - Contenedor de base de datos

### Despliegue
- **Railway** - Plataforma de despliegue en la nube
- **Next.js Production Build** - Builds de producción optimizados
- **Gestión de Variables de Entorno** - Configuración multi-entorno

### Control de Versiones
- **Git** - Control de versiones distribuido
- **GitHub Actions** - Workflows de CI/CD

---

## Herramientas y Prácticas de Desarrollo

### Calidad de Código
- **ESLint** - Linter de JavaScript/TypeScript
- **Prettier** - Formateador de código
- **TypeScript Compiler** - Verificación de tipos
- **Syncpack** - Gestión de versiones de dependencias en monorepo

### Testing
- **Cypress** - Framework de testing end-to-end

### Utilidades
- **date-fns** - Biblioteca moderna de utilidades de fechas
- **uuid** y **cuid2** - Generación de IDs únicos
- **clsx** y **tailwind-merge** - Utilidades para nombres de clases condicionales
- **ExcelJS** - Manipulación de archivos Excel
- **file-saver** - Guardado de archivos del lado del cliente

---

## Arquitectura de Monorepo

### Estructura de Workspace
Comprensión de:
- **Patrones de monorepo** con múltiples apps y paquetes compartidos
- **pnpm workspaces** para gestión de dependencias
- **Tareas y estrategias de caché** de Turborepo
- **Exports de paquetes** y referencias internas entre paquetes

### Paquetes Clave
- `@workspace/ui` - Componentes de UI compartidos
- `@workspace/database` - Capa de base de datos con Prisma
- `@workspace/auth` - Lógica de autenticación
- `@workspace/email` - Plantillas y envío de emails
- `@workspace/billing` - Lógica de pagos y suscripciones
- `@workspace/api-keys` - Gestión de API keys
- `@workspace/analytics` - Integración de analytics
- `@workspace/monitoring` - Seguimiento de errores
- `@workspace/i18n` - Internacionalización
- `@workspace/webhooks` - Manejo de webhooks
- `@workspace/rate-limit` - Limitación de tasa
- `@workspace/image-processing` - Manipulación de imágenes

---

## Conceptos y Habilidades Clave

### Conocimientos Requeridos
- **Arquitectura de monorepo** y gestión de workspaces
- **Server-side rendering** (SSR) y **Static Site Generation** (SSG)
- **React Server Components** y **Server Actions**
- **Desarrollo de API con type-safety** usando TypeScript
- **Diseño de esquemas de base de datos** y migraciones
- **OAuth 2.0** y flujos de autenticación
- **Webhooks de Stripe** y gestión de suscripciones
- **Entrega de emails** y renderizado de plantillas
- **Orquestación de contenedores** con Docker
- **Configuración basada en entornos**

### Mejores Prácticas
- Enfoque **type safety first** con TypeScript
- **Desarrollo basado en componentes** con componentes de UI reutilizables
- **Diseño API-first** con documentación apropiada
- **Mejores prácticas de seguridad** (hashing de contraseñas, headers seguros, rate limiting)
- **Optimización de rendimiento** (code splitting, lazy loading, caché)
- **Internacionalización** (i18n) con next-intl
- **Monitoreo de errores** y logging
- **Diseño responsive** y accesibilidad

---

## Habilidades Adicionales

### Deseable Tener
- Experiencia con patrones de **arquitectura SaaS**
- Implementación de **facturación por suscripción**
- Patrones de **multi-tenancy**
- **Características en tiempo real** con webhooks
- **Optimización SEO** para Next.js
- **Monitoreo y optimización de rendimiento**
- Plataformas de **despliegue en la nube** (Railway, Vercel)
- **Optimización de PostgreSQL** y tuning de queries

---

## Entorno de Desarrollo

### Herramientas Requeridas
- **VS Code** (o IDE similar con soporte para TypeScript)
- **Node.js 20+**
- **pnpm 9+**
- **Docker** y **Docker Compose**
- **PostgreSQL** (local o containerizado)
- **Git**

### Herramientas Opcionales
- **Prisma Studio** - Editor visual de base de datos
- **Mailhog** - Testing local de emails
- **Railway CLI** - Herramienta de despliegue

---

## Licencia

MIT

## Contribuir

Este es un documento vivo. Si notas alguna tecnología faltante o tienes sugerencias, por favor abre un issue o envía un pull request.
