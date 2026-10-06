# AI Integration Research Guide

## Scope

Research covering integration of AI/LLM systems into products or workflows: capability assessment, risk evaluation, evaluation design, vendor selection, and responsible deployment.

## Source Hierarchy

1. Official model and API documentation: provider release notes, model cards, system cards, and technical reports disclosing training data, known limitations, and evaluation results.
2. Peer-reviewed AI safety and evaluation research: NeurIPS, ICML, ACL, ICLR, Arxiv preprints with institutional affiliation.
3. Standards and frameworks: NIST AI RMF, EU AI Act guidance, ISO/IEC 42001, OWASP LLM Top 10.
4. Independent benchmarks: HELM, BIG-Bench, LMSYS Chatbot Arena (note evaluation methodology and date of run).
5. Vendor documentation and blogs: treat as potentially promotional; cross-check capability claims against independent evaluation.

## Key Questions to Answer

- What specific task is the AI component performing, and what is its measured accuracy on a representative evaluation set?
- What are the documented failure modes, and what is their frequency and severity?
- What data does the system use as input, and what are the privacy and data-handling implications?
- What regulatory framework applies (EU AI Act risk tier, sector-specific regulations)?
- What human oversight and fallback mechanisms exist?
- How will the system's performance be monitored in production?
- What are the known bias and fairness risks for the target population?

## Common Evidence Traps

- Benchmark scores are context-specific; a model scoring well on a public benchmark may perform differently on the actual task and data distribution.
- Vendor accuracy claims often lack methodology disclosure; require task definition, dataset, evaluation metric, and comparison baseline.
- "Hallucination rate" varies by task and measurement method; figures are not comparable across providers unless methodology is identical.
- Compliance statements ("GDPR-compliant") are self-reported; verify against the actual regulatory requirement.

## Output Checklist

- [ ] Capability claims cite a specific evaluation with disclosed task, dataset, and metric.
- [ ] Failure modes are documented with frequency estimates where available.
- [ ] Applicable regulatory framework is identified with the current regulation version.
- [ ] Data flow and privacy implications cite applicable data protection law.
- [ ] Oversight and fallback procedures are defined.
