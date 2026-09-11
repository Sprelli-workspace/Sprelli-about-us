# Sprelli - Online Tutoring Platform

**Sprelli** is a modern educational marketplace connecting students, parents, and verified tutors in Poland. The platform enables booking individual, group, and package lessons, real-time learning through interactive tools, progress tracking, and content monetization - all in one place, without any external tools.

---

## What is Sprelli?

Sprelli is a complete educational platform where:

- **Students** can find a verified tutor, book a lesson, and pay securely online
- **Parents** can browse tutors, request a match, book a multi-lesson package with flexible payment plans, and follow their child's progress from a dedicated panel
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
- **Referral program** — earn XP bonuses by inviting friends with a personal code
- **Real-time notifications** — lesson reminders, reschedule requests, new messages

---

## For Parents

A dedicated panel for parents who want a hands-off, managed experience rather than booking lesson-by-lesson:

- **Request a match** — describe the subject, level and availability, get matched with suitable tutors, or browse and choose directly
- **Lesson packages** — book a recurring block of lessons (e.g. 24 over 6 months) with a fixed price per lesson
- **Flexible payment plans** — pay upfront or in installments, with automatic retry and dunning on failed payments
- **Multi-child support** — manage more than one child's lessons and packages from a single account
- **Progress notes** — tutors leave a short note after every lesson, visible to the parent
- **Reschedule and cancellation flow** — request a new time, with a fair-use limit before lessons convert to a makeup lesson at the end of the schedule
- **Direct messaging** with the assigned tutor
- **Help request intake** — a simple "help me get set up" form for parents who prefer a human to walk them through registration

Tutors opt in to the parent pool separately (accepting dedicated terms) before they can be matched with parent requests.

---

## For Tutors

- **Professional public profile** with bio, teaching style tags, certificates, student reviews and pinned achievements
- **Flexible availability management** - weekly schedule, per-slot duration, break configuration, days off
- **Individual lessons** - bookings, cancellations (always 100% refund), reschedule proposals with counter-offer flow
- **Group lessons** - dynamic per-person pricing, participant queue, accept/reject flow, 4-hour payment deadline timer
- **Parent packages** - recurring lesson blocks booked by parents, with automatic scheduling and payout on completion
- **Lesson Room** - built-in video, whiteboard, chat, quizzes and mini-games, no external tools needed
- **Materials marketplace** - upload PDFs, set visibility (private / share with students / marketplace), sell with lifetime or time-limited access
- **Quiz creator** - 5 built-in templates, assign to students or publish publicly (unlocked after 20 lessons)
- **Mini-game editor** - 6 game types, assign to students or publish
- **Identity and qualification verification** — document upload, trust badge visible on profile
- **Earnings wallet** - lesson earnings accrue to an in-platform balance and can be withdrawn on demand; full Stripe identity/payout verification (KYC) is only required at the moment of a tutor's first withdrawal, not before — so a new tutor can be listed, booked and paid without clearing Stripe first
- **Subscription plans** - tiered plans reducing platform commission and expanding capabilities
- **Founders program** - the first 100 verified tutors receive the top subscription tier free for 90 days
- **Onboarding tutorial** - interactive step-by-step guide for new tutors
- **Statistics panel** - lessons count, student count, average rating, income over time
- **Real-time notifications** - new bookings, payment confirmations, student messages, review alerts

---

## Lesson Room

A fully built-in space for conducting online lessons - no Zoom, no Google Meet needed:

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
- **9 levels** - from Beginner to Education Colossus — with custom SVG icons per level
- **Streak** - consecutive days of activity with XP milestone rewards (3, 7, 14, 30, 60, 100 days)
- **Achievements** - badges across 6 categories: lessons, quizzes, materials, streak, social, milestones
- **Pinned achievements** - up to 3 badges displayed on the public profile
- **Learning goals** - tutor creates goals with milestones, student marks them complete
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
- **Stripe** integration - card payments and BLIK (Polish instant payment)
- **Wallet-based payouts** - tutor earnings accrue in an internal ledger with a short holding period (protects against refunds/chargebacks) before becoming withdrawable; the platform tracks its own reserve against every payout obligation
- **Right of withdrawal** checkbox - legally required, visible on every booking
- Idempotent payment processing - no double charges
- Automatic refunds on teacher cancellation (always 100%)
- Group lessons with partial payment tracking per participant
- Parent packages with upfront or installment payment plans, automatic dunning on failed installments
- Reschedule proposal → counter-offer → accept/reject flow
- Payment history and invoice download in student and tutor panels

---

## Messaging

