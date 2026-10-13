### Hi, I'm Vinicius 👋

Senior AI Engineer, based in Manaus, Brazil and working remotely in English and Portuguese. I build LLM systems that hold up in production, and the Python and TypeScript backends that ship them.

At **AlphaSearch**, I'm the founding AI engineer and technical lead of a B2B company-search SaaS. I own the FastAPI/MongoDB backend, the React frontend and ETL over roughly 10M companies. I also own the agents on a multi-provider LLM layer, the retrieval evals and LLM judge, and Stripe billing. At **Lateralus AI Lab** I consult and build my own tools.

Most AI failures I find aren't bad model output. They're green gates that never looked.

**Some results**
- An eval run that cost $0.70, against real data, caught a regression that halved the number of named leads.
- Built a Stripe credit ledger with signature-verified webhooks, guarded by mutation testing and dedicated CI jobs.
- Built an agent harness in which an orchestrator dispatches parallel Codex and Claude Code lanes in isolated worktrees. An independent critic reviews every change, and about 22 gates run per issue.

**Open source**
- [lateralus-workflow](https://github.com/vinipy12/lateralus-workflow): a fail-closed orchestration harness for coding agents, with push and merge guards, TDD receipts, quality gates and a failure library.
- [lateralus-pramana](https://github.com/vinipy12/lateralus-pramana): evidence-based company-domain verification, using blind multi-agent labeling and judge adjudication.
- [lateralus-bussola](https://github.com/vinipy12/lateralus-bussola): a weekly job radar over ATS feeds that writes grounded AI job cards, with a phone swipe-triage UI.
- [lateralus-story-finder](https://github.com/vinipy12/lateralus-story-finder): a Telegram bot that briefs Reddit threads in Portuguese, with a model-comparison eval harness. Work in progress.

**Stack:** Python (FastAPI, asyncio, Temporal) · TypeScript (NestJS, Fastify) · LangGraph · LangChain · RAG · MongoDB Atlas Vector Search · PostgreSQL · ClickHouse · AWS · Terraform · React

**Elsewhere:** [LinkedIn](https://www.linkedin.com/in/vinicius-cavalcante-827565140/) · vinicius.loureiro.cavalcante12@gmail.com
