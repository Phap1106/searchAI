# Sales Research Guide

## Scope

Research covering sales strategy, customer acquisition, funnel analysis, conversion optimization, pricing, objection handling, CRM, sales operations, revenue metrics, and buyer psychology.

## Source Hierarchy

1. Primary buyer and sales data: CRM exports, sales call recordings and transcripts, win/loss analyses, customer surveys with methodology disclosed.
2. Industry research with method: reports from Gartner, Forrester, McKinsey, HBR, and academic journals with sample size, industry, and time period stated.
3. Practitioner platforms with disclosed methodology: SalesHacker, Pavilion, LinkedIn Sales research.
4. Vendor-published research: treat as potentially biased toward their product; cross-check against independent sources.
5. Blog posts, case studies, and thought leadership: corroboration only; not standalone evidence for quantitative claims.

## Key Questions to Answer

- What is the target customer segment, and what does primary data say about their buying behavior?
- What is the current state of the funnel: volume, conversion rate at each stage, average deal size, and sales cycle length?
- What objections appear at each stage, and what evidence explains them?
- What is the competitive landscape, and how do buyers compare alternatives?
- What pricing model and positioning best fits the segment based on evidence from comparable markets?
- What metrics define success, and how are they currently measured?

## Common Evidence Traps

- Conversion rate benchmarks vary widely by industry, channel, and deal size. Do not apply a generic benchmark without confirming it matches the specific context.
- Vendor-published statistics (e.g., "companies that use X see Y% improvement") require independent verification.
- Anecdotal case studies are not representative data. Treat as directional only.
- "Best practices" evolve with buyer behavior; confirm the source date before citing as current guidance.

## Output Checklist

- [ ] Every quantitative claim cites sample size, time period, geography, and measurement method.
- [ ] Competitive positioning claims cite independent sources, not vendor comparisons alone.
- [ ] Funnel metrics are segmented (not blended averages masking high variance).
- [ ] Jurisdiction or market is specified for all regulatory or pricing claims.
*** Add File: .agents/skills/domain-research/references/journalism.md
# Journalism and Fact-Checking Research Guide

## Scope

Research supporting news reporting, investigative journalism, source verification, claim fact-checking, media analysis, and misinformation assessment.

## Source Hierarchy

1. Primary documents: official records, court filings, government databases, financial disclosures, original data releases, and on-record statements.
2. On-record sources: named individuals with direct knowledge, cited with role and relationship to the claim.
3. Established fact-checking organizations with published methodology: PolitiFact, FactCheck.org, AFP Fact Check, Reuters Fact Check, Snopes (assess methodology per claim).
4. Archived contemporaneous reporting from reputable outlets.
5. Secondary analysis and commentary: corroboration only; note editorial stance of the publication.

## Key Questions to Answer

- What is the original source of the claim, and who made it first?
- What documentary evidence exists, and is it publicly accessible and authentic?
- Have named sources with direct knowledge confirmed it on record?
- Have independent outlets with different editorial stances reported the same facts?
- Is the claim verifiable, or does it depend on classified, private, or unavailable information?
- What is the strongest credible counter-evidence or alternative explanation?

## Verification Protocol

- Trace every claim to its original source; do not rely on summaries or retellings.
- Distinguish what a source says from what is independently confirmed.
- Identify the publication date of original reporting; note if subsequent reporting has corrected or updated the record.
- For images, audio, and video: note provenance, platform, upload date, and any available reverse-image or metadata check results.
- For statistics: identify the producing organization, methodology, sample, and time period.

## Common Evidence Traps

- Viral shares do not establish truth. Reach and engagement are not corroboration.
- Quotes stripped of context change meaning. Always verify the full original statement.
- Older correct facts may be outdated. Confirm whether the situation has changed since original reporting.
- Satire and parody are frequently mistaken for real reporting. Confirm the publication's stated purpose.

## Output Checklist

- [ ] Every factual claim traces to a primary document or named on-record source.
- [ ] Conflicting accounts are presented with explanation, not suppressed.
- [ ] Publication dates of all sources are recorded; outdated information is flagged.
- [ ] The verdict (true / false / misleading / unverifiable) is stated with supporting reasoning, not assertion.
*** Add File: .agents/skills/domain-research/references/landing-page.md
# Landing Page Research Guide

