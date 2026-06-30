# Sprelli — Online Tutoring Platform

**Sprelli** is a modern educational marketplace connecting students with verified tutors in Poland. The platform enables booking individual and group lessons, learning through interactive tools, and tracking progress — all in one place.

---

## What is Sprelli?

Sprelli is a complete educational platform where:

- **Students** (and parents) can find a verified tutor, book a lesson and pay securely online
- **Tutors** build their brand, manage their schedule, sell educational materials and teach without any external tools
- **Schools and institutions** can use the platform to complement their educational offering

Our mission: democratize access to high-quality tutoring in Poland.

---

## For Students

- **Search and filter** tutors by subject, level, price and availability
- **Book lessons** — individual or group — with verified tutors
- **Learn online** in a dedicated Lesson Room with video, whiteboard, chat and quizzes
- **Track progress** — XP points, levels, learning streaks, achievements and goals
- **Solve quizzes and play educational games** assigned by your tutor or from the public library
- **Buy educational materials** from tutors via the marketplace
- **Parent account management** — dedicated panel for parents of children

---

## For Tutors

- **Professional profile** with bio, teaching styles, certificates and student reviews
- **Flexible scheduling** — precise availability control, breaks between lessons, days off
- **Individual and group lessons** — full management: bookings, cancellations, reschedules
- **Lesson Room** with video conferencing, shared whiteboard, materials and live quizzes
- **Materials marketplace** — sell PDFs, notes and exercises directly to students
- **Quiz and mini-game creator** for your students (6 types of educational games)
- **Identity and qualification verification** — trust badge visible on your public profile
- **Statistics dashboard** — earnings, student count, ratings and lesson history
- **Subscription plans** — expand your capabilities and reduce commission

---

## Lesson Room

A fully built-in space for conducting online lessons:

| Tool | Description |
|------|-------------|
| **Video** | Real-time audio and video connection |
| **Whiteboard** | Shared drawing and writing board, PNG export |
| **Chat** | Built-in text chat |
| **Quizzes** | Tutor sends a quiz, student solves it live |
| **Materials** | File sharing during the lesson |
| **Mini-games** | 6 types of interactive educational games |
| **Timer** | Lesson countdown visible to the tutor |

Group lessons support multiple participants with dynamic per-person pricing.

---

## Gamification System

Learning on Sprelli is also fun. The platform features a full motivation system:

- **XP (experience points)** for completed lessons, quizzes and learning streaks
- **9 levels** — from Beginner to Education Colossus
- **Streak** — consecutive days of activity with XP rewards at milestones (3, 7, 14, 30, 60, 100 days)
- **Achievements** — badges across 6 categories (lessons, quizzes, materials, streak, social, milestones)
- **Learning goals** — tutor sets goals with milestones, student completes them
- **Leaderboards** and public profiles with pinned achievements

---

## Tech Stack

Sprelli is built on a modern, battle-tested technology stack:

**Frontend**
- Next.js 16 (App Router) + React 19 + TypeScript 5
- Tailwind CSS 4 — responsive design, dark mode
- PWA — installable app on mobile devices

**Backend**
- Python + FastAPI — high-performance async API
- PostgreSQL — relational database
- Redis — sessions, task queues, WebSocket pub/sub
- JWT authentication with automatic token refresh

**Infrastructure**
- Frontend hosting: Vercel (global CDN)
- Backend hosting: Railway (auto-scaling)
- File storage: AWS S3 (European region)
- Payments: Stripe (cards, BLIK)
- Transactional email: Resend
- CI/CD: GitHub Actions (automated tests on every PR)

**Security**
- HTTPS + HSTS
- Full GDPR / RODO compliance
- Rate limiting on registration and login endpoints
- Content Security Policy
- AI bot blocking (content protection)

---

## Legal Compliance

The platform operates in full compliance with Polish and European law:

- **GDPR / RODO** — data export, account deletion, marketing consent management
- **CMP (Cookie Consent)** — granular cookie management with saved preferences
- **Terms of Service**, Privacy Policy, Tutor Terms, Cookie Policy — complete legal documentation
- **Right of withdrawal** — visible on every booking in accordance with the Electronic Services Act
- **Dispute handling** — built-in complaint and refund system

---

## SEO & GEO

Sprelli is built with organic search and AI-driven discovery in mind from the ground up:

**Content infrastructure**
- **21 blog articles** targeting high-intent educational keywords (exam prep, subject guides, tutoring tips)
- **Dynamic landing pages** for every subject × city combination — `/korepetycje/[subject]/[city]`
- **Matura prep pages** — `/matura/[subject]` and `/matura/[subject]/[city]`
- **Egzamin ósmoklasisty pages** — per subject, targeting middle school exam queries
- **Education level pages** — `/korepetycje-dla/[poziom]` (primary, secondary, university)
- **Online tutoring pages** — `/korepetycje-online/[city]` per major Polish city
- **Competitor comparison pages** — `/sprelli-vs/[competitor]`
- **Price guide** — `/ile-kosztuja-korepetycje` targeting high-volume cost queries

**Technical SEO**
- Dynamic XML sitemap generated at build time covering all routes and priorities
- `robots.txt` with precise crawler rules — Googlebot permitted, content scrapers blocked
- Canonical URLs on all pages to prevent duplicate content
- Open Graph and Twitter Card meta on every page
- `hreflang` tags for international targeting

**Structured data (JSON-LD)**
- `BreadcrumbList` — navigation context for all nested pages
- `FAQPage` — rich results for FAQ and common questions
- `Course` — tutor subject pages eligible for Google course rich results
- `HowTo` — step-by-step guides (how to find a tutor, how to prepare for exams)
- `Service` — platform and subject service schema
- Teacher profile pages with individual structured data

**GEO (Generative Engine Optimization)**
- `X-Robots-Tag: noai, noimageai` — prevents content from being used in AI training datasets without consent
- AI bot blocking middleware on the backend — 14 known AI crawlers return 403
- Content structured for AI answer engines (clear headings, definitions, Q&A format in blog)
- FAQ schema enabling Sprelli answers to appear directly in AI-generated search responses

---

## Project Scale

- **116 pages** and subpages in the application
- **Student panel** — 16 dedicated pages with full API integration
- **Tutor panel** — 18 dedicated pages with full API integration
- **Admin panel** — 40+ pages covering moderation, analytics, payouts, marketing and verification
- **47 reusable components** across the frontend
- **21 blog articles** with SEO-targeted content
- **Dynamic SEO landing pages** across subjects, cities, levels and exam types
- **27 transactional email templates** (welcome, booking, cancellation, reschedule, refund, verification, group lessons, password reset and more)
- **6 types of educational mini-games** with a built-in creator for tutors
- **Referral program** with unique codes and XP bonuses

---

## Status

The platform is actively developed and being prepared for launch on the Polish market.

**Contact:** support@sprelli.com  
**Website:** [sprelli.com](https://sprelli.com)

---

*SPRELLI Sp. z o.o. — Poland*
