# Sprelli — Online Tutoring Platform

**Sprelli** is a modern educational marketplace connecting students with verified tutors in Poland. The platform enables booking individual and group lessons, real-time learning through interactive tools, progress tracking, and content monetization — all in one place, without any external tools.

---

## What is Sprelli?

Sprelli is a complete educational platform where:

- **Students** (and parents) can find a verified tutor, book a lesson, and pay securely online
- **Tutors** build their brand, manage their schedule, sell educational materials, and teach without needing Zoom, Google Meet, or any third-party tool
- **Schools and institutions** can use the platform to complement their educational offering (B2B)

Our mission: democratize access to high-quality tutoring in Poland.

---

## For Students

- **Search and filter** tutors by subject, level, price and availability
- **Book lessons** — individual or group — with verified tutors
- **Learn online** in a dedicated Lesson Room with video, whiteboard, chat and quizzes
- **Track progress** — XP points, levels, streaks, achievements and learning goals
- **Solve quizzes and play educational mini-games** assigned by your tutor or from the public library
- **Buy educational materials** from tutors via the marketplace (PDF, notes, exercises)
- **Manage group lesson bookings** with live payment status and timers
- **Parent account** — manage multiple children from a single account
- **Referral program** — earn XP bonuses by inviting friends with a personal code
- **Real-time notifications** — lesson reminders, reschedule requests, new messages

---

## For Tutors

- **Professional public profile** with bio, teaching style tags, certificates, student reviews and pinned achievements
- **Flexible availability management** — weekly schedule, per-slot duration, break configuration, days off
- **Individual lessons** — bookings, cancellations (always 100% refund), reschedule proposals with counter-offer flow
- **Group lessons** — dynamic per-person pricing, participant queue, accept/reject flow, 4-hour payment deadline timer
- **Lesson Room** — built-in video, whiteboard, chat, quizzes and mini-games, no external tools needed
- **Materials marketplace** — upload PDFs, set visibility (private / share with students / marketplace), sell with lifetime or time-limited access
- **Quiz creator** — 5 built-in templates, assign to students or publish publicly (unlocked after 20 lessons)
- **Mini-game editor** — 6 game types, assign to students or publish
- **Identity and qualification verification** — document upload, trust badge visible on profile
- **Earnings dashboard** — revenue history, monthly breakdown, weekly stats, payout management
- **Subscription plans** — tiered plans reducing platform commission and expanding capabilities
- **Stripe Connect** — direct payout setup via Stripe for receiving earnings
- **Onboarding tutorial** — interactive step-by-step guide for new tutors
- **Statistics panel** — lessons count, student count, average rating, income over time
- **Real-time notifications** — new bookings, payment confirmations, student messages, review alerts

---

## Lesson Room

A fully built-in space for conducting online lessons — no Zoom, no Google Meet needed:

| Tool | Description |
|------|-------------|
| **Video** | Real-time audio and video connection |
| **Whiteboard** | Shared collaborative drawing and writing board, export to PNG |
| **Chat** | Built-in real-time text chat (WebSocket) |
| **Quizzes** | Tutor sends a quiz, student solves it live with instant results |
| **Mini-games** | 6 types of interactive educational games playable during the lesson |
| **Materials** | File sharing and access during the lesson |
| **Timer** | Lesson countdown visible to the tutor |
| **Rating flow** | Student rates the lesson only after the tutor ends it |

Group lesson rooms support multiple participants simultaneously.

---

## Gamification System

Learning on Sprelli is also fun. The platform features a full motivation system for both students and tutors:

- **XP (experience points)** earned for completed lessons, quizzes, streaks and achievements
- **9 levels** — from Beginner to Education Colossus — with custom SVG icons per level
- **Streak** — consecutive days of activity with XP milestone rewards (3, 7, 14, 30, 60, 100 days)
- **Achievements** — badges across 6 categories: lessons, quizzes, materials, streak, social, milestones
- **Pinned achievements** — up to 3 badges displayed on the public profile
- **Learning goals** — tutor creates goals with milestones, student marks them complete
- **XP leaderboard** and public creator profiles

