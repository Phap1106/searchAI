# RAG, LangChain/Redis Stack Reference and Domain Reading List

This document is a concept map and reading guide, not runtime configuration. APIs, product names, and compatibility requirements change; verify all version-sensitive details against current upstream documentation before implementation.

## Two Retrieval Paths — Keep Them Distinct

| Path | Description |
|---|---|
| **Document RAG** | Ingest a known corpus offline; preserve source metadata; index chunks; retrieve relevant passages at query time; ground the answer in those passages. |
| **Live web research** | Discover and fetch current pages at question time; capture provenance (URL, title, access date); cite fetched evidence. Search snippets alone are not sufficient evidence. |

One system may use both paths. A static RAG index does not contain current internet information unless it was refreshed and its freshness is known.

## RAG Concept Map

| Stage | What happens | Key design decisions |
|---|---|---|
| **Ingestion** | Load files or pages; normalize and deduplicate; preserve original source metadata. | Loader choice, deduplication key, metadata fields to retain. |
| **Chunking** | Split content for retrieval without losing headings, page numbers, URLs, or offsets needed for citations. | Chunk size, overlap, splitting strategy, boundary preservation. |
| **Indexing** | Embed chunks; store searchable text, vectors, and metadata in the chosen store. | Embedding model, index schema, metadata filters. |
| **Retrieval** | Select candidate chunks using semantic, lexical, filtered, or hybrid search. | Query mode, k, score threshold, reranking. Validate ranking on a domain-specific evaluation set. |
| **Generation** | Answer from retrieved evidence; expose source references; state insufficient evidence rather than filling gaps from memory. | Prompt structure, citation format, abstention signal. |
| **Evaluation** | Test retrieval relevance separately from answer correctness, citation coverage, and abstention rate. | Eval dataset, retrieval metrics (recall@k, MRR), answer metrics (citation precision, abstention precision). |

## Stack Roles

| Component | Role | When to add |
|---|---|---|
| **LangChain** | Integrations and abstractions for models, document loaders, text splitters, embeddings, vector stores, and retrievers. | Start here for most RAG workflows. |
| **LangGraph** | Explicit stateful control flow: branching, loops, checkpoints, retry, and human-in-the-loop. | Add when a linear retrieval-and-answer chain is insufficient. |
| **Redis / RedisVL** | Storage and search for vectors, text, and metadata. Supports vector, text, and hybrid queries (version-dependent). | Add when persistence, hybrid retrieval, or high-throughput is needed. Verify Redis and RedisVL versions before choosing query modes. |

Keep the initial design minimal. Add hybrid retrieval, reranking, graph workflows, or persistent state only when measured evaluation results justify them.

## Technical Reading List

- LangChain RAG: https://python.langchain.com/docs/tutorials/rag/
- LangChain retrieval: https://python.langchain.com/docs/concepts/retrieval/
- LangChain text splitters: https://python.langchain.com/docs/concepts/text_splitters/
- LangGraph overview: https://langchain-ai.github.io/langgraph/
- LangGraph persistence: https://langchain-ai.github.io/langgraph/concepts/persistence/
- Redis vector search: https://redis.io/docs/latest/develop/ai/search-and-query/vectors/
- RedisVL documentation: https://docs.redisvl.com/en/latest/
- RedisVL LangChain integration: https://docs.redisvl.com/en/latest/integrations/langchain.html
- LangSmith evaluation: https://docs.smith.langchain.com/evaluation
- Agent Skills specification: https://agentskills.io/specification

Vendored snapshots in `third_party/` are reference material only; see `docs/third-party-skills.md` for commit, license, and gap notes.

## Domain Topic Guides

Load only the one guide that matches the current task. Do not load all guides into the same context.

| Domain | Topic reference file |
|---|---|
| Sales, customers, funnel, revenue | `.agents/skills/domain-research/references/sales.md` |
| Journalism, verification, fact-checking | `.agents/skills/domain-research/references/journalism.md` |
| Landing pages, conversion copy, UX claims | `.agents/skills/domain-research/references/landing-page.md` |
| AI integration, risk, evaluation, deployment | `.agents/skills/domain-research/references/ai-integration.md` |
| Education, pedagogy, learning research | `.agents/skills/domain-research/references/education.md` |
| History, primary sources, interpretation | `.agents/skills/domain-research/references/history.md` |
| Accounting, standards, tax, financial reporting | `.agents/skills/domain-research/references/accounting.md` |
| Business, markets, competitors, strategy | `.agents/skills/domain-research/references/business.md` |
| Travel destinations, visa, safety, services | `.agents/skills/domain-research/references/travel.md` |

Topic guides are research frameworks and prompt checklists. They do not replace jurisdiction-specific law, professional advice, or primary data from authoritative bodies.

## Design Questions Before Implementation

Answer these before choosing components or writing code.

- What is the authoritative corpus, and how often must it refresh?
- Which source fields must appear in answer citations?
- What retrieval misses and abstention behaviors are acceptable?
- What domain-specific evaluation dataset will be used to compare lexical, vector, and hybrid retrieval?
- Which exact Redis, RedisVL, LangChain, and LangGraph versions does the contest environment allow?