- Real-time direct messaging between students and tutors (WebSocket, Redis pub/sub)
- Direct messaging between parents and their assigned tutor
- In-lesson chat within the Lesson Room
- New message email notifications via Resend
- Admin can view and moderate conversations

---

## Trust & Safety

- **Identity and qualification verification** for tutors, with a document review queue and trust badge
- **Anti-fraud signup engine** - a risk-scoring layer evaluates every new registration (disposable emails, datacenter IPs, velocity, bot signatures) and can quarantine suspicious accounts for review
- **Child safety compliance** - dedicated safeguards for tutors working with minors through the parent panel
- **Moderation tools** - warnings, account blocks, and a full activity/audit log for every admin action
- **Dispute & refund system** - built-in complaint flow with partial and full refund support

---

## Admin Panel

A full-featured internal management system covering every aspect of platform operations:

| Area | Capabilities |
|------|-------------|
| **Dashboard** | Revenue KPIs, lesson counts, new registrations, support ticket overview |
| **Users** | List, search, filter, view profiles, manage roles, ban/unban |
| **Teachers** | Verification queue, document review, approve/reject with feedback |
| **Lessons** | All platform lessons - filter by status, teacher, date; reschedule and request revisions |
| **Group lessons** | Platform-wide group lesson management |
| **Parent pool** | Parent requests, tutor matching, package and installment oversight |
| **Payments** | Transaction list, hold/release payouts, commission tracking |
| **Wallet & payouts** | Tutor wallet balances, platform reserve vs. liabilities, withdrawal queue, ledger reconciliation |
| **Disputes** | Complaint timeline, partial refunds, reject with reason, user warnings |
| **Support tickets** | Ticket queue, respond, escalate, resolve |
| **Moderation** | Activity log, warn user, block account |
| **Audit log** | Full record of admin actions for accountability |
| **Materials** | Set price, block author, manage marketplace listings |
| **Quizzes** | Block author, manage public quiz library |
| **Gamification** | Edit achievement definitions, view XP leaderboard |
| **Subscriptions** | User subscription management, plan changes, founders program tracking |
| **Marketing hub** | Campaigns, newsletter subscribers, push notifications, discount codes, email templates editor, banners/popups |
| **Email deliverability** | Bounce/complaint monitoring, delivery health across all transactional and marketing email |
| **Banners** | Create system-wide banners and popups visible in user panels |
| **Reviews** | Moderate student reviews |
| **Analytics** | Revenue charts, user growth, lesson volume, marketplace metrics |
| **SEO & GEO tracking** | Search Console integration, keyword/city coverage dashboard |
| **Anti-fraud** | Signup risk scoring, quarantine queue, calibration controls |
| **Alerts** | Automated monitoring rules across revenue, payouts, disputes and platform health |
| **Reports** | Exportable reports |
| **Activity** | Platform-wide activity feed |
| **Messages** | Admin messaging oversight |
| **Security** | Security settings and logs |
| **System** | Platform-wide system settings, deploy/version tracking |
| **Settings** | Admin account and configuration |
| **Invoices** | Invoice management |

Fully responsive, including a slide-out navigation for phone use.

---

## Real-Time Features

Built on **WebSockets** with **Redis pub/sub**:

- Live lesson chat (student ↔ tutor, per lesson room)
- Collaborative whiteboard - shared drawing state synced in real time
- Real-time notifications - lesson start alerts, reschedule requests, payment confirmations
- Group lesson participant status updates
- Quiz delivery and result collection during live lessons

---

## Tech Stack

**Frontend**
- Next.js 16 (App Router) + React 19 + TypeScript 5
- Tailwind CSS 4 - responsive design, full dark mode support
- PWA — installable app on mobile (Android + iOS)
- Lucide React icons, custom CSS animation system

**Backend - 35 API modules**
- Python + FastAPI — high-performance async API
- PostgreSQL - relational database (100+ tables)
- Redis - sessions, WebSocket pub/sub, task queues, token blacklist
- ARQ - background worker for scheduled jobs and async task processing
- JWT authentication (15-minute access token + 30-day httpOnly refresh cookie)
- Gunicorn + Uvicorn workers (4 workers in production)
- Alembic - database migrations (75+ applied)

**Infrastructure**
- Frontend: Vercel (global CDN, auto-deploy on push)
- Backend: Railway (auto-scaling, health checks, SSH access for operations)
- File storage: AWS S3 with presigned URLs (European region)
- Payments: Stripe (cards, BLIK, Stripe Connect for tutor payouts)
- Transactional email: Resend (30+ email templates)
- Monitoring: Uptime Kuma, automated alert rules on revenue/payout/platform health