---

## Materials Marketplace

Tutors can monetize their educational content:

- Upload files (PDF, DOCX, images) with configurable visibility
- Set access type: lifetime or time-limited (7 / 14 / 30 days)
- Students browse, preview and purchase materials
- **DRM protection** — watermark overlay and pointer-events blocking on purchased content previews
- Ratings and reviews on marketplace materials
- Admin can moderate, block authors and manage listings

---

## Booking & Payments

- Full booking flow with calendar-based slot selection
- **Stripe** integration — card payments and BLIK (Polish instant payment)
- **Right of withdrawal** checkbox — legally required, visible on every booking
- Idempotent payment processing — no double charges
- Automatic refunds on teacher cancellation (always 100%)
- Group lessons with partial payment tracking per participant
- Reschedule proposal → counter-offer → accept/reject flow
- Payment history and invoice download in student and tutor panels

---

## Messaging

- Real-time direct messaging between students and tutors (WebSocket, Redis pub/sub)
- In-lesson chat within the Lesson Room
- New message email notifications via Resend
- Admin can view and moderate conversations

---

## Admin Panel

A full-featured internal management system with 40 pages:

| Area | Capabilities |
|------|-------------|
| **Dashboard** | Revenue KPIs, lesson counts, new registrations, support ticket overview |
| **Users** | List, search, filter, view profiles, manage roles, ban/unban |
| **Teachers** | Verification queue, document review, approve/reject with feedback |
| **Lessons** | All platform lessons — filter by status, teacher, date |
| **Group lessons** | Platform-wide group lesson management |
| **Payments** | Transaction list, hold/release payouts, commission tracking |
| **Payouts** | Tutor payout management with filters and status tracking |
| **Disputes** | Complaint timeline, partial refunds, reject with reason, user warnings |
| **Support tickets** | Ticket queue, respond, escalate, resolve |
| **Moderation** | Activity log, warn user, block account |
| **Audit log** | Full record of admin actions for accountability |
| **Materials** | Set price, block author, manage marketplace listings |
| **Quizzes** | Block author, manage public quiz library |
| **Gamification** | Edit achievement definitions, view XP leaderboard |
| **Subscriptions** | User subscription management, plan changes |
| **Marketing hub** | Campaigns, newsletter subscribers, push notifications, discount codes, email templates editor, banners/popups |
| **Banners** | Create system-wide banners and popups visible in user panels |
| **Reviews** | Moderate student reviews |
| **Analytics** | Revenue charts, user growth, lesson volume, marketplace metrics |
| **Reports** | Exportable reports |
| **Activity** | Platform-wide activity feed |
| **Alerts** | System alerts and monitoring |
| **Messages** | Admin messaging oversight |
| **Performance** | Platform performance monitoring |
| **Security** | Security settings and logs |
| **System** | Platform-wide system settings |
| **Settings** | Admin account and configuration |
| **Accounts** | Account management tools |
| **Calculator** | Internal pricing calculator |
| **Test room** | Internal lesson room test environment |
| **Invoices** | Invoice management |

---

## Real-Time Features

Built on **WebSockets** with **Redis pub/sub**:

- Live lesson chat (student ↔ tutor, per lesson room)
- Collaborative whiteboard — shared drawing state synced in real time
- Real-time notifications — lesson start alerts, reschedule requests, payment confirmations
- Group lesson participant status updates
- Quiz delivery and result collection during live lessons

---

## Tech Stack

**Frontend**
- Next.js 16 (App Router) + React 19 + TypeScript 5
- Tailwind CSS 4 — responsive design, full dark mode support
- PWA — installable app on mobile (Android + iOS)
- Lucide React icons, custom CSS animation system

**Backend — 28 API modules**
- Python + FastAPI — high-performance async API
- PostgreSQL — relational database (54+ tables)
- Redis — sessions, WebSocket pub/sub, task queues, token blacklist
- JWT authentication (15-minute access token + 30-day httpOnly refresh cookie)
- Gunicorn + Uvicorn workers (4 workers in production)
- Alembic — database migrations