## Scope

Research supporting landing page strategy, conversion copy, headline claims, UX and accessibility, A/B testing, trust signals, CTA design, and compliance with advertising standards.

## Source Hierarchy

1. Platform and tool primary data: conversion analytics, heatmaps, session recordings, and A/B test results from the specific page or comparable audience.
2. Peer-reviewed UX and behavioral research: ACM CHI, Nielsen Norman Group research reports, Journal of Marketing Research.
3. Reputable CRO practitioners with disclosed methodology: ConversionXL (CXL), Baymard Institute (for checkout and form UX).
4. Platform-published benchmarks (Google, Meta, HubSpot): note industry, funnel stage, and date; do not generalize across contexts.
5. Blog posts and agency case studies: directional only; not standalone evidence for specific claim values.

## Key Questions to Answer

- What is the primary action the visitor must take, and what friction currently prevents it?
- What claims are made on the page, and what evidence supports each?
- Are there regulatory constraints on claims (advertising standards, consumer protection law) applicable to the jurisdiction and product category?
- What trust signals are present, and are they verifiable?
- What does the target audience's primary data reveal about their decision drivers and objections?
- What have controlled tests on comparable pages shown about headline, CTA, and form design?

## Common Evidence Traps

- "The average conversion rate is X%" — benchmark is meaningless without industry, traffic source, device, and funnel stage specified.
- Case study results are not transferable. Results depend on audience, offer, traffic source, and testing rigor; treat as directional.
- Heuristics (e.g., "above the fold," "7 trust signals") are starting hypotheses, not proven rules. Cite the test that validated them for a comparable context.
- Superlative claims ("fastest," "best," "#1") require substantiated basis per advertising standards (FTC, ASA, or applicable body).

## Output Checklist

- [ ] Every headline or body claim is linked to evidence or flagged as requiring substantiation.
- [ ] Regulatory constraints for the jurisdiction and product category are identified.
- [ ] Benchmark figures include industry, funnel stage, traffic source, and date.
- [ ] Trust signals are assessed for verifiability (real reviews, actual certifications, genuine data).
*** Add File: .agents/skills/domain-research/references/ai-integration.md
# AI Integration Research Guide

## Scope

Research covering integration of AI/LLM systems into products or workflows, covering capability assessment, risk evaluation, evaluation design, operational concerns, vendor selection, and responsible deployment.

## Source Hierarchy

1. Official model and API documentation: provider release notes, model cards, system cards, and technical reports disclosing training data, known limitations, and evaluation results.
2. Peer-reviewed AI safety and evaluation research: NeurIPS, ICML, ACL, ICLR, Arxiv preprints with institutional affiliation.
3. Standards and frameworks: NIST AI RMF, EU AI Act guidance, ISO/IEC 42001, OWASP LLM Top 10.
4. Independent benchmarks and evaluation organizations: HELM, BIG-Bench, LMSYS Chatbot Arena (note evaluation methodology and date).
5. Vendor documentation and blog posts: treat as marketing material; cross-check capability claims against independent evaluation.

## Key Questions to Answer

- What specific task is the AI component performing, and what is its measured accuracy on a representative evaluation set?
- What are the documented failure modes, and what is their frequency and severity?
- What data does the system use as input, and what are the privacy and data-handling implications?
- What regulatory framework applies (EU AI Act risk tier, sector-specific regulations)?
- What human oversight and fallback mechanisms exist?
- How will the system's performance be monitored in production?
- What are the known bias and fairness risks for the target population?

## Common Evidence Traps

- Benchmark scores are context-specific. A model scoring well on a public benchmark may perform differently on the specific task and data distribution.
- Vendor accuracy claims often lack methodology disclosure. Require: task definition, dataset, evaluation metric, and comparison baseline.
- "Hallucination rate" varies by task and measurement method. Figures are not comparable across providers unless methodology is identical.
- Compliance statements ("GDPR-compliant") are self-reported. Verify against the actual regulatory requirement.

