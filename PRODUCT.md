# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

General portfolio visitors: anyone who wants to see what Mert Lafcı builds and how. No single audience is prioritized (owner's decision, 2026-11-21); the site is a portfolio, not a job-application page or a support page.

## Product Purpose

A single-page personal portfolio for Mert Lafcı as an independent developer. It presents three shipped apps, explains how he works, and gives a way to get in touch. The owner is satisfied with the current content and how it is presented; future work refines it rather than repositioning it.

## Positioning

Real, shipped products with concrete technical claims, built by one person who owns scope, decisions, testing and releases while AI agents write most of the code in a branch / pull request / CI workflow.

## Operating Context

- Static site on GitHub Pages at mertlafci.com: one `index.html` (inline CSS and JS) plus `assets/`. No build step, no framework.
- Bilingual: English by default, Turkish available via toggle or `?lang=tr`; the choice is saved in `localStorage`.
- Visitors arrive from links to the domain; the page links out to the App Store, Google Play, GitHub repos and release downloads, and LinkedIn.

## Capabilities and Constraints

- Sections: hero, Projects, How I work, Contact.
- Exactly three projects: Meridyen Terapi Asistanı (iOS and Android, live in Turkey, subscription), HiFi Companion (macOS, open source), PocketPaste (Android to Mac, open source).
- Stays a single static page with no build step.

## Brand Commitments

- Name: Mert Lafcı. Title: "Independent Developer" / "Bağımsız Geliştirici".
- Both languages stay; English is the default.
- Out of scope by owner's choice: corporate career history, music and audio-engineering background, hi-fi reviewing.
- Voice: plain, factual, no hype; Turkish copy reads naturally, not as a translation.
- Contact address is the owner's personal email for now; it may move to a domain address later.

## Evidence on Hand

- App screenshots in `assets/`: `meridyen-calendar.jpg`, `meridyen-clients.jpg`, `hifi-companion-eq-light.jpg`, `hifi-companion-eq-dark.jpg`, `pocketpaste-menu.jpg`; link-preview image `og-cover.jpg`.
- Verifiable claims already on the page: row-level security for therapist data (Meridyen), bit-exact audio path with a flat EQ verified by a null test (HiFi Companion), AES-256-GCM with a key shared only through the pairing QR code (PocketPaste).
- Absent and not to be fabricated: testimonials, user or download counts, revenue, client names, ratings.

## Product Principles

1. Show real work; every claim must be one the owner can back up.
2. Keep it to one page that is quick to read.
3. Treat both languages as equals.
4. Let the products carry the page; the chrome stays out of their way.
