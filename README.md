### Hi, I'm Wahiduzzaman 👋

Applied AI engineer in Dhaka. I build LLM systems that people rely on at work: document extraction that writes into live Excel models, tool-calling agents across 40+ services, and hybrid retrieval.

**What I focus on**
- 📏 **Measuring quality:** labelled test sets, field-level accuracy, and blocking changes that make results worse
- 🔎 **Grounded outputs:** every extracted value must point to the evidence it came from
- 🛡️ **Agents with guardrails:** what an agent may do is enforced in code, not asked for in a prompt
- ⚡ **Cost and latency:** rules first, model only where needed

**Featured**
- [`governed-agents`](https://github.com/wshuv-o/governed-agents): a platform for internal AI agents you can trust with real systems: durable Postgres queue with resumable runs, **tool grants by risk tier enforced in code**, human approval with all-or-nothing rollback, a full audit log, and a golden eval suite (prompt injection, invented progress, private-data leaks) that gates CI; includes Terraform for **Google Cloud** (Cloud Run, Cloud SQL, keyless GitHub deploys)
- [`code-search`](https://github.com/wshuv-o/code-search): retrieval for code with an eval that decides what's kept: AST chunking, BM25 and local embeddings compared on 110 labelled queries, measured on whether the right code fits a model's context budget (hybrid 71%, whole files 2%); no paid APIs
- [`llm-gateway`](https://github.com/wshuv-o/llm-gateway): an OpenAI-compatible LLM gateway in **Go** (standard library only): failover routing across OpenAI-compatible and Anthropic providers, circuit breakers, per-key auth, rate limits and token budgets, a per-tenant cache that collapses duplicate requests, streaming with a safe failover point, Prometheus metrics and an audit log
- [`doc-extraction-evals`](https://github.com/wshuv-o/doc-extraction-evals): evaluation harness for LLM document extraction (labelled PDFs, grounded extractors, CI gate), exposed to agents as a read-only **MCP server**, with **OpenTelemetry** tracing of tokens and latency, and packaged as a secured API for **Kubernetes (AWS EKS)** with Terraform, NetworkPolicy, image scanning and keyless GitHub OIDC deploys

**Stack:** Python · Go · TypeScript · FastAPI · LangChain · OpenAI / Anthropic / Gemini · Qdrant · PostgreSQL · Redis · Docker · GitHub Actions

📫 [LinkedIn](https://linkedin.com/in/wahid-shuvo) · [Portfolio](https://wshuv-o.github.io) · Open to remote applied AI roles

