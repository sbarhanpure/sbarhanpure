# Sandeep Barhanpure

I build platforms that let other people build, and I ship AI before it's obvious. 16 years across Fortune 1 retail, hyperscale cloud, and healthcare services — always on both the product side and the engineering side at the same time.

I run engineering organizations and I still write code. Leaders who stop building stop knowing what questions to ask.

---

## The pattern

The through-line across my career isn't a domain. It's a pattern: find the under-leveraged opportunity, build the system or product to capture it, make it the standard.

At RBL Bank, I built pricing and risk frameworks from scratch that became institutional standards. At MTM Health, I spotted a whitespace in client analytics, built the company's first commercial SaaS product from zero, set the pricing, closed the clients, and owned the P&L. At AWS, I saw the case for applying GenAI to contract processing in early 2022 — months before it was on the company roadmap — assembled the team, pitched leadership, and shipped it. At Walmart, I'm running a builder platform that cuts program onboarding from months to weeks and building a greenfield business line where no requirements, no team, and no code existed when I started.

The domain changes. The approach doesn't.

---

## Now — Walmart Health & Benefits Technology

Director, Software Engineering. Two portfolios, one organization.

**Builder platform.** A low/no-code self-serve platform that lets business and engineering teams ship benefit programs without queuing behind a central team. The goal: shift *who* can build on the platform, not just how fast. First milestone shipped Q1 2025. Onboarding time cut from ~6 months to under 4 weeks.

**Greenfield business line.** Took on the most undefined initiative in the division — a new capability in a highly regulated space with no existing requirements, no internal expertise, and no prior code. Deconstructed the value chain from zero, wrote the strategy, built the financial model from first principles, secured executive sponsorship. Details under NDA.

Both portfolios share data, governance, and coordinated roadmaps. The org design reflects that — two teams executing independently on two strategic bets without contention.

---

## Before that

**AWS — Engineering & Analytics (2021–2024)**

50-person engineering org. Two portfolios: the contract management platform behind a large share of AWS commercial revenue, and the customer analytics and demand planning system used by sales leadership across the company.

Shipped GenAI-powered contract automation in early 2022 — before it was on anyone's roadmap. Consolidated five-plus enterprise systems into one platform, cut 80% of operational overhead, and built the demand planning platform that gave sales leadership real-time pipeline visibility and accelerated deal velocity by 25%.

Amazon Bar Raiser (BRIT).

**MTM Health — Engineering & Analytics (2015–2021)**

First data and analytics hire. Zero team, zero platform, no product. Left with a 30-person engineering org, the company's first commercial SaaS product (built, priced, sold, and operated by me), and AI/ML systems running across tens of millions of records annually.

Built a real-time intelligent dispatching platform: missed trips dropped from 9% to under 3%, member satisfaction went from 70% to over 85%. Those aren't vanity metrics — they tied directly to HEDIS access measures and Medicaid/Medicare contract retention.

Identified the whitespace in client analytics, built the business case, launched the product, and closed state Medicaid agencies and managed care organizations as paying clients. 95% client satisfaction. First commercial product the company ever launched.

**RBL Bank — Pricing & Operations (2010–2013)**

Built pricing, reporting, and risk frameworks for consumer and commercial financial products from scratch. Became the operating standard across the institution. This is where I learned to think in systems and work from first principles before I knew what those phrases meant.

---

## How I operate

**Find the opportunity nobody is working on.** At AWS in early 2022, everyone was doing traditional ML. GenAI for contract automation was sitting there unclaimed. At MTM, nobody had thought about selling the analytics capability as a product. The pattern: look at what the business needs and what the org is ignoring, then move fast.

**Write the product narrative before the spec.** If you can't explain in one paragraph who the user is, what hurts today, and how this changes their day — the work isn't ready. Most failed projects I've seen failed at this step, then tried to fix it with engineering.

**Build the smallest thing that proves the thesis.** Not MVP in the bloated sense — the actual minimum that answers whether you're right. If it takes more than a few weeks, the question is too big.

**Architecture is a series of bets about what won't change.** Pick those bets carefully. Everything else should be cheap to throw away. Most over-engineering comes from treating reversible decisions as irreversible.

**Throughput beats control, until it doesn't.** Central teams that block product teams in the name of standards usually create more risk than they prevent — the work routes around them anyway. Standards should be paved roads, not toll booths.

**Hire for taste and slope.** An engineer who has shipped one real thing end-to-end is worth more than someone who has held the title at five companies. 25+ people I've managed now run their own orgs.

---

## What I'm building

Side projects. Where I keep my hands in the code and test ideas I can't run inside a large company.

### member-360-agentic-experience-layer

**Problem.** A member gets a denied claim. The actual answer — why it was denied, what to do next — lives in an EDI transaction, a denial code table, the plan design, and a provider billing record. Four systems, four teams, no shared view. The member gets a code that means nothing and a phone tree that leads nowhere.

**Approach.** Agents that reason over claims data instead of scripted bot flows. The agent reads the 835, maps the denial to a plain-English explanation, checks plan rules, and tells the member what to do next. Built so a non-engineer can read the transcript and verify the reasoning.

**Stack.** Python, LangChain, Streamlit (operator view), React (member view).

**Status.** Prototype. The hard part isn't the agent loop — it's the data model that lets the agent answer questions without hallucinating policy.

### fitness-intel

**Problem.** I ride bikes seriously. Training data in Strava, recovery in Oura, weather in Open-Meteo — none of it answers the question I actually want answered: *should I go hard today, and why?* Generic AI fitness advice ignores the data I already have.

**Approach.** Pull everything into one store. Ask in plain English over Telegram. Answers grounded in real numbers — power output, HRV, forecast — not generic coaching language.

**Stack.** TypeScript, Supabase (Postgres + pgvector), Telegram, scheduled syncs on cron.

**Status.** Private while I get the reasoning right. Generic advice backed by personal data is still generic advice — I'd rather it stay narrow and correct.

### cadence

AI assistant for short-term rental operators. Early stage. The real question is which workflows actually compress with AI versus which ones just look like they should. More when I know.

---

## Tech I work with

**Languages & Frameworks.** Python · TypeScript · React · Node.js · Streamlit

**AI / LLM.** Claude API · OpenAI API · LangChain · RAG · Vector databases (pgvector, Pinecone) · MCP · Prompt engineering and evals · SageMaker · Bedrock

**Data & Integration.** PostgreSQL · Supabase · Snowflake · Kafka · Spark · REST · ETL and event pipelines

**Cloud & DevOps.** AWS · Azure · GCP · Docker · Kubernetes · Terraform · GitHub Actions · CI/CD

**Domain.** Healthcare EDI (835/837) · HIPAA · FHIR/CMS · Pharmacy benefits · Enterprise SaaS · Financial products and pricing

---

## Contact

[LinkedIn](https://www.linkedin.com/in/sandeepbarhanpure)