**Infrastructure**
- Frontend: Vercel (global CDN, auto-deploy on push)
- Backend: Railway (auto-scaling, health checks)
- File storage: AWS S3 with presigned URLs (European region)
- Payments: Stripe (cards, BLIK, Stripe Connect for tutor payouts)
- Transactional email: Resend (27 email templates)
- CI/CD: GitHub Actions — pytest + ruff on every PR, Playwright E2E tests
- Monitoring: Uptime Kuma, Grafana metrics endpoint

**Security**
- HTTPS + HSTS (2 years, preload)
- Content Security Policy (full whitelist)
- Rate limiting on registration (3/min) and login (5/min) endpoints
- AI bot blocking middleware — 14 known crawlers blocked with 403
- Source maps disabled in production
- Admin panel isolated login (separate from user auth)
- CORS restricted to `sprelli.com` only
- `X-Robots-Tag: noai, noimageai` on all responses

---

## Legal Compliance

The platform operates in full compliance with Polish and European law:

- **GDPR / RODO** — data export, account deletion, granular marketing consent management
- **CMP (Cookie Consent)** — granular cookie manager with saved preferences per category
- **Right of withdrawal** — legally prescribed text visible on every booking (Electronic Services Act)
- **6 legal documents** — Terms of Service, Privacy Policy, Tutor Terms, Cookie Policy, Payment Terms, Complaints Policy
- **Dispute & refund system** — built-in complaint flow with partial and full refund support
- **Compliance router** — dedicated backend module for all GDPR operations

---

## SEO & GEO

Built for organic search and AI-driven discovery from day one:

**Content**
- **21 blog articles** targeting high-intent educational keywords
- Dynamic landing pages for every subject × city combination — `/korepetycje/[subject]/[city]`
- **Matura prep pages** — `/matura/[subject]` and `/matura/[subject]/[city]`
- **Egzamin ósmoklasisty pages** — per subject, targeting middle school exam queries
- **Education level pages** — `/korepetycje-dla/[poziom]`
- **Online tutoring pages** — `/korepetycje-online/[city]` per major Polish city
- **Competitor comparison pages** — `/sprelli-vs/[competitor]`
- **Price guide, how-to guides, FAQ** — high-volume informational queries

**Technical SEO**
- Dynamic XML sitemap covering all routes with priorities
- `robots.txt` — Googlebot permitted, scrapers blocked
- Canonical URLs, Open Graph, Twitter Card meta on every page
- `hreflang` for international targeting
- Custom 404 that doesn't expose internal paths

**Structured data (JSON-LD)**
- `BreadcrumbList`, `FAQPage`, `Course`, `HowTo`, `Service` schemas
- Teacher profile pages with individual structured data

**GEO (Generative Engine Optimization)**
- `X-Robots-Tag: noai, noimageai` — content protection from AI training
- AI bot blocking middleware (14 crawlers → 403)
- Content structured for AI answer engines (headings, Q&A format, definitions)
- FAQ schema enabling Sprelli answers in AI-generated search responses

---

## Project Scale

- **116 pages** and subpages in the application
- **Student panel** — 16 dedicated pages with full API integration
- **Tutor panel** — 18 dedicated pages with full API integration
- **Admin panel** — 40 pages covering every aspect of platform management
- **42 public pages** — landing pages, SEO content, legal documents, auth flows
- **47 reusable frontend components**
- **28 backend API modules**
- **54+ database tables**
- **21 blog articles** with SEO-targeted content
- **Dynamic SEO landing pages** across subjects, cities, levels and exam types
- **27 transactional email templates**
- **6 types of educational mini-games** with a built-in creator for tutors
- **5 quiz templates** for rapid quiz creation
- **4 subscription tiers** with commission-based differentiation
- **Referral program** with unique codes and XP bonuses

---

## Status

The platform is actively developed and being prepared for launch on the Polish market.

**Contact:** support@sprelli.com
**Website:** [sprelli.com](https://sprelli.com)

---

*SPRELLI Sp. z o.o. — Poland*
