---
framework_version: 1.0.0
---

# Interview Preparation Guide

<!-- SETUP: STAR examples are personalized by running /setup based on your actual experience -->

## STAR Format

Structure answers as: **Situation** (context), **Task** (your responsibility), **Action** (what you did), **Result** (outcome).

Keep answers to 1-2 minutes. Be specific. End with what you learned or would do differently.

## Ready-Made STAR Examples

<!-- These are populated by /setup from your actual experience. Below are templates showing the format. -->

### 1. SOURCE Climate Solutions - Client Pilots ($560K) (client-facing delivery, business development)
**S:** Joined the founding team of SOURCE Climate Solutions, an AI energy-efficiency startup expanding beyond its initial customers into commercial real estate and data centers.
**T:** Help win pilot projects — identify prospects, build the pitch, and carry client conversations alongside MBA teammates.
**A:** Prepared tailored pitch decks (PowerPoint, Tableau) per customer segment, drove insights-driven outreach, and led client-facing conversations through to close.
**R:** Secured pilot projects with Prologis, Primestor, and Stanford Facilities, generating $560K in profit for an early-stage startup.
**Use for:** "Tell me about a time you influenced/persuaded someone", "Describe working with clients", "Tell me about working in a fast-paced/ambiguous environment"

### 2. SOURCE Climate Solutions - Retrofit Analytics MVP (building product, data-driven iteration)
**S:** Engineers at SOURCE spent large amounts of manual time analyzing each building retrofit opportunity, throttling how many deals the team could evaluate.
**T:** Automate the analysis so the team could scale.
**A:** Designed an automated retrofit analytics MVP, A/B tested it against the manual workflow, and deployed it to the team.
**R:** Reduced engineer analysis time by 40%, directly increasing deal throughput.
**Use for:** "Tell me about a technical project you owned", "Describe improving a process", "How do you validate your work?"

### 3. Plug & Play - Investment Memos to Fortune 500 LPs (investment analysis, communicating to senior audiences)
**S:** As an energy investment analyst at Plug & Play (climate VC), the fund needed diligence on seed-round energy startups and theses on emerging areas.
**T:** Source and evaluate companies, and produce investment recommendations credible enough for the fund's LPs.
**A:** Sourced and scored 30+ startups via discovery calls, technical diligence, and market sizing; built Excel models for TAM/SAM/SOM, unit economics (LTV/CAC), and profitability projections feeding VC/DCF valuations; wrote three investment memos on grid resilience, data-center behind-the-meter energy supply, and maritime decarbonization.
**R:** Presented to Fortune 500 LPs including PG&E and Tokyo Gas, recommending potential 10x fund returners.
**Use for:** "Walk me through an analysis you did", "Tell me about presenting to senior stakeholders", "Why investing/finance?"

### 4. Enline Consulting Engagement - 37-Page Whitepaper (leadership, structured problem-solving)
**S:** Through Stanford Energy Club & Sustainable Investment Group, Enline (a grid-technology company) wanted advice on US market entry.
**T:** Co-lead a 14-member student team through a full consulting engagement.
**A:** Structured the work into competitive and regulatory analysis, pricing and moat assessment, and evaluation of non-traditional revenue channels (hyperscalers, insurers, utilities); managed the team to synthesis.
**R:** Delivered a 37-page whitepaper presented to Enline's board.
**Use for:** "Tell me about leading a team", "Describe a time you broke down an ambiguous problem", "Why consulting?"

### 5. IvyBound Consulting - Co-Founder & CFO (entrepreneurship, ownership, growth)
**S:** Co-founded IvyBound, a BIPOC-focused college consulting startup, in 2021 while in high school.
**T:** As CFO, own financial strategy and growth initiatives.
**A:** Launched group coaching, test prep partnerships, and ad campaigns across the US and Europe; managed pricing and finances while scaling the client base.
**R:** 32K+ followers, 67 clients, $230K+ revenue growth, 7-figure valuation — sustained over 4+ years.
**Use for:** "Tell me about something you built from scratch", "Describe long-term commitment/grit", "Tell me about a time you wore multiple hats"

