# Sandeep Barhanpure

I build platforms that let other people build, and I ship AI before it's obvious.

16 years across Fortune 1 retail, hyperscale cloud, and healthcare — product and engineering, never one without the other. I run organizations. I still write code. Leaders who stop building eventually stop knowing what questions to ask.

---

## The pattern

The through-line isn't a domain. It's a pattern: find the under-leveraged opportunity, build the system or product to capture it, make it the standard.

At RBL Bank, I built pricing and risk frameworks from scratch that became the operating standard across the institution. At MTM Health, I spotted whitespace in client analytics, built the company's first commercial SaaS product end-to-end, set the pricing, closed the clients, and owned the P&L. At AWS, I saw the case for applying GenAI to contract automation in early 2022 — months before it was on the company roadmap — assembled the team, pitched leadership, and shipped it. At Walmart, I'm running a builder platform that cuts program onboarding from months to weeks and standing up a greenfield business line where no requirements, no team, and no code existed when I started.

Different industries. Same approach.

---

## Now — Walmart Health & Benefits Technology

Director, Software Engineering. Two portfolios, one organization.

**Builder platform.** A low/no-code self-serve platform that lets business and engineering teams ship benefit programs without queuing behind a central team. The shift is *who* can build, not just how fast. First milestone shipped Q1 2025. Onboarding cut from roughly six months to under four weeks.

**Greenfield business line.** The most undefined initiative in the division — a new capability in a highly regulated space with no existing requirements, no internal expertise, no prior code. I deconstructed the value chain from zero, wrote the strategy, built the financial model from first principles, and secured executive sponsorship. Details under NDA.

Both portfolios share data, governance, and coordinated roadmaps. The org design reflects that — two teams executing independently on two strategic bets without contention.

---

## Before that

**AWS — Engineering & Analytics (2021–2024)**

Ran a 50-person engineering organization across two portfolios: the contract management platform behind a large share of AWS commercial revenue, and the customer analytics and demand planning system used by sales leadership across the company.

Shipped GenAI-powered contract automation in early 2022 — before it was on anyone else's roadmap. Consolidated five-plus enterprise systems into one platform. Cut 80% of operational overhead. Built the demand planning platform that gave sales leadership real-time pipeline visibility and lifted deal velocity by 25%.

Amazon Bar Raiser (BRIT).

**MTM Health — Engineering & Analytics (2015–2021)**

First data and analytics hire. Zero team, zero platform, no product. I left with a 30-person engineering organization, the company's first commercial SaaS product (built, priced, sold, and operated by me), and AI/ML systems running across tens of millions of records annually.

The real-time dispatching platform I built dropped missed trips from 9% to under 3% and lifted member satisfaction from 70% to over 85%. Those weren't vanity metrics — they tied directly to HEDIS access measures and Medicaid/Medicare contract retention.

I identified whitespace in client analytics, built the business case, launched the product, and closed state Medicaid agencies and managed care organizations as paying clients. 95% client satisfaction. First commercial product the company ever launched.

**RBL Bank — Pricing & Operations (2010–2013)**

Built pricing, reporting, and risk frameworks for consumer and commercial financial products from scratch. They became the operating standard across the institution. This is where I learned to think in systems and work from first principles, before I knew what those phrases meant.

---

## How I operate

**Find the opportunity nobody is working on.** At AWS in early 2022, everyone was doing traditional ML. GenAI for contract automation was sitting there unclaimed. At MTM, nobody had thought of selling the analytics capability as a product. The pattern: watch what the business needs and what the org is ignoring, then move fast.

**Write the product narrative before the spec.** If you can't explain in one paragraph who the user is, what hurts today, and how this changes their day — the work isn't ready. Most failed projects I've seen failed at this step, then tried to fix it with engineering.

**Build the smallest thing that proves the thesis.** Not MVP in the bloated sense — the actual minimum that tells you whether you're right. If it takes more than a few weeks, the question is too big.

