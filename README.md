# Awesome Forward Deployed Engineer [![Awesome](https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of resources for becoming — and thriving as — a **Forward Deployed Engineer (FDE)**: the customer-facing software engineer who ships production code *inside* a client's environment and owns the outcome end-to-end.

The role pioneered by Palantir is now the fastest-growing job in AI. Forward Deployed Engineer postings grew **729% year-over-year** (Apr 2025 → Apr 2026), and mid-to-senior total comp runs **$350K–$550K**. OpenAI stood up a dedicated FDE business; Anthropic launched a $1.5B JV to embed Claude FDEs in financial services. This list collects the best material to understand the role, build the skills, and land the job.

## Contents

- [What Is an FDE](#what-is-an-fde)
- [Why It Matters](#why-it-matters)
- [Companies Hiring FDEs](#companies-hiring-fdes)
- [Core Skills](#core-skills)
- [Agent Frameworks & SDKs](#agent-frameworks--sdks)
- [Evals & Observability](#evals--observability)
- [Deployment & Integration](#deployment--integration)
- [Interview Prep](#interview-prep)
- [Learn & Practice](#learn--practice)
- [Jobs & Salary Data](#jobs--salary-data)
- [Newsletters & Communities](#newsletters--communities)
- [Contributing](#contributing)

## What Is an FDE

- [Forward Deployed Engineer — Wikipedia](https://en.wikipedia.org/wiki/Forward_Deployed_Engineer) — Neutral, well-sourced primer on the role and its history.
- [Forward Deployed Engineers, and why they're in demand — The Pragmatic Engineer](https://newsletter.pragmaticengineer.com/p/forward-deployed-engineers) — Gergely Orosz on what FDEs actually do and why the model works.
- [So You Want to Hire a Forward Deployed Engineer — First Round Review](https://review.firstround.com/so-you-want-to-hire-a-forward-deployed-engineer/) — The hiring-manager view; reveals what the role is really evaluated on.
- [Why OpenAI and Anthropic are hiring FDE teams — The New Stack](https://thenewstack.io/forward-deployed-engineers-ai/) — How frontier labs adapted the Palantir model for AI deployment.
- [Understanding Palantir: Forward-Deployed Engineers — Medium](https://medium.com/@balajibal/understanding-palantir-forward-deployed-engineers-and-the-making-of-an-unusual-platform-company-494dc7812f24) — The origin story and the "Delta" program that built Foundry.
- [The Complete Guide to the FDE Role — Netguru](https://www.netguru.com/blog/forward-deployed-engineer-role-guide) — End-to-end overview of responsibilities and day-to-day.

## Why It Matters

- [Forward Deployed Engineer: Role, Skills & Meaning (2026) — JADA Squad](https://www.jadasquad.com/blog/forward-deployed-engineer) — Current market framing and skill breakdown.
- [The FDE Boom: 224 Open Roles Across 39 AI Companies — Jobs by Culture](https://jobsbyculture.com/blog/forward-deployed-engineer-boom-2026) — Snapshot of live demand across the market.
- [What Is a Forward Deployed Engineer — MarkTechPost](https://www.marktechpost.com/2026/05/20/what-is-a-forward-deployed-engineer-the-ai-role-openai-anthropic-and-google-are-hiring-in-2026/) — Why OpenAI, Anthropic, and Google are all hiring it.

## Companies Hiring FDEs

- [Palantir — Forward Deployed Software Engineer](https://jobs.lever.co/palantir) — Where the role was invented; still the reference implementation.
- [OpenAI FDE role breakdown — Paraform](https://www.paraform.com/blog/openai-forward-deployed-engineer) — Skills, scope, and comp for OpenAI's "Deployment Company."
- Also actively hiring FDE-style roles: **Anthropic**, **Databricks**, **Ramp**, **Stripe**, **Salesforce**, **Scale AI**, **Google Cloud**, and hundreds of AI-native startups.

## Core Skills

An FDE is a full-stack engineer who is also comfortable in front of the customer. The skills that separate FDEs from both SWEs and solutions engineers:

- **Production coding in unfamiliar environments** — you ship into the client's stack, not a demo sandbox.
- **Applied LLM / agent engineering** — prompt design, tool use, retrieval, and agent orchestration against real data.
- **Evaluation & reliability** — proving a system works before it touches operational decisions.
- **Systems integration** — auth, data pipelines, APIs, and legacy systems.
- **Customer discovery & outcome ownership** — translating a vague business problem into a shipped, measurable result.

## Agent Frameworks & SDKs

Tools FDEs reach for when building agentic systems in customer environments:

- [OpenAI Agents SDK](https://platform.openai.com/docs/guides/agents) — Official OpenAI framework for building agentic apps.
- [Anthropic Claude — Building Agents](https://docs.anthropic.com/en/docs/build-with-claude/agents) — Patterns and the Model Context Protocol (MCP).
- [LangChain](https://www.langchain.com/) & [LangGraph](https://www.langchain.com/langgraph) — Composable chains and stateful agent graphs.
- [LlamaIndex](https://www.llamaindex.ai/) — Data framework for retrieval-augmented and agentic apps.
- [CrewAI](https://www.crewai.com/) — Role-based multi-agent orchestration.
- [Microsoft AutoGen](https://microsoft.github.io/autogen/) — Multi-agent conversation framework.
- [DSPy](https://dspy.ai/) — Programming (not prompting) language models.
- [fde-framework](https://github.com/atulkapoor/fde-framework) — Engagement framework built for the FDE workflow itself: a client brief becomes typed facts, seven gates refuse the build until data access is verified and a baseline exists, and the emitted project ships evals, runbooks and a risk doc the client can read.

## Evals & Observability

You can't own an outcome you can't measure. Core tooling:

- [LangSmith](https://www.langchain.com/langsmith) — Tracing, evals, and monitoring for LLM apps.
- [Langfuse](https://langfuse.com/) — Open-source LLM observability and evals.
- [Braintrust](https://www.braintrust.dev/) — Eval-driven development for AI products.
- [Arize Phoenix](https://phoenix.arize.com/) — Open-source LLM tracing and evaluation.
- [Ragas](https://docs.ragas.io/) — Metrics for retrieval-augmented generation.

## Deployment & Integration

- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) — Open standard for connecting models to tools and data.
- [Vercel AI SDK](https://sdk.vercel.ai/) — Framework for building AI-powered product surfaces.
- [Temporal](https://temporal.io/) — Durable execution for long-running, reliable agent workflows.

## Interview Prep

- [FDE role & interview signal — Paraform](https://www.paraform.com/blog/forward-deployed-engineer-palantir-runway-greptile) — What Palantir, Runway, and Greptile look for.
- [First Round: how FDEs are evaluated](https://review.firstround.com/so-you-want-to-hire-a-forward-deployed-engineer/) — Read the hiring bar from the buyer's side.
- Practice loop: take a real dataset, build an agent that produces a business outcome, then write the eval that proves it. That artifact *is* the interview.

## Learn & Practice

Structured ways to build FDE skills, from free to institutional:

- [A10X](https://a10x.dev/) — Always-current FDE curriculum that tracks new agent frameworks, eval methods, and deployment patterns as the field shifts, plus a **free hands-on [Arena](https://a10x.dev/arena)** to practice deployment and evaluation drills. Self-serve, built for the individual engineer.
- [fde.academy (Futurense × IIT Roorkee)](https://fde.academy/) — Institutional PGP cohort program.
- [Building agents — Anthropic docs](https://docs.anthropic.com/en/docs/build-with-claude/agents) — Free, authoritative, hands-on.
- [DeepLearning.AI short courses](https://www.deeplearning.ai/short-courses/) — Free/low-cost applied LLM and agent courses.

## Jobs & Salary Data

- [FDE Pulse](https://fdepulse.com/) — Live FDE job board and salary data.
- [Palantir careers](https://jobs.lever.co/palantir) — Source-of-truth FDE and FDSE listings.
- [Paraform — FDE hiring & comp benchmarks](https://www.paraform.com/blog/forward-deployed-ai-engineer) — Market comp ranges by level.

## Newsletters & Communities

- [The Pragmatic Engineer](https://newsletter.pragmaticengineer.com/) — Regular coverage of the FDE role and market.
- [The New Stack](https://thenewstack.io/) — Ongoing reporting on AI deployment engineering.

## Contributing

Contributions welcome. Open a PR to add a resource — keep entries high-signal, vendor-neutral in framing, and with a one-line description of *why* it's worth an FDE's time. Low-quality or purely promotional links will be declined.

---

*Maintained by the team at [A10X](https://a10x.dev/) — making the AI Forward Deployed Engineer role learnable, and keeping it learnable as the field shifts. This list is vendor-neutral; A10X is listed once alongside real alternatives.*