### 6. Stanford Doerr - Groundwater & Wildfire Research (technical depth, communicating science to decision-makers)
**S:** California's Central Valley faces groundwater depletion, and stakeholders needed quantified evidence to allocate resources.
**T:** As a geophysics ML researcher, turn satellite data into decision-ready analysis.
**A:** Analyzed NASA InSAR/GRACE satellite data with Pandas and Sklearn to quantify depletion; produced geospatial maps for California government audiences; separately built a PyTorch wildfire prediction model.
**R:** Work informed resource allocation and $175M in infrastructure investment decisions; wildfire model showcased to Governor Green's Office, UH Manoa, and KIUC in Hawaii.
**Use for:** "Tell me about working with messy/real-world data", "Describe explaining something technical to a non-technical audience", "Tell me about your research"

### 7. EXL x NBA - Game Integrity Product (end-to-end product ownership, ML + product judgment)
**S:** Insider trading on NBA player prop bets is a federal-indictment-level liability for the league (Jontay Porter, Malik Beasley, Terry Rozier cases); the NBA needed to detect suspicious games before prosecutors do.
**T:** As EXL business analytics intern (summer 2026), build a working detection platform — data, model, and investigator-facing product.
**A:** Built Postgres pipelines over 32,385 player-games (NBA API box scores + play-by-play, 58,338 FanDuel prop quotes via OddsAPI, Basketball Reference salaries). Designed a three-signal suspicion score — performance (z-scored Hollinger game score + custom 9-stat effort metric + line shortfall), market (closing line/price and movement), motive (salary percentile) — weighted 0.45/0.30/0.25 by logistic regression, behind categorical screening gates (cut-then-rank, 32K → 4,811). Shipped a React/FastAPI "Season Ledger" dashboard with LLM-generated case summaries and PDF case reports. Tested and rejected alternatives (Isolation Forest, residualization, Polymarket signals) with documented reasoning.
**R:** All known flagged games rank in the top 0.4% of 32,385 player-games; model iteration moved their average rank from #1,918 to #75. Delivered final presentation; now developing the product into a startup pitch.
**Use for:** "Walk me through a product you built end-to-end", "How do you make modeling trade-offs?", "Tell me about a high-stakes/ambiguous problem" — lead example for FanDuel/DraftKings and any analytics/product role

### 8. Augmentage - Founding a Tokenized Infrastructure Exchange (market insight, initiative, domain depth)
**S:** Through VC diligence at Plug & Play and infra research, saw both sides of a structural problem: infra funds' capital locked in 10-12 year deals with no secondary liquidity, and retail investors locked out by $1M minimums — against a $106T infrastructure buildout through 2040.
**T:** As Founder & CEO, design a venue that solves both: a blockchain alternative trading system issuing small-lot tokenized yield notes on institutional infra assets.
**A:** Designed the full stack — ERC-3643 issuance, USDC T+0 settlement, Chainlink oracles carrying SCADA telemetry for live asset pricing; mapped the regulatory path (Reg D 506(c) now, Reg A+ later; partner broker-dealer under Reg ATS, own B-D in parallel — no new legislation needed post-GENIUS Act); built the business model (issuance fee + trading take + servicing + data licensing; one $30M tokenization ≈ $700K year-1 revenue); competitive analysis across Securitize/Ondo, Plural/Energea, Forge/EquityZen; recruited a CTO/advisor with 30+ years of institutional systems experience (Morgan Stanley, JPM, Citi). GTM: DESRI pilot via warm intro, then BlackRock GIP/Brookfield/Stonepeak.
**R:** Complete investor deck presented at YC Startup Expo; pilot conversations leveraging direct contacts at BlackRock GIP and DESRI.
**Use for:** "Why infrastructure/energy investing?" (the definitive answer), "Tell me about an opportunity you spotted that others missed", "Walk me through a market", "Tell me about something you're building" — lead with this at DESRI, BlackRock, and any infra/fintech interview

