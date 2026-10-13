# Hi, I'm Vinicius Cavalcante

AI Engineer with 5 years of experience shipping production LLM systems and the backends around them, in **Python and TypeScript**. Based in Manaus, Brazil, working remotely in English and Portuguese.

I build **agentic systems that can be trusted in production**: multi-provider LLM layers, retrieval, evaluation harnesses and LLM judges. Underneath them sit event-driven services, queues, billing and data pipelines. I also build the harnesses I develop with. A Claude Code orchestrator directs parallel Codex agents in isolated worktrees, and every change has to clear guardrails enforced by tooling, not by prompts.

Most AI failures I find aren't bad model output. They're green gates that never looked.

## Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

* **AI & LLMs:** LangGraph, LangChain, multi-provider LLM layers (Anthropic, OpenAI, Gemini) with retries and structured-output fallback, ReAct agents and tool use, RAG on MongoDB Atlas Vector Search, embedding and reranking evals, LLM-as-judge, Langfuse, LangSmith
* **Agentic engineering:** Claude Code, Codex and Cursor; multi-agent orchestration, hooks and side-effect guards, worktree isolation, spec-driven development, reviewing AI-generated code
* **Backend:** Python (FastAPI, Pydantic, asyncio, Temporal, Luigi), TypeScript (NestJS, Fastify), REST APIs, webhooks, SQS consumers with retries and DLQs, Stripe billing, n8n
* **Data:** MongoDB, PostgreSQL, ClickHouse, Redis, DynamoDB, SQLite
* **Platform:** AWS (ECS, Lambda, SQS, SNS, S3, DynamoDB), Terraform and Terragrunt, Docker, GitHub Actions, Heroku, Datadog
* **Frontend & testing:** React, Tailwind, MUI, pytest, Jest, Playwright, mutation testing (mutmut, Stryker)

## Experience

### Founder & Principal AI Engineer | Lateralus AI Lab (2026 to present)
* Built a multi-agent development harness. A Claude Code orchestrator plans and reviews while parallel Codex agents implement, each in its own git worktree. Hooks and side-effect guards enforce the rules, and every issue passes about 22 automated gates. The harness itself is covered by roughly 1,000 tests.
* Ships evidence-first LLM products: website-to-company verification with independent agent labelers and a judge, and a multi-provider eval suite comparing local and frontier models.

### Founding AI Engineer & Technical Lead | AlphaSearch (June 2025 to present)
* Owns the platform end to end: a FastAPI/MongoDB backend, a React frontend, and Luigi ETL pipelines over a corpus of roughly 10M companies. Previously led a team of 3 developers.
* Built a Playwright data-acquisition pipeline that collected 200,000+ company profiles across 7,000+ targeted queries.
* Built a conversational discovery agent and a ReAct enrichment agent on a multi-provider LLM layer, with Langfuse tracing and Atlas Vector Search.
* Built retrieval evals (Voyage, Cohere and BGE embeddings and rerankers) and an LLM judge for lead quality. A $0.70 eval run against a real population caught a regression that halved named leads.
* Designed the LLM-as-judge contract behind lead verification. Each verdict needs verbatim evidence, validated as shared NFKC quotes. Failures are isolated per candidate, and an independent audit judge checks the results.
* Implemented Stripe billing: a transactional credit ledger, signature-verified webhooks and a background event processor. Mutation testing and dedicated CI jobs guard the money paths.
* Hardened CI against gates that pass without looking. A test-reachability check fails when a test file runs in no job, and mutation-score ratchets cover the credit and billing paths.

### Software Engineer | SIDIA - Samsung R&D (2021 to 2025)
* Designed and optimized FastAPI REST APIs serving 500+ daily users.
* Cut legacy process execution times by 30% through SQL tuning and code optimization.
* Built Jenkins and Docker CI/CD pipelines, cutting deployment times by 40%.
* Raised unit and integration test coverage to 80% across all applications.

## Open source

* [**lateralus-pramana**](https://github.com/vinipy12/lateralus-pramana): evidence-based company website verification. Deterministic evidence collection, three independent agent labelers and a judge, and a transactional SQLite store.
* [**lateralus-story-finder**](https://github.com/vinipy12/lateralus-story-finder): a Telegram bot that writes weekly Reddit briefs in Brazilian Portuguese, with a multi-provider eval suite (Anthropic, OpenAI, Codex, Ollama), a scoring rubric and LLM-judge reports.

## What I'm working on

- Making agent verification loops trustworthy enough to lean on. The bottleneck is proving that a gate covers the code it claims to guard, not model capability.
- Calibrated LLM judges: evidence contracts, legitimate abstention, and measuring whether "high confidence" means anything.
- Retrieval quality beyond recall: precision on weak slices, and canonicalizing free text before it becomes a filter.

## Reach me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vinicius-cavalcante-827565140/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vinicius.loureiro.cavalcante12@gmail.com)
