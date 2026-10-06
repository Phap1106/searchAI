# Web Research Guide

## Research Loop

Execute this loop for every research task. Scale depth to the decision impact and freshness requirements of the question.

1. **Define the question.** State scope, required date range, geography, language, and output format. Identify terms that need disambiguation before searching.
2. **Decompose.** Split broad questions into independently searchable subquestions. Assign each a priority based on how much the answer changes the conclusion.
3. **Search for primary evidence first.** Target official documentation, datasets, filings, standards, and research papers before secondary commentary.
4. **Read the source page, not the snippet.** Open the original URL and inspect the relevant passage, surrounding context, author identity, publication date, and supporting data. Record access date.
5. **Extract evidence in context.** Capture enough surrounding text to preserve definitions, units, caveats, scope, and method. Do not strip qualifications.
6. **Seek independent corroboration.** Cross-check important claims against sources that collected their own data independently. Syndicated copies, articles citing the same report, and aggregator pages are not independent corroboration.
7. **Resolve conflicts explicitly.** Compare source authority, methodology, sample size, definitions, and publication date. If a conflict cannot be resolved, report both positions and explain the disagreement; do not silently select the convenient one.
8. **Draft from evidence.** Write claims only to the strength supported by evidence. Place each citation immediately after the claim it supports, not only in a reference list.
9. **Audit before delivery.** Verify every factual claim has a citation to a source actually read; remove or downgrade unsupported specifics; preserve expressed uncertainty.

## Source Assessment Criteria

Evaluate every source against these six dimensions before including it as evidence.

| Dimension | Question to answer |
|---|---|
| **Authority** | Who produced this, and are they responsible for the underlying data or decision being cited? |
| **Proximity** | Is this primary evidence, or commentary, summary, or copied material? |
| **Method** | Are the sample, definitions, measurement approach, and limitations visible and appropriate for the claim? |
| **Recency** | Do publication and update dates fit the time sensitivity of the question? |
| **Independence** | Was this evidence collected independently, or does it trace back to a single shared source? |
| **Traceability** | Can the exact source and relevant passage be reopened and verified? |

Search ranking, polished writing, and publication in a well-known outlet do not establish reliability. Assess the evidence itself.

## Evidence Record Format

Create one record per distinct source/passage. Use this format in notes and reports.

| Field | Content |
|---|---|
| Evidence ID | Short stable identifier used in answer citations (e.g., `E1`) |
| Claim supported | The single verifiable claim this evidence supports |
| Title | Title as shown on the source |
| Publisher / Author | Organization or individual responsible for the content |
| URL | Exact URL of the page or document |
| Published / Updated | Date shown by the source, or `date unknown` |
| Accessed | Date the source was retrieved |
| Passage | Direct quotation within permitted limits, or a faithful paraphrase clearly marked as such |
| Scope / Caveats | Sample population, geographic scope, method limitations, or definitional boundaries that affect how broadly the claim applies |
| Independence level | `primary`, `independent corroboration`, or `derivative` |

## Report Format

Structure every research output as follows:

1. **Answer** — Concise response with inline citations (e.g., [E1]) next to each supported claim.
2. **Evidence summary** — List each evidence item: ID, source, and what claim it supports.
3. **Conflicts and gaps** — Describe source disagreements, missing dates, inaccessible pages, and open questions that could change the conclusion.
4. **Conclusion status** — One of: `fully supported`, `partially supported`, or `insufficient evidence`.

## Abstention Rules

Do not state a conclusion when:
- No retrieved source directly supports the specific claim.
- All supporting sources trace to a single origin (not independently verified).
- The only available sources are outdated by a margin that could change the answer.
- Retrieved content contradicts the claim without clear resolution.

In these cases, state exactly what evidence is missing and what type of source could resolve it.
