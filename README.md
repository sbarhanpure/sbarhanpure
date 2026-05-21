# Sandeep Barhanpure

Product and engineering leader. 16 years building software in healthcare, retail, and cloud infrastructure — industries where the work actually matters to the person on the other end of it.

I run engineering organizations and I still write code. The two aren't separable. Leaders who stop building lose the ability to tell good work from bad.

---

## What I do now

I lead engineering at Walmart Health & Benefits Technology. Two portfolios on a platform that serves millions of members across the enterprise.

**Builder platform.** A set of services and primitives that lets product and engineering teams ship benefits experiences without queuing behind a central team. The thesis: most enterprise platforms slow teams down because they optimize for control instead of throughput. We optimize for throughput and add controls where they actually pay for themselves.

**New healthcare business line.** Built from zero — new domain, new team, no existing code, no existing customer. The first six months were almost entirely product work: figuring out who the user is, what they actually need, and what we refuse to build. The next six were engineering: getting the architecture right before scale punishes us for getting it wrong.

## Before this

**AWS — Contract Management & Analytics.** Built and ran a 50-person engineering org behind the contract management and analytics systems that supported a large share of AWS commercial revenue. Internal-facing, but if it broke, deals stopped moving and revenue recognition broke with them. The job taught me how to run engineering at a scale where every architectural decision compounds and every outage gets a postmortem with a VP in the room.

**MTM Health — Data Science & Analytics.** First data and analytics hire. Built the AI, data, and analytics systems that supported a multi-year stretch of significant revenue growth. Started with no team and a spreadsheet culture. Left with a data engineering org and decisions getting made off models instead of gut.

---

## How I operate

A few things I've learned the hard way and now treat as defaults.

**Write the product narrative before the code.** If you can't explain in one paragraph who the user is, what hurts today, and how this changes their day, the spec isn't ready. Most failed projects I've seen failed at this step and tried to fix it later with engineering.

**Build the smallest thing that proves the thesis.** Not an MVP in the bloated sense — the actual minimum that lets you learn whether you're right. If the prototype takes more than a few weeks, the question is too big.

**Architecture is a series of bets about what won't change.** Pick those bets carefully. Everything else should be cheap to throw away. Most over-engineering comes from treating reversible decisions as irreversible.

**Throughput beats control, until it doesn't.** Central teams that block product teams in the name of standards usually create more risk than they prevent — the work just routes around them. Standards should be paved roads, not toll booths.

**Hire for taste and slope, not the resume.** A senior engineer who has shipped one real thing end-to-end is worth three who've held the title at five companies.

**Healthcare is fragmented because the systems don't talk to each other.** Most of what patients experience as bureaucracy is actually an integration problem. The teams that fix that with software — not more process — will define the next decade.

---

## What I'm building

These are the side projects. They're where I keep my hands in the code and test ideas I can't run inside a large company.

### member-360-agentic-experience-layer

**Problem.** A health plan member gets a denied claim. The denial code means nothing to them. The phone tree means nothing either. The actual answer lives inside an 835 EDI transaction, a CARC/RARC code table, the member's plan design, and the provider's billing record — four systems, four teams, no shared view.

**Approach.** Agents that reason over claims data instead of scripted bot flows. The agent reads the 835, maps the denial to a plain-English explanation, checks plan rules, and tells the member what to do next. Built so a non-engineer can read a transcript and verify the reasoning.

**Stack.** Python, LangChain, Streamlit for the operator view, React for the member view.

**Status.** Prototype. The hard part isn't the agent loop — it's the data model that lets the agent answer questions without hallucinating policy.

### fitness-intel

**Problem.** I ride bikes seriously. My ride data lives in Strava, recovery in Oura, weather in Open-Meteo, and none of it answers the actual question: *should I go hard today, and why?* Generic AI fitness advice ignores the data I already have.

**Approach.** Pull everything into one store. Ask questions in plain English over Telegram. Answers are grounded in real numbers — last week's TSS, this morning's HRV, the wind forecast — not generic coaching language.

**Stack.** TypeScript, Supabase (Postgres + pgvector), Telegram bot interface, scheduled syncs on cron.

**Status.** Private while I get the reasoning layer right. Generic AI giving generic advice is worse than no advice — I'd rather it stay narrow and correct.

### cadence

An AI assistant for short-term rental operators. Early. The interesting question is which workflows actually compress with AI versus which ones just look like they should. More to share when I know.

### github-traffic-tracker

GitHub's traffic API drops data after 14 days. This archives it. Daily cron, JSON file archive, static dashboard, zero runtime dependencies. Small tool, built the way small tools should be built — no framework, no database, deploys in one file.

---

## Tech I work with

**Languages & Frameworks.** Python · TypeScript · React · Node.js · Streamlit

**AI / LLM.** Claude API · OpenAI API · LangChain · RAG · Vector databases (pgvector, Pinecone) · MCP · Prompt engineering and evals

**Data & Integration.** PostgreSQL · Supabase · Kafka · REST · Webhooks · ETL and event pipelines

**Cloud & DevOps.** AWS · Docker · Terraform · GitHub Actions · CI/CD

**Domain.** Healthcare EDI (835 / 837) · HIPAA · Pharmacy benefits (NCPDP D.0) · Claims adjudication · Property management and STR operations

---

## Contact

[LinkedIn](https://www.linkedin.com/in/sandeepbarhanpure)
