# N Page Digital — Complete Site Package

This is the full, current state of the site — 37 real pages, verified with zero rendering errors, ready to push to GitHub.

## What's included

- **Homepage** — hero, real case study results, draft testimonials pending client approval, subtle grid background
- **6 Service pages** — SEO, Local SEO & GBP, Google Ads & PPC, Social Media Marketing, AI Marketing & Automation, Website Design
- **9 Industry pages** — Dental Clinics, Hospitals & Clinics, Real Estate, Restaurants & Hospitality, Interior Designers, Education, E-commerce & Retail, Law Firms, Astrology
- **Learning Hub** — 4 category pages, 8 published blog posts, all interlinked, all with FAQ sections
- **Free Tools** — a hub page plus 3 real, tested interactive tools: UTM Builder, WhatsApp Link Generator, Meta Title & Description Generator
- **1 Demo site** — Nakshatra Jyotish, showcased on the Astrology industry page
- **About, Contact, Privacy Policy, Terms of Service**
- **schema markup** — every single page above has valid JSON-LD (Organization, Service, FAQPage, BlogPosting, WebApplication, or CollectionPage as appropriate)
- **sitemap.xml** — all 37 URLs, verified as well-formed XML
- **robots.txt** — allows AI citation crawlers (OAI-SearchBot, PerplexityBot, Claude-SearchBot, etc.), blocks AI training crawlers (GPTBot, ClaudeBot, Google-Extended)
- **Deployment workflow** (`.github/workflows/deploy.yml`) — GitHub Actions → Hostinger via FTP, triggers automatically on every push to `main`

## What's genuinely still outstanding

- **Real testimonials** — homepage currently shows 5 honest draft quotes clearly marked "pending client approval," not real client statements
- **GBP service-area business setup** — a free change in your Google Business Profile account, still unconfirmed
- **Legal review** — Privacy Policy and Terms of Service are standard templates, not reviewed by an actual lawyer. Do this before relying on them, especially given India's DPDP Act (2023)
- **Blog post publish dates** — each post's schema currently has `"datePublished": "2026-09-02"` (today, when this was built) as a placeholder. Update these to the actual date each post goes live, for accuracy
- **AI Visibility Checker** — a 4th tool exists as a built file but is intentionally excluded from the nav, hub page, and sitemap, since it's a self-assessment checklist rather than a genuine live AI scan. Not included in this package's public/tools/ folder

## How to push this to GitHub

1. Unzip this package
2. If you already have the repo cloned via GitHub Desktop, delete the old contents of that folder and copy everything from this unzipped package in instead (on Mac, press Cmd+Shift+. in Finder first so the hidden `.github` folder actually copies)
3. If not yet cloned: open GitHub Desktop → File → Clone Repository → paste `https://github.com/NabaDutta/N-Page-Digital.git`
4. In GitHub Desktop: you should see roughly 37+ changed files listed under "Changes." Write a commit summary like "Full site — schema, Free Tools, Learning Hub complete," click "Commit to main," then "Push origin"

## Before this actually goes live on Hostinger

Add these three secrets in the GitHub repo's Settings → Secrets and variables → Actions:
- `FTP_SERVER`
- `FTP_USERNAME`
- `FTP_PASSWORD`

All three come from Hostinger's hPanel → Files → FTP Accounts. Until these are set, pushing to `main` will trigger the deploy workflow but it will fail at the FTP step — that's expected, not a bug.