## Output Checklist

- [ ] Capability claims cite a specific evaluation with disclosed task, dataset, and metric.
- [ ] Failure modes are documented with frequency estimates where available.
- [ ] Applicable regulatory framework is identified and current regulation version is noted.
- [ ] Data flow and privacy implications are stated with reference to applicable data protection law.
- [ ] Oversight and fallback procedures are defined.
*** Add File: .agents/skills/domain-research/references/education.md
# Education Research Guide

## Scope

Research covering pedagogy, curriculum design, learning outcomes, educational technology, assessment, student engagement, professional development, and education policy.

## Source Hierarchy

1. Peer-reviewed educational research: Journal of Educational Psychology, American Educational Research Journal, Review of Educational Research, British Journal of Educational Technology.
2. Government and intergovernmental bodies: UNESCO, OECD PISA/TALIS reports, national ministry of education statistics with disclosed methodology.
3. Research centers with transparent methodology: What Works Clearinghouse (evidence standards), Education Endowment Foundation (EEF), Campbell Collaboration.
4. Curriculum standards bodies: national or state/regional curriculum frameworks applicable to the jurisdiction.
5. Practitioner publications and ed-tech vendor research: directional only; note potential commercial interest.

## Key Questions to Answer

- What is the learning objective, and how is mastery currently measured?
- What does peer-reviewed evidence say about the effectiveness of the proposed method for this learner population?
- What are the age group, prior knowledge level, socioeconomic context, and language of instruction?
- What curriculum standards or accreditation requirements apply?
- What is the evidence base for the assessment approach?
- What barriers to access or equity exist for the target population?

## Common Evidence Traps

- Effect sizes from meta-analyses are averages across varied contexts; confirm that the original studies match the target learner population and setting.
- Learning style theories (visual/auditory/kinesthetic) lack robust empirical support; do not treat as established fact.
- Ed-tech efficacy claims from vendors frequently lack control groups or independent replication.
- Policy context matters: what works in one jurisdiction may not transfer due to curriculum, teacher training, or resource differences.

## Output Checklist

- [ ] Learner population (age, context, prior knowledge) is specified for all evidence cited.
- [ ] Effect sizes are reported with sample size, study design (RCT vs. observational), and confidence interval where available.
- [ ] Applicable curriculum standards or accreditation requirements are identified.
- [ ] Equity and access implications are addressed.
*** Add File: .agents/skills/domain-research/references/history.md
# Historical Research Guide

## Scope

Research covering historical events, periods, figures, and processes, including primary source analysis, historiographical debate, chronology verification, and causal interpretation.

## Source Hierarchy

1. Primary sources: original documents, official records, contemporaneous accounts, archaeological findings, and archival material with provenance established.
2. Peer-reviewed historical scholarship: journals such as American Historical Review, Past & Present, Journal of Modern History, and domain-specific journals.
3. University press monographs and edited volumes with peer review.
4. Reference works: Dictionary of National Biography, Encyclopedia of World History, country-specific national encyclopedias.
5. Popular history, documentary, and general encyclopedias: background orientation only; not standalone evidence for contested factual claims.

## Key Questions to Answer

- What primary sources directly document the event, decision, or figure in question?
- What is the scholarly consensus, and where does significant historiographical debate exist?
- What is the provenance and reliability of the primary source: who created it, when, for what purpose, and for what audience?
- Are there conflicting accounts, and what explains the conflict (perspective, access to information, political context)?
- What is the chronological context, and does the source date from before, during, or after the events it describes?
- How have subsequent discoveries or reinterpretations changed the historical understanding?

## Primary Source Evaluation

| Question | Why it matters |
|---|---|
| Who created this source? | Authorship affects perspective, access, and incentive to represent facts accurately. |
| When was it created relative to the event? | Contemporary accounts differ from retrospective accounts in reliability and purpose. |
| What was the intended audience? | Public documents differ from private correspondence in what they reveal. |
| What does the author know that they cannot know? | Anachronism and retroactive attribution are common errors in secondary interpretation. |
| Is the source authentic? | Forgeries and misattributions exist; note when authenticity is established or disputed. |

