# AI Research Knowledge Pack

Skills, prompt guides, and reference documents for AI-assisted research: web sourcing, RAG, LangChain/Redis stack, and domain-specific workflows.

This repository does not configure or run an AI model. The owner configures model, search provider, credentials, and contest rules separately from official organizer documentation.

## Quick Start

1. Read `AGENTS.md` — repo-wide ground rules for every AI task.
2. Open `.agents/skills/web-research/SKILL.md` — for any question that requires current facts from the internet.
3. Open `.agents/skills/rag-docs/SKILL.md` — for RAG, LangChain, LangGraph, or Redis/RedisVL guidance.
4. Open `.agents/skills/domain-research/SKILL.md` — for domain-specific research; load only the one topic reference that matches the task.
5. Fill `docs/competition-rules.template.md` from official organizer material only.

## Documents

| File | Purpose |
|---|---|
| `docs/web-research.md` | Source evaluation criteria, evidence record format, and grounded report structure. |
| `docs/rag-langchain-redis.md` | RAG concept map, stack roles, reading list, and nine domain topic guides. |
| `docs/research-evaluation-rubric.md` | Pre-delivery checklist: citation coverage, abstention, and source quality. |
| `docs/third-party-skills.md` | Provenance, commit, license, and gap notes for vendored third-party skills. |
| `docs/competition-rules.template.md` | Template for recording organizer-supplied contest rules. |

## Repository Layout

```
.agents/skills/
  web-research/SKILL.md
  rag-docs/SKILL.md
  domain-research/
    SKILL.md
    references/
      sales.md  journalism.md  landing-page.md  ai-integration.md
      education.md  history.md  accounting.md  business.md  travel.md
docs/
  web-research.md
  rag-langchain-redis.md
  research-evaluation-rubric.md
  third-party-skills.md
  competition-rules.template.md
third_party/
  langchain-skills/langchain-rag/SKILL.md   (MIT, langchain-ai)
  deer-flow/deep-research/SKILL.md          (MIT, ByteDance/DeerFlow)
  deer-flow/consulting-analysis/SKILL.md    (MIT, ByteDance/DeerFlow)
```
