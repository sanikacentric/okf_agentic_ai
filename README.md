# Production Agentic AI: OKF + Hybrid RAG + Governed Context

A production-oriented reference architecture demonstrating that **OKF/direct knowledge navigation and RAG are complementary**.

### Architecture

`User → Supervisor Agent → Policy/Intent Guard → Knowledge Strategy Agent → {OKF Navigator | Hybrid Retriever | SQL/API Tool} → Context Engineer → Answer Agent → Critic/Grounding Agent → Response + Provenance`

### Production concerns included

- Multi-agent orchestration with explicit state
- Structured OKF-style Markdown/YAML knowledge
- Direct navigation for curated knowledge
- Lexical + semantic-style + hybrid retrieval
- RBAC / classification enforcement **before context reaches the model**
- Tool registry and bounded tool execution
- Provenance and citations
- Context budgeting
- Grounding/critic gate
- Telemetry and trace IDs
- Retry/error boundaries
- Evaluation and security regression tests
- Optional OpenAI-compatible LLM adapter (core demo runs locally without API keys)

> This notebook deliberately separates **knowledge representation**, **retrieval**, **reasoning**, and **governance**.