## Common Evidence Traps

- Wikipedia is not a primary source; use it to locate sources, then verify at origin.
- Documentary and popular history programmes often compress, dramatize, or simplify contested history.
- Dates in historical secondary sources sometimes follow different calendars (Julian vs. Gregorian); note the system used.
- "Common knowledge" historical facts are often simplified, partially incorrect, or actively disputed in scholarship.

## Output Checklist

- [ ] Every factual claim cites a primary source or peer-reviewed scholarship with publication date.
- [ ] Contested interpretations are identified, and the state of scholarly debate is described.
- [ ] Anachronistic language or concepts have been avoided or flagged.
- [ ] Dates include calendar system notation where relevant.
*** Add File: .agents/skills/domain-research/references/accounting.md
# Accounting and Financial Reporting Research Guide

## Scope

Research covering financial reporting standards, accounting treatment, taxation, audit, internal controls, financial analysis, and regulatory compliance.

## Source Hierarchy

1. Authoritative standards bodies: IFRS Foundation (IASB standards), FASB (US GAAP ASC), IAASB (auditing standards), PCAOB, national tax authorities.
2. Regulatory bodies: SEC filings and guidance, ESMA, national financial regulators.
3. Big-4 and major accounting firm technical guidance: Deloitte, EY, KPMG, PwC accounting guides — useful for interpretation, but represent the firm's view, not the standard itself.
4. Peer-reviewed accounting journals: The Accounting Review, Journal of Accounting Research, Journal of Finance.
5. CPA/ACCA/CIMA professional body guidance: jurisdiction-specific; note applicable geography.

## Key Questions to Answer

- Which accounting standard applies (IFRS, US GAAP, local GAAP), and what is the current effective version?
- What is the specific ASC topic, IFRS standard number, or equivalent reference?
- What jurisdiction's tax law applies, and what is the current tax year and applicable rate?
- Are there pending amendments or exposure drafts that could change the treatment?
- Is there interpretive guidance from the relevant standard-setter or regulator?
- What disclosure requirements apply, and in which financial statement section?

## Standard-Specific Anchors

- IFRS: https://www.ifrs.org/issued-standards/
- US GAAP (ASC): https://asc.fasb.org/
- PCAOB standards: https://pcaobus.org/Standards
- IRS (US tax): https://www.irs.gov/
- HMRC (UK tax): https://www.gov.uk/government/organisations/hm-revenue-customs

## Common Evidence Traps

- Accounting standards are amended frequently. Always confirm the effective date of the version cited.
- IFRS and US GAAP treatment differs on many items. Confirm which framework applies before citing a treatment.
- Tax rates, thresholds, and elections change each fiscal year. State the year and jurisdiction for every tax figure.
- Big-4 guidance materials are interpretations, not the standard itself. Cite the standard directly for authoritative treatment.
- "Common practice" is not the same as required treatment; distinguish between what standards require and what firms typically do.

## Output Checklist

- [ ] The applicable standard, version, and effective date are stated.
- [ ] Jurisdiction and tax year are specified for all tax claims.
- [ ] Pending amendments relevant to the treatment are noted.
- [ ] Standard-setter or regulator citations are direct, not filtered through firm interpretations.
*** Add File: .agents/skills/domain-research/references/business.md
# Business and Market Research Guide

## Scope

Research covering market analysis, competitive intelligence, company research, strategy, operations, supply chain, M&A, investment due diligence, and macroeconomic context.

## Source Hierarchy

1. Primary company data: annual reports, 10-K/20-F filings, investor presentations, earnings call transcripts, and official press releases.
2. Regulatory filings and government statistics: SEC EDGAR, Companies House, national statistics bureaus (BLS, ONS, GSO), central bank data.
3. Paid industry research with disclosed methodology: Gartner Magic Quadrant, Forrester Wave, IBISWorld, Euromonitor, Statista (verify methodology and sample for each dataset).
4. Reputable financial and business journalism: FT, WSJ, Bloomberg, Reuters, The Economist — for context and synthesis, not as primary data.
5. Vendor and consulting firm research: note potential commercial interest; cross-check key figures against independent sources.

