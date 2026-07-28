# 👋 Hi, I'm Vinicius Cavalcante

Staff AI Engineer with 5+ years building production AI systems — and, increasingly, the systems that keep them honest.

I work on **agent infrastructure and AI reliability**: multi-agent orchestration, LLM-as-judge contracts, evaluation harnesses with real spend controls, and the CI gates that catch a model's confident wrong answer before a customer does. Before that, and still: large-scale retrieval, RAG, and the full-stack work to ship it.

My current focus is the unglamorous half of applied AI — **proving a system does what it claims**. Most AI failures I find aren't bad model output; they're green gates that never looked.

## 💻 Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=FastAPI&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

---

* **Agent systems:** multi-agent orchestration, MCP servers, tool-use contracts, sandboxing and permission boundaries, worktree isolation, headless agent fleets
* **AI reliability:** LLM-as-judge design, evidence/citation contracts, eval harnesses, golden datasets, calibration, spend caps and cost accounting, mutation testing on money paths
* **Retrieval:** RAG at 5M+ documents, MongoDB Atlas Vector Search (HNSW), hybrid retrieval, recall/precision benchmarking, embedding quality gates
* **Backend:** Python, FastAPI, Django, Flask, MongoDB, PostgreSQL, Redis, async/concurrency, tenant isolation, idempotency and transactional correctness
* **Platform:** GitHub Actions, Docker, Heroku, AWS (EC2, SES, IAM), GCP, Jenkins, CI quality ratchets
* **Frontend:** JavaScript, React

## 🚀 Professional Experience

### Staff AI Engineer | AlphaSearch (Remote)
* Built the agent harness the team develops with: a Claude orchestrator directing parallel headless Codex implementer lanes, each isolated to its own git worktree, with guardrails enforced by tooling rather than prose — `PreToolUse` hooks, launcher sandbox refusals, and a one-command verification pass that re-derives every claim outside the agent's sandbox.
* Designed the LLM-as-judge contract behind lead verification: verbatim-evidence requirements with shared NFKC quote validation, per-candidate failure isolation, and an independent audit judge. Diagnosed and fixed a defect where the judge was marked malformed for *correctly rejecting* candidates, because the contract demanded a supporting quote for a negative verdict.
* Built a production readiness harness with hard spend caps, a no-spend preflight, frozen configuration snapshots keyed to an evaluated commit SHA, secret/PII redaction, and human adjudication records — so a launch decision rests on reproducible evidence instead of a green check.
* Hardened CI against gates that pass without looking: a test-reachability check that fails when any test file is executed by no job (it found auth and subscription integration tests running nowhere), plus mutation-score ratchets over credit and billing paths.
* Found and closed cross-tenant isolation defects in review, including account-private company records readable through an unscoped shared-collection query and leaking into a shared embedding index via semantic search.
* Architected and deployed the RAG system: 5M+ documents on MongoDB Atlas Vector Search (HNSW), sub-10-second retrieval, with Cohere embeddings/reranking and Gemini chat, on Heroku.
* Engineer and maintain the full-stack application — FastAPI backend, MongoDB, React frontend.

### Software Engineer | Sidia Instituto de Ciência e Tecnologia
* Designed and optimized RESTful APIs with FastAPI, serving 500+ daily users.
* Reduced legacy process execution times by 30% through SQL tuning and code optimization.
* Built and maintained CI/CD pipelines (Jenkins, Docker), cutting deployment times by 40%.
* Boosted unit and integration test coverage to 80% across all applications.

## 📊 GitHub Stats
![Your GitHub stats](https://github-readme-stats.vercel.app/api?username=vinipy12&show_icons=true&theme=radical)

## 🔥 Selected Work

### 🤝 Multi-Agent Development Harness
A version-controlled orchestration harness where a Claude orchestrator plans and reviews while parallel Codex lanes implement — one git worktree each, no shared state. Guardrails are enforced by tools, not documentation: hooks that block the orchestrator from writing application code, a launcher that refuses unsafe sandbox modes, and a verification script that runs the checks a sandboxed agent structurally cannot. Includes a conformance pass that answers the one question gates can't — *did the agent build what was actually asked?*

### 🧪 Evidence-Grade Evaluation Harness
A readiness gate for a paid, LLM-driven pipeline: mutually exclusive preflight and paid-run modes, per-case cost reservations against a hard cap, a frozen config snapshot bound to the evaluated SHA, redaction of credentials and PII, an independent audit judge, and adjudication records for human review. Designed so the honest outcome is often *"not ready"* — and so that verdict is reproducible.

### 🔍 RAG System for Large-Scale Document Retrieval
Retrieval-Augmented Generation over a 5M+ document MongoDB collection using LangChain, local Ollama models and cloud-hosted models, with Cohere embeddings/reranking and Gemini for chat. Optimized indexing and retrieval for low latency, deployed on Heroku.

### 🔄 CRM Backend System
A scalable Django backend with RESTful APIs deployed on AWS EC2 using Docker. Implemented AWS SES integration for notifications and secure IAM roles for access control.

### 🔬 COVID-19 Detection CNN
A convolutional neural network achieving 92% accuracy detecting COVID-19 from X-ray images, using Python, Keras and TensorFlow.

## 🌱 What I'm working on

- Making agent verification loops trustworthy enough to lean on — the bottleneck is proving a gate covers the code it claims to guard, not model capability
- Calibrated LLM judges: evidence contracts, legitimate abstention, and measuring whether "high confidence" means anything
- Retrieval quality beyond recall — precision on weak slices, and canonicalizing free text before it becomes a filter

## 📫 How to reach me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vinicius-cavalcante-827565140/)
