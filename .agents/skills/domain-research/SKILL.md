---
name: domain-research
description: Research questions in a specific professional or subject domain — sales, journalism, landing page, AI integration, education, history, accounting, business, or travel. Load only the one topic reference that matches the task. Use web-research for source retrieval and rag-docs for stack questions.
---

# Domain Research Skill

This skill provides domain-specific research frameworks, source hierarchies, and prompt checklists. It does not replace the web-research skill for actual source retrieval or rag-docs for stack guidance.

## How to Use

1. Identify the primary domain of the research task.
2. Load only the one matching topic reference from the table below.
3. Apply the web-research workflow (`../web-research/SKILL.md`) to retrieve evidence using the domain-specific source hierarchy and questions provided in the reference.
4. Apply the evaluation rubric (`../../../docs/research-evaluation-rubric.md`) before delivering the output.

## Topic Reference Index

| Domain | File to load |
|---|---|
| Sales, customers, funnel, conversion, revenue | `references/sales.md` |
| Journalism, verification, fact-checking, reporting | `references/journalism.md` |
| Landing pages, conversion copy, UX claims | `references/landing-page.md` |
| AI integration, risk assessment, evaluation, deployment | `references/ai-integration.md` |
| Education, pedagogy, curriculum, learning research | `references/education.md` |
| History, primary sources, chronology, interpretation | `references/history.md` |
| Accounting, financial reporting, standards, tax | `references/accounting.md` |
| Business, markets, competitors, strategy, operations | `references/business.md` |
| Travel destinations, visa, safety, logistics | `references/travel.md` |

## Universal Domain Research Rules

- Jurisdiction matters. Standards, laws, regulations, and best practices vary by country and region. Always identify the applicable jurisdiction before stating a rule as fact.
- Distinguish current from historical. Regulations, market data, and statistics expire. State the source date and note when information may have changed.
- Professional domains require professional primary sources. Academic papers, government statistics, regulatory filings, and standards body publications outrank blog posts, vendor content, and AI-generated summaries.
- Quantitative claims need method transparency. Report sample size, time period, geography, and definition. Aggregate figures from incompatible studies without noting differences in method.
- Topic guides are frameworks, not authoritative sources. They improve search focus and evaluation; they do not substitute for retrieved evidence.
