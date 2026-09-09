# Search Queries for Job Scraper

## Installed portal CLIs (primary for `/scrape`)

`/scrape` discovers every portal skill under `.agents/skills/*/SKILL.md` and runs its CLI first. Shipped country-agnostic CLIs include `linkedin-search` and `freehire-search`; Danish demos remain **disabled** (US market). You do **not** need a matching `site:` line below for those CLIs to run.

The `site:` query templates in this file are the **WebSearch fallback** — for portals without a CLI, company career pages, or when a CLI fails.

**Language scope:** all queries in English (US market). Eshaan also works in Hindi, Spanish, and Mandarin — no separate query languages needed, but per `04-job-evaluation.md`'s Language Gate, postings requiring those languages pass.

**Cycle context:** searching for **Summer 2027 internships**. Consulting/finance/quant deadlines open earliest (Aug–Jan); tech and analytics roll later. Always include "2027" or "summer 2027" in internship queries to avoid stale 2026 postings.

## Search Sites

Primary:
- **linkedin.com/jobs** - covered by `linkedin-search` CLI (filter: United States; NYC + SF Bay Area first)
- **Handshake (joinhandshake.com / stanford.joinhandshake.com)** - Stanford's internship board; check manually, no CLI
- **indeed.com** - general US board
- Company career pages directly — most Priority 1/2 targets recruit via their own portals (see `documents/targets-and-networking.md` for saved application links)

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for known target companies

## Query Categories

### Priority 1: Strategy & Analytics at Elite Firms

**Calibration (Eshaan, 2026-08-09):** lead with strategy & analytics roles at big-name firms — archetypes are Jane Street Strategy & Product and D.E. Shaw Strategy & BD. Mid-tier finds go in a clearly-labeled secondary list, never the headline. Many elite 2027 postings open late 2026-early 2027: check the watch list by name every run, don't conclude "nothing new."

Elite watch list (check career pages directly every run):
- **Jane Street** — Strategy & Product Internship (janestreet.com/join-jane-street/open-roles)
- **D.E. Shaw** — Strategy & Business Development Intern (deshaw.com/careers)
- **BlackRock** — 2027 Summer Internship AMERS (careers.blackrock.com)
- **Citadel / Citadel Securities** — Associate Program (citadel.com/careers)
- **Bain** (ACI — Aug 31), **McKinsey** (2028-cycle opens ~Jan 2027), **BCG** (~Jan-Feb 2027)
- **Capital One** — Strategy Consulting intern (opens Aug 17, 2026), Data Analyst intern (capitalonecareers.com)
- **SpaceX** — Business Operations Internship (greenhouse.io/spacex; apply within 48-72h of posting)
- **Amazon** — Ops Finance Rotational + BI intern roles (amazon.jobs)
- **Point72, Bridgewater, SIG, Optiver, IMC** — business/strategy tracks first, quant tracks secondary
- **Google** — BizOps/Strategy intern; **Goldman Sachs, Morgan Stanley** — 2027 summer analyst (open ~fall 2026)

```
site:janestreet.com strategy product internship
site:deshaw.com strategy OR "business development" intern
site:linkedin.com/jobs "strategy intern" OR "business strategy intern" summer 2027 New York OR "San Francisco"
site:linkedin.com/jobs "associate consultant intern" 2027
site:bain.com "associate consultant intern" 2027
site:greenhouse.io spacex "business operations" internship 2027
site:capitalonecareers.com strategy consulting intern 2027
```

### Priority 2: Energy & Infrastructure Investing

Domain expertise. DESRI is the top named target.

```
site:linkedin.com/jobs "investment intern" OR "investment analyst intern" energy OR infrastructure OR renewables 2027
site:linkedin.com/jobs "infrastructure" "summer analyst" 2027
site:desri.com careers OR intern
site:linkedin.com/jobs "climate" OR "clean energy" intern investing OR finance New York OR "San Francisco"
site:linkedin.com/jobs "private equity intern" infrastructure OR energy 2027
site:linkedin.com/jobs "asset management" "summer analyst" infrastructure 2027
```

### Priority 3: Analytics, Sportsbook & Business Intelligence

Leverages EXL sportsbook analytics project + BI skills.

```
site:linkedin.com/jobs "analytics intern" FanDuel OR DraftKings
site:draftkings.com intern OR internship
site:fanduel.com careers intern
site:linkedin.com/jobs "business intelligence intern" OR "data analyst intern" summer 2027 New York OR "San Francisco"
site:linkedin.com/jobs "business analytics intern" 2027
```

### Priority 4: Big Tech, Data-Center Strategy & SWE (wider net)

```
site:linkedin.com/jobs "software engineering intern" summer 2027
site:linkedin.com/jobs "data center" strategy OR operations intern 2027
site:linkedin.com/jobs "data science intern" summer 2027 New York OR "San Francisco" OR Seattle
site:google.com/about/careers intern infrastructure OR "data center" 2027
```

## Target-Company Watch List

When scraping, also check these companies by name (full list with contacts in `documents/targets-and-networking.md`):
Bain, D.E. Shaw, Jane Street, Baringa, Deloitte, McKinsey, DESRI, BlackRock, Macquarie, Ares, JP Morgan (Infrastructure), Jefferies, Tiger Global, Fervo Energy, Tesla, Schneider Electric, GE Vernova, Digital Realty, FanDuel, DraftKings, Amazon, Cisco, Capital One, Google, xAI, Apple, Databricks, Susquehanna (SIG), IMC Trading.

## Location Filter

In-person preferred. Tiers:
- **Ideal:** New York City; San Francisco / Bay Area (incl. Palo Alto, Menlo Park, Mountain View)
- **Acceptable:** Seattle, Los Angeles, Chicago
- **Borderline:** other major US metros (Boston, Austin, Denver, Houston, DC) — flag, don't drop
- **Flag:** fully remote (prefers in-person, not excluded); outside US

## Compensation Filter

Flag any internship paying under ~$35/hr, unpaid, or stipend-only — Eshaan explicitly wants to out-earn his summer 2025 rate. Consulting/finance/big-tech intern rates clear this easily; research and nonprofit roles often don't.

## Language Filter

Working languages and levels are in CLAUDE.md's Languages table (English native, Hindi fluent, Spanish proficient, Mandarin intermediate). Apply `04-job-evaluation.md`'s Language Gate: a posting requiring an undeclared language is excluded; a posting requiring a higher level than declared is flagged, not excluded.

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not yet passed. If a posting date cannot be determined, include it but flag as "date unknown". For internships, also flag any posting whose target summer is 2026 (stale cycle).

## Adapting Queries

If the user specifies a focus area, select queries from the matching category and also generate 2-3 custom queries for that focus. For example:
- "/scrape consulting" -> Priority 1 queries + custom Bain/Deloitte/Baringa page checks
- "/scrape sportsbook" -> Priority 3 queries + FanDuel/DraftKings career pages
