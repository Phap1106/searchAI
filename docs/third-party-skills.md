# Third-Party Skills: Provenance and Usage Notes

Vendored files under `third_party/` are read-only reference snapshots, not active instructions. Verify all technical claims against current upstream docs before using any content from these files. The organizer-provided rules screenshot says teams write prompts and direct BTC AI during the contest; whether prebuilt skills may be imported or used is unresolved. Obtain organizer approval before using these snapshots in contest work.

## langchain-ai/langchain-skills — langchain-rag

| Field | Value |
|---|---|
| Vendored file | `third_party/langchain-skills/langchain-rag/SKILL.md` |
| Source repo | https://github.com/langchain-ai/langchain-skills |
| License | MIT — Copyright (c) LangChain, Inc. |
| License file | `third_party/langchain-skills/LICENSE` |
| Pinned commit | `16a992f09ab3ccfb642dd4f08d350d833d1990bf` |
| Snapshot date | 2026-10-06 |
| Upstream status | Early development; content may change without notice. |

**Covers:** RAG pipeline patterns — document loaders, RecursiveCharacterTextSplitter, embeddings, vector stores (Chroma, FAISS, Pinecone), metadata filtering, MMR retrieval, and common chunking mistakes. Python and TypeScript examples.

**Gaps:** OpenAI and selected stores only — no Redis/RedisVL, no hybrid retrieval, no LangGraph, no evaluation or abstention patterns. Package versions reflect snapshot date; verify against current LangChain release notes before use.

**Safe use:** Pattern reference for pipeline structure and common pitfalls. Do not copy import statements or model names without verifying against current upstream docs.

---

## bytedance/deer-flow — deep-research

| Field | Value |
|---|---|
| Vendored file | `third_party/deer-flow/deep-research/SKILL.md` |
| Source repo | https://github.com/bytedance/deer-flow |
| License | MIT — Copyright (c) 2025 Bytedance Ltd. and/or its affiliates; Copyright (c) 2025-2026 DeerFlow Authors |
| License file | `third_party/deer-flow/LICENSE` |
| Pinned commit | `3725ba1bfb65046df589bf6346d1c6e92594c932` |
| Snapshot date | 2026-10-06 |

**Covers:** Systematic multi-angle web research methodology — initial survey, deep investigation, cross-checking, source reading protocol, quality checklist, and search strategy including temporal query construction.

**Gaps:** Designed for the DeerFlow tool ecosystem; references `web_fetch` and specific search tools that may not be available. Does not address domain-specific source hierarchies, RAG indexing, citation format, or evaluation rubrics.

**Safe use:** Use the research loop, quality checklist, and search strategy as methodology guidance. Adapt tool names and API calls to the actual environment; do not assume availability without verification.

---

## bytedance/deer-flow — consulting-analysis

| Field | Value |
|---|---|
| Vendored file | `third_party/deer-flow/consulting-analysis/SKILL.md` |
| Source repo | https://github.com/bytedance/deer-flow |
| License | MIT — same as above |
| License file | `third_party/deer-flow/LICENSE` |
| Pinned commit | `3725ba1bfb65046df589bf6346d1c6e92594c932` |
| Snapshot date | 2026-10-06 |

**Covers:** Two-phase consulting report framework. Phase 1: analysis framework with chapter skeleton, data requirements, and framework selection (SWOT, PESTEL, Porter, VRIO, BCG, etc.). Phase 2: final report generation after data collection. Includes output format and data authenticity protocol.

**Gaps:** Default output language is zh_CN; override with output_locale. Phase 1 assumes a downstream data-collection skill performs actual retrieval — it does not retrieve sources itself. Designed for DeerFlow multi-skill orchestration; handoff steps require adaptation for single-agent use.

**Safe use:** Use the analysis framework selection table and chapter skeleton as scaffolding for structured research reports. Drive web-research queries from Phase 1 output. Always apply citation and evidence requirements from `docs/web-research.md` — do not use without grounded source retrieval.