## Key Questions to Answer

- What is the target market size, and how was it measured (TAM/SAM/SOM methodology and source)?
- Who are the primary competitors, and what do their public filings reveal about positioning, revenue, and strategy?
- What macro and regulatory trends affect this market, and what is the source and timeframe?
- What is the company's financial position, and what ratios are relevant to the research question?
- What is the basis for any growth rate or forecast — bottom-up or top-down, and what are the key assumptions?
- Are there pending regulatory changes, M&A activity, or supply chain risks that could change the analysis?

## Common Evidence Traps

- Market size figures vary significantly across research firms due to different definitions, geographies, and methodologies. Always state the source and note definitional scope.
- Revenue figures from private companies are estimates unless from audited filings. State source confidence.
- Industry CAGR forecasts embed assumptions about adoption, competition, and macro conditions. Treat as directional; note the date and the forecast horizon.
- Competitor "intelligence" from third-party sources may be outdated or inferred. Prefer primary filings.
- "Market leader" claims require substantiation: leader by what metric, in what geography, over what period?

## Output Checklist

- [ ] Market size and growth figures state source, methodology, geography, and date.
- [ ] Competitor data cites public filings or audited sources where available.
- [ ] Forecasts are labeled as estimates with stated assumptions and forecast horizon.
- [ ] Regulatory or macro risks are current (within 12 months) or flagged as potentially outdated.
*** Add File: .agents/skills/domain-research/references/travel.md
# Travel Destination Research Guide

## Scope

Research covering travel destinations, visa and entry requirements, safety and security conditions, health requirements, accommodation, transport, local regulations, and traveler logistics.

## Source Hierarchy

1. Government travel advisories and entry requirement portals: destination country's official immigration authority; traveler's home country foreign ministry travel advisory (e.g., US State Dept, FCDO, DFAT, MOFA).
2. International health authorities: WHO travel health notices, CDC Travelers' Health, destination country health ministry.
3. Official destination tourism boards for general information: note they have a promotional interest.
4. Established travel platforms with recent user reviews (Tripadvisor, Google Maps, Booking.com): useful for current operational status and recent visitor experience; not authoritative for regulations.
5. Travel journalism and guidebooks: orientation only; verify regulatory and safety details against government sources.

## Key Questions to Answer

- What are the current entry requirements: visa, passport validity, onward ticket, proof of funds, and vaccination requirements for the traveler's specific nationality?
- What is the current government travel advisory level, and what specific risks are cited?
- What health requirements and recommended vaccinations apply?
- What local laws differ significantly from the traveler's home country (alcohol, photography, dress, currency export)?
- What is the current operational status of key attractions, transport links, and accommodation?
- What emergency contacts and consular services are available at the destination?

## Time Sensitivity Rules

Travel regulations and safety conditions change rapidly. Apply these rules to every output:

- Visa and entry requirements: treat any source older than 90 days as potentially outdated; direct the traveler to the official immigration authority for current requirements.
- Travel advisories: state the advisory level and date; note that conditions can change within days.
- Health requirements: direct to WHO and the traveler's national health authority for current vaccination and medication requirements.
- Operational status (hours, prices, closures): treat sources older than 30 days as potentially outdated; direct to the venue's official source.

## Common Evidence Traps

- Visa requirements depend on the traveler's specific passport, not generic "tourist" requirements. Always specify nationality.
- Informal traveler reports on forums may reflect outdated conditions or exceptional individual experiences.
- Tourism board content promotes the destination; safety and regulatory information requires independent official verification.
- "Visa on arrival" policies change without notice. Verify at the official immigration portal.

## Output Checklist

- [ ] Visa and entry requirements cite the official immigration authority of the destination country.
- [ ] Travel advisory level and issue date are stated for the traveler's home country.
- [ ] Health requirements cite WHO or national health authority, with access date.
- [ ] All time-sensitive information is labeled with the source date and a directive to verify before travel.
- [ ] Local laws that differ significantly from the traveler's home country are explicitly flagged.