**Security**
- HTTPS + HSTS (2 years, preload)
- Content Security Policy (full whitelist)
- Rate limiting on registration, login and sensitive write endpoints
- Anti-fraud signup risk engine - scores every registration, quarantines high-risk accounts
- AI bot blocking middleware - known crawlers blocked with 403
- Source maps disabled in production
- Admin panel isolated login (separate from user auth)
- CORS restricted to `sprelli.com` only
- `X-Robots-Tag: noai, noimageai` on all responses

---

## Legal Compliance

The platform operates in full compliance with Polish and European law:

- **GDPR / RODO** — data export, account deletion, granular marketing consent management
- **CMP (Cookie Consent)** - granular cookie manager with saved preferences per category
- **Right of withdrawal** - legally prescribed text visible on every booking (Electronic Services Act)
- **6 legal documents** - Terms of Service, Privacy Policy, Tutor Terms, Cookie Policy, Payment Terms, Complaints Policy
- **Dispute & refund system** - built-in complaint flow with partial and full refund support
- **Child safety compliance** - dedicated process for tutors working with minors through the parent panel
- **Compliance router** - dedicated backend module for all GDPR operations

---

## SEO & GEO

Built for organic search and AI-driven discovery from day one:

**Content**
- **29 blog articles** targeting high-intent educational keywords
- **Over 4,200 indexed URLs** generated dynamically from subject, city and level combinations, served through a split sitemap index (core pages, geographic pages, tutor profiles) for cleaner indexing signals:

| URL pattern | Combinations | Count |
|-------------|-------------|-------|
| `/korepetycje/[subject]/[city]` | 35 subjects × 80 cities | 2,800 |
| `/matura/[subject]/[city]` | 14 subjects × 80 cities | 1,120 |
| `/korepetycje/[subject]/poziom/[level]` | 35 subjects × 4 levels | 140 |
| `/korepetycje-online/[city]` | 80 cities | 80 |
| `/korepetycje/[subject]` | 35 subjects | 35 |
| `/matura/[subject]` | 14 subjects | 14 |
| `/sprelli-vs/[competitor]` | 15 competitors | 15 |
| `/egzamin-osmoklasisty/[subject]` | 4 subjects | 4 |
| Static + blog + parent panel + other | - | ~68 |
| **Total** | | **~4,270** |

- **35 subjects** covered - from mathematics, languages and sciences to programming and music
- **80 Polish cities** - full nationwide geographic coverage
- **15 competitor comparison pages** - direct SEO targeting of alternative platform searches
- **Price guide, how-to guides, FAQ** - high-volume informational queries

**Technical SEO**
- Sitemap index split into core / geographic / tutor-profile sitemaps, each independently trackable in Search Console
- `robots.txt` - Googlebot permitted, scrapers blocked
- Canonical URLs, Open Graph, Twitter Card meta on every page
- `hreflang` for international targeting
- Custom 404 that doesn't expose internal paths

**Structured data (JSON-LD)**
- `BreadcrumbList`, `FAQPage`, `Course`, `HowTo`, `Service` schemas
- Teacher profile pages with individual structured data

**GEO (Generative Engine Optimization)**
- `X-Robots-Tag: noai, noimageai` - content protection from AI training
- AI bot blocking middleware
- Content structured for AI answer engines (headings, Q&A format, definitions)
- FAQ schema enabling Sprelli answers in AI-generated search responses
- In-house SEO/GEO tracking dashboard (Search Console data + manual AI-answer checks)

---

## Project Scale

- **192 pages** and subpages in the application
- **Student panel** - 14 dedicated pages with full API integration
- **Tutor panel** - 17 dedicated pages with full API integration
- **Parent panel** - 12 dedicated pages, launched as a new product line
- **Admin panel** - 46 pages covering every aspect of platform management
- **47+ reusable frontend components**
- **35 backend API modules**
- **100+ database tables**
- **29 blog articles** with SEO-targeted content
- **~4,270 dynamically generated URLs** - 35 subjects × 80 cities × levels × exam types × competitors
- **30+ transactional email templates**
- **6 types of educational mini-games** with a built-in creator for tutors
- **5 quiz templates** for rapid quiz creation
- **4 subscription tiers** with commission-based differentiation
- **Founders program** for the first 100 verified tutors
- **Referral program** with unique codes and XP bonuses

---

## Status

**Sprelli launched on the Polish market on September 10, 2026.** The platform is live and in active use, with continued development on the parent panel, tutor payouts, and search/AI visibility.

**Contact:** support@sprelli.com
**Website:** [sprelli.com](https://sprelli.com)

---

*SPRELLI Sp. z o.o. — Poland*