**Architecture is a series of bets about what won't change.** Pick those bets carefully. Everything else should be cheap to throw away. Most over-engineering comes from treating reversible decisions as irreversible.

**Throughput beats control, until it doesn't.** Central teams that block product teams in the name of standards usually create more risk than they prevent — the work routes around them anyway. Standards should be paved roads, not toll booths.

**Hire for taste and slope.** An engineer who has shipped one real thing end-to-end is worth more than someone who has held the title at five companies. 25+ people I've managed now run their own orgs.

---

## What I'm building

Real products. Where I keep my hands in the code and test ideas I can't run inside a large company.

### Member360 — the AI advocate for health plan members.

Most members get a denied claim and a code that means nothing. The real answer lives across an EDI 835 transaction, a denial code table, the plan design, and a provider billing record — four systems, four teams, no shared view. Member360 reads the 835, maps the denial, checks plan rules, and tells the member in plain English what happened and what to do next. The reasoning is transparent — a non-engineer can read the transcript and verify it.

**First surface.** Denial Decoder — a free consumer tool at [`decoder.member360.ai`](https://decoder.member360.ai).

**Stack.** Python, LangChain, Streamlit (operator view), React (member view).

**Status.** Live consumer product. Commercial pricing model in development for payer and employer segments. The hard part isn't the agent loop — it's the data model that lets the agent answer without hallucinating policy.

### Fitness Intel — agentic AI for endurance coaching.

Serious endurance athletes already have more data than they can use. Strava tracks the training, Oura or Whoop tracks the recovery, Garmin tracks the ride, the weather app tracks the forecast — and none of them answer the question that actually matters at 5 AM: *what do I do today, and why?*

Fitness Intel is a coach in your pocket. Specialized agents reason across training load (TSS, CTL, ATL, form), recovery state (HRV, resting HR, sleep), and the day ahead (weather, schedule, terrain) to produce one defensible recommendation — not a static plan, not generic coaching language. Every suggestion shows the signals behind it: *"Z2 for 90 minutes today. CTL is climbing, HRV dropped 12% overnight, and you have intervals scheduled Thursday. Save the load."*

Built for amateurs who already live in TrainingPeaks or intervals.icu and want a coach that integrates the data instead of ignoring it. Interface is Telegram — because that's where you are at 5 AM, not a dashboard.

**Stack.** TypeScript, Supabase (Postgres + pgvector), agent orchestration, Telegram bot, scheduled syncs on cron.

**Status.** Multi-tenant, invite-only while the reasoning layer matures. Generic advice backed by personal data is still generic advice — I'd rather it stay narrow and correct.

### Cadence — the AI operations layer for short-term rental hosts.

STR operators run on duct tape: pricing tools, channel managers, cleaning schedulers, guest comms — different tabs, different logins, no shared brain. Cadence sits on top: an AI assistant that triages messages, flags revenue issues, and handles the recurring decisions that don't need a human. The real question isn't what AI *can* do — it's which workflows actually compress with AI versus which ones just look like they should.

**Status.** Early. More when there's something to show.

---

## Tech I work with

**Languages & Frameworks.** Python · TypeScript · React · Node.js · Streamlit

**AI / LLM.** Claude API · OpenAI API · LangChain · RAG · Vector databases (pgvector, Pinecone) · MCP · Prompt engineering and evals · SageMaker · Bedrock

**Data & Integration.** PostgreSQL · Supabase · Snowflake · Kafka · Spark · REST · ETL and event pipelines

**Cloud & DevOps.** AWS · Azure · GCP · Docker · Kubernetes · Terraform · GitHub Actions · CI/CD

**Domain.** Healthcare EDI (835/837) · HIPAA · FHIR/CMS · Pharmacy benefits · Enterprise SaaS · Financial products and pricing · Endurance training science (TSS / CTL / ATL / HRV)

---

## Contact

[LinkedIn](https://www.linkedin.com/in/sandeepbarhanpure)
