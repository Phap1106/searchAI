---
name: rag-docs
description: Explain, research, or document RAG systems and the LangChain, LangGraph, Redis, and RedisVL stack using current official references. Use for architecture guidance, component comparison, retrieval design, or stack documentation. Do not use for general internet research — use web-research instead.
---

# RAG and Stack Documentation Skill

Concept map and reading list: `../../../docs/rag-langchain-redis.md`
LangChain RAG patterns reference (vendored snapshot, not current API authority): `../../../third_party/langchain-skills/langchain-rag/SKILL.md`
Consulting report framework reference (vendored snapshot): `../../../third_party/deer-flow/consulting-analysis/SKILL.md`

## Workflow

1. **Classify the question.** Determine whether it concerns a general RAG concept, a LangChain/LangGraph API, Redis/RedisVL behavior, evaluation design, or contest-specific configuration.
2. **Check upstream docs for version-sensitive details.** Do not rely on model memory or vendored snapshots as the current API surface. Use the reading list in `../../../docs/rag-langchain-redis.md`.
3. **Separate the pipeline stages.** Distinguish ingestion/chunking/indexing (offline) from retrieval and generation (query-time). Explain what data is indexed, how it is retrieved, and how the answer is grounded.
4. **Distinguish document RAG from live web search.** A vector index is not a substitute for current web retrieval; clarify which path applies and whether both are needed.
5. **Recommend the minimal architecture.** Start with the simplest design that meets stated requirements. Add hybrid retrieval, reranking, LangGraph, or persistent state only when evaluation results support them.
6. **Include provenance and failure behavior.** Any proposed RAG design must address: source metadata preserved in chunks, citation format in answers, evaluation plan, and abstention signal when evidence is insufficient.
7. **Do not configure the stack.** Do not select a model, API provider, embedding model, or vector store unless the repository owner provides explicit requirements and contest constraints.

## Output Checks

- Cite upstream official docs for every version-sensitive technical claim.
- Explicitly label assumptions and unresolved compatibility questions.
- Do not present archived repositories or tutorials as current API references.
- Do not inherit provider defaults, model names, or API signatures from the vendored snapshots.
