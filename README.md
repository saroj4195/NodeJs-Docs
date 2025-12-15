ased on my analysis of the HotelKite-X project, here's a comprehensive overview of the tech stack and packages used:

🏗️ Project Overview
HotelKite-X is an enterprise-grade Property Management System (PMS) for hotels built with a microservices-inspired modular architecture. It's a comprehensive hospitality management platform with 14 specialized modules and 190+ database models.

🛠️ Core Tech Stack
Runtime & Language
Node.js 18+ - JavaScript runtime environment
TypeScript 5.9.2 - Type-safe JavaScript with strict mode enabled
Express.js 5.1.0 - Web application framework
Database & ORM
PostgreSQL 15 - Primary database with multi-schema architecture (14 schemas)
Prisma 6.16.1 - Modern ORM with type-safe database access
Redis 7 - Caching and session storage
Architecture Patterns
Dependency Injection - TSyringe container for IoC
Multi-Schema Database - 14 PostgreSQL schemas for logical separation
Modular Design - Feature-based module organization
API-First Design - RESTful APIs with comprehensive documentation
📦 Key Production Dependencies
Core Framework & Utilities
express (5.1.0) - Web framework
cors (2.8.5) - Cross-origin resource sharing
helmet (8.1.0) - Security middleware
dotenv (17.2.2) - Environment configuration
reflect-metadata (0.2.2) - Metadata reflection for decorators
Database & Data Management
@prisma/client (6.16.1) - Database client
decimal.js (10.6.0) - High-precision decimal arithmetic
drizzle-orm (0.44.5) - Additional ORM capabilities
Authentication & Security
jsonwebtoken (9.0.2) - JWT token handling
google-auth-library (10.3.0) - Google OAuth integration
express-rate-limit (8.1.0) - Rate limiting
rate-limit-redis (4.2.2) - Redis-backed rate limiting
Async Processing & Queues
bullmq (5.58.5) - Redis-based job queues
@bull-board/api & @bull-board/express (6.12.7) - Queue monitoring UI
ioredis (5.7.0) - High-performance Redis client
bottleneck (2.19.5) - Rate limiting and job scheduling
HTTP & API
axios (1.12.2) - HTTP client
axios-retry (4.5.0) - Automatic retry logic
swagger-jsdoc (6.2.8) - API documentation generation
swagger-ui-express (5.0.1) - API documentation UI
File Processing & Storage
@aws-sdk/client-s3 (3.888.0) - AWS S3 integration
multer (2.0.2) - File upload handling
sharp (0.34.3) - Image processing
pdf-lib (1.17.1) - PDF manipulation
Observability & Monitoring
OpenTelemetry Suite - Comprehensive observability
@opentelemetry/api (1.9.0)
@opentelemetry/auto-instrumentations-node (0.64.1)
@opentelemetry/sdk-node (0.205.0)
Multiple OTLP exporters for traces, metrics, and logs
winston (3.17.0) - Structured logging
winston-daily-rotate-file (5.0.0) - Log rotation
morgan (1.10.1) - HTTP request logging
Date & Time
date-fns (4.1.0) - Modern date utility library
date-fns-tz (3.2.0) - Timezone support
dayjs (1.11.18) - Lightweight date library
Validation & Parsing
zod (4.1.8) - TypeScript-first schema validation
libphonenumber-js (1.12.17) - Phone number validation
xml2js (0.6.2) - XML parsing
xmlbuilder2 (3.1.1) - XML building
Utilities
lodash (4.17.21) - Utility functions
uuid (11.1.0) - UUID generation
glob (11.0.3) - File pattern matching
ua-parser-js (2.0.5) - User agent parsing
🧪 Development & Testing Stack
Testing Framework
jest (30.1.3) - Testing framework
ts-jest (29.4.2) - TypeScript preprocessor for Jest
jest-mock-extended (4.0.0) - Advanced mocking capabilities
@faker-js/faker (10.0.0) - Test data generation
Code Quality & Linting
eslint (9.35.0) - JavaScript/TypeScript linting
typescript-eslint (8.44.0) - TypeScript-specific ESLint rules
prettier (3.6.2) - Code formatting
eslint-config-prettier (10.1.8) - ESLint-Prettier integration
Build & Development Tools
typescript (5.9.2) - TypeScript compiler
ts-node (10.9.2) - TypeScript execution
nodemon (3.1.10) - Development server with hot-reload
tsc-alias (1.8.16) - Path alias resolution
tsconfig-paths (4.2.0) - TypeScript path mapping
Git Hooks & Workflow
husky (9.1.7) - Git hooks management
lint-staged (16.1.6) - Run linters on staged files
@commitlint/cli (19.8.1) - Commit message linting
cross-env (10.0.0) - Cross-platform environment variables
🏗️ Architecture Highlights
Modular Structure (14 Modules)
Core & Setup - Properties, rooms, rate plans
Authentication & Authorization - RBAC, JWT, sessions
Reservations - Booking lifecycle, payments
Front Office Management - Check-in/out, folios
CRM - Guest profiles, preferences
Housekeeping - Task management, room status
Channel Manager - OTA integrations
Revenue Management - Pricing, yield management
Subscription & Billing - Plans, invoicing
Reputation Management - Reviews, ratings
Procurement - Vendor management
Point of Sale - Restaurant/bar operations
Communication Hub - Multi-channel messaging
System Administration - Configurations, monitoring
Database Architecture
Multi-schema PostgreSQL with 14 schemas
190+ Prisma models with 91% metadata compliance
Consistent naming conventions and audit fields
Performance Features
Redis caching for frequently accessed data
BullMQ job queues for async processing
Connection pooling via Prisma
Rate limiting and circuit breakers
OpenTelemetry observability for monitoring
This is a sophisticated, enterprise-grade hospitality management system built with modern, production-ready technologies and architectural patterns designed for scalability, maintainability, and high performance.

Credits used: 1.43