## Common Tough Questions

### "Your background is energy/climate — why consulting / quant strategy / sportsbook analytics?"
> Frame the through-line as *markets + analysis + client outcomes*, not a sector switch: "Energy is where I learned to do diligence, model businesses, and present to decision-makers — the skills transfer directly. I deliberately took a technical role this past summer; now I want the market- and investment-facing side." For FanDuel/DraftKings specifically: lead with the EXL sportsbook analytics project.

### "You don't have formal consulting/banking experience."
> Acknowledge, then bridge: the Enline engagement was a real consulting project with a real client board; the Plug & Play memos were real investment work presented to real LPs; IvyBound is a real P&L. "I've done the work — just through entrepreneurial channels rather than a brand-name employer. That's exactly what an internship is for."

### "Where do you see yourself in 5 years?"
> Investing or strategy work at the intersection of energy/infrastructure and technology — and publishing research on infrastructure market trends. Tailor the emphasis: consulting firms hear "post-MBA consultant or industry strategy"; investment firms hear "analyst → investor building sector depth."

### "What's your biggest weakness?"
> *(Draft — Eshaan should personalize.)* Candidate option: breadth over depth — involved in many things (VC, startup, research, founding a company); learning to concentrate effort on fewer, deeper bets. Mitigation: chose to spend summer 2025 fully embedded in one startup rather than juggling; applying the same focus to recruiting priorities now.

### "Why this company specifically?"
> Customize per company. Must reference: specific projects, company values, market position, or team structure. Never give a generic answer.

## Questions You Should Ask Interviewers

### About the Role
- "What does a typical week look like in this role?"
- "What would success look like in the first 6 months?"
- "What's the biggest challenge the team is facing right now?"

### About the Team
- "How big is the team, and how do you divide work?"
- "What does the development/project lifecycle look like, from idea to production?"
- "How do you onboard new team members?"

### About Tech & Growth
- "What's your current tech stack for [relevant area]?"
- "Is there room to grow into more architectural or strategic decisions?"
- "How does the team stay current with new tools and methods?"

### About Culture (use these to prevent disappointment)
- "How would you describe the team culture?"
- "What does professional development look like here?"
- "Is there flexibility for remote/hybrid work?"
- "What's the balance between development/new projects and maintenance work?"
- "How would you describe the leadership style in this team?"
- "What do people who thrive here have in common?"

## Phone/Video Interview Tips
- Have STAR examples written out (use this file)
- Keep a glass of water nearby
- Smile when speaking (it changes your tone)
- Ask for clarification if a question is vague
- It's OK to take 5 seconds to think before answering
- End with: "Is there anything else you'd like to know about my background?"

## After the Application (Best Practice)

### Follow-Up Etiquette
- **Don't call to "stand out"** or to learn more about the role post-submission - this risks a negative impression
- If the employer specified a timeline, respect it and wait
- If no timeline was given and significant time has passed (2+ weeks), a brief call to ask about status is acceptable
- If you have genuinely new, relevant information to share, a short follow-up is fine

### Thank-You Notes
- When you receive any update (interview invitation, rejection, or status update), send a brief thank-you message
- Express appreciation for their time and the process
- Keep it short (2-3 sentences)

## Roleplay Guidelines
When the user asks for interview practice:
1. Ask which role/company to simulate
2. Start with easy warm-up questions ("Tell me about yourself")
3. Progress to role-specific technical questions
4. Include 1-2 behavioral questions using the competencies from the job posting
5. End with a tough question or curveball
6. After each answer, give brief feedback: what worked, what to sharpen
7. Suggest which STAR example would work best for each question
