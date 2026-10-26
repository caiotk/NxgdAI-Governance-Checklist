# AI Governance Checklist

_Twelve controls to build, run and evidence responsible AI at enterprise scale._

Version 1.1.0 · Updated 2026-10-26 · Published by NexGuide.AI

**Other formats:** [Interactive web checklist](https://caiotk.github.io/NxgdAI-Governance-Checklist/) · [Excel workbook](sheets/ai-governance-checklist.xlsx) · [CSV for Google Sheets](sheets/checklist.csv)

## Summary

| # | Control | Area | Owner |
|---|---|---|---|
| 01 | [AI inventory completed](#01--ai-inventory-completed) | Foundations | Chief AI Officer / AI governance lead |
| 02 | [Risk classification framework defined](#02--risk-classification-framework-defined) | Foundations | Chief Risk Officer |
| 03 | [Governance committee established](#03--governance-committee-established) | Accountability | Executive sponsor / Board |
| 04 | [AI policies documented](#04--ai-policies-documented) | Accountability | Chief AI Officer / General Counsel |
| 05 | [Model documentation standardised](#05--model-documentation-standardised) | Transparency | Model owner / ML engineering lead |
| 06 | [Bias and fairness testing implemented](#06--bias-and-fairness-testing-implemented) | Trustworthiness | Model owner / Data science lead |
| 07 | [Explainability requirements defined](#07--explainability-requirements-defined) | Trustworthiness | Business owner / Model owner |
| 08 | [Security and privacy controls applied](#08--security-and-privacy-controls-applied) | Protection | CISO / Privacy Officer |
| 09 | [Continuous monitoring enabled](#09--continuous-monitoring-enabled) | Operations | ML operations / Platform owner |
| 10 | [Incident response process established](#10--incident-response-process-established) | Operations | CISO / Head of operations |
| 11 | [Regulatory compliance reviews scheduled](#11--regulatory-compliance-reviews-scheduled) | Assurance | Compliance / Internal audit |
| 12 | [Generative AI usage rules created](#12--generative-ai-usage-rules-created) | Foundations | Chief AI Officer / CISO |

## The checklist

### 01 · AI inventory completed

- [ ] **AI inventory completed** — Identify and record every AI system, model, tool, agent and use case in the organisation, including embedded vendor AI and shadow use.

**Evidence an auditor will ask for:** AI register with owner, purpose, data used, vendor, risk tier and lifecycle status for each entry; date of last review.

**Quick test:** Pick three business units at random. Does every AI tool they use appear in the register?

**Suggested owner:** Chief AI Officer / AI governance lead

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 4.3, 7.5; Annex A.4 | GOVERN 1.6; MAP 1.1 | Art. 6, 49 (high-risk classification and registration) | IEEE 2863-2026 (governing-body oversight of AI); Australia AI6 practice 4 (AI system register) |

### 02 · Risk classification framework defined

- [ ] **Risk classification framework defined** — Apply one consistent method to rate AI risk by impact and likelihood, and tie each tier to the controls and approvals it requires.

**Evidence an auditor will ask for:** Approved risk methodology; risk tier recorded against every register entry; documented tier-to-control matrix.

**Quick test:** Can two assessors rate the same use case independently and land on the same tier?

**Suggested owner:** Chief Risk Officer

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 6.1, 8.2; Annex A.5 | MAP 1–5; GOVERN 1.3 | Art. 6, 9 (classification, risk management) | EN 18286:2026 (Art. 17(1)(g) risk management within the QMS); Australia AI6 practices 2–3 (impacts, risk) |

### 03 · Governance committee established

- [ ] **Governance committee established** — Stand up a cross-functional AI governance body with clear terms of reference, decision rights and a named accountable owner for every AI system.

**Evidence an auditor will ask for:** Terms of reference; membership spanning risk, legal, privacy, security, data and business; minutes showing decisions made.

**Quick test:** For any production AI system, can you name the one person accountable for it in under a minute?

**Suggested owner:** Executive sponsor / Board

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 5.1, 5.3; Annex A.3 | GOVERN 2.1–2.3 | Art. 17, 26 (quality management, deployer obligations) | IEEE 2863-2026 (governance principles and processes for the governing body); Australia AI6 practice 1 (accountability) |

### 04 · AI policies documented

- [ ] **AI policies documented** — Approve and publish policies covering ethics, acceptable use, data, model governance and accountability, and train people on them.

**Evidence an auditor will ask for:** Board- or executive-approved AI policy; review date; staff attestation or training completion records.

**Quick test:** Ask five staff where the AI policy lives and what it forbids. How many can answer?

**Suggested owner:** Chief AI Officer / General Counsel

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 5.2; Annex A.2 | GOVERN 1.2, 1.4 | Art. 4 (AI literacy), Art. 17 | EN 18286:2026 (harmonised QMS standard for Art. 17; presumption of conformity from 14 Oct 2026); IEEE 2863-2026 |

### 05 · Model documentation standardised

- [ ] **Model documentation standardised** — Use standard templates such as model cards and datasheets so every system can be understood, audited and handed over.

**Evidence an auditor will ask for:** Completed model card and data sheet per system, version-controlled, covering intended use, limits, training data provenance and evaluation results.

**Quick test:** Could an auditor who has never seen the system reconstruct what it does and why from the documentation alone?

**Suggested owner:** Model owner / ML engineering lead

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 7.5; Annex A.6, A.7 | MAP 2.1–2.3; MEASURE 2.1 | Art. 11, 12 (technical documentation, record-keeping) | EN 18286:2026 (Art. 17(1)(b)–(e) design, development, testing and technical specifications) |

### 06 · Bias and fairness testing implemented

- [ ] **Bias and fairness testing implemented** — Test models for bias across relevant groups, disaggregated rather than in aggregate, and act on what you find.

**Evidence an auditor will ask for:** Fairness test plan with defined groups and thresholds; disaggregated results; remediation log for findings.

**Quick test:** Are results reported per group, and is there a written threshold that would block release?

**Suggested owner:** Model owner / Data science lead

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Annex A.5, A.7 | MEASURE 2.11 | Art. 10 (data and data governance) | Australia AI6 practice 2 (impacts, incl. fairness); IEEE 2863-2026 (ethical principles) |

### 07 · Explainability requirements defined

- [ ] **Explainability requirements defined** — Set the level of explanation each system must provide based on the risk and impact of its decisions, including to affected people.

**Evidence an auditor will ask for:** Explainability standard by risk tier; sample explanations; human review and challenge route for affected individuals.

**Quick test:** If a person asks why the system decided against them, what exactly do you send them, and who sends it?

**Suggested owner:** Business owner / Model owner

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Annex A.8 | MEASURE 2.9 | Art. 13, 14, 86 (transparency, human oversight, right to explanation) | Australia AI6 practices 4 and 6 (information for affected people; human control) |

### 08 · Security and privacy controls applied

- [ ] **Security and privacy controls applied** — Protect data, models and outputs with security and privacy safeguards, including AI-specific threats such as prompt injection and data leakage.

**Evidence an auditor will ask for:** Privacy impact assessment; AI threat model; red-team or penetration test results; access controls on training data and prompts.

**Quick test:** Has the system been attacked on purpose (prompt injection, data exfiltration) before go-live, and were the findings fixed?

**Suggested owner:** CISO / Privacy Officer

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Annex A.7; aligns with ISO/IEC 27001, 27701 | MEASURE 2.7, 2.10 | Art. 15 (accuracy, robustness, cybersecurity) | ISO/IEC 27090:2026 (AI security threats: poisoning, evasion, model inversion and extraction, prompt and output injection) |

### 09 · Continuous monitoring enabled

- [ ] **Continuous monitoring enabled** — Monitor performance, data drift, fairness and system behaviour in production, with alerts that reach a named person.

**Evidence an auditor will ask for:** Monitoring dashboard; defined metrics and thresholds; alert routing; drift and performance reports over time.

**Quick test:** If accuracy dropped 10% after a vendor model update, who would get the alert, and how fast?

**Suggested owner:** ML operations / Platform owner

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 9.1; Annex A.6 | MANAGE 4.1; MEASURE 3.1 | Art. 72 (post-market monitoring) | EN 18286:2026 (Art. 17(1)(h) post-market monitoring); Australia AI6 practice 5 (monitoring); ISO/IEC 27090:2026 (attack detection) |

### 10 · Incident response process established

- [ ] **Incident response process established** — Define how AI incidents are detected, escalated, contained, remediated and reported, and rehearse it.

**Evidence an auditor will ask for:** AI incident playbook; severity definitions; incident log; at least one tabletop exercise with lessons learned.

**Quick test:** Can you switch the system off or roll it back today, and has anyone practised doing it?

**Suggested owner:** CISO / Head of operations

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 10.2; Annex A.8 | MANAGE 4.3; GOVERN 4.3 | Art. 73 (reporting of serious incidents) | EN 18286:2026 (Art. 17(1)(i) serious-incident procedures); Australia AI6 practice 5 (incident thresholds) |

### 11 · Regulatory compliance reviews scheduled

- [ ] **Regulatory compliance reviews scheduled** — Track changing laws and standards and run periodic compliance assessments and independent audits.

**Evidence an auditor will ask for:** Regulatory horizon register; compliance assessment schedule; internal audit reports and management responses.

**Quick test:** When did a law affecting your AI last change, and how long did it take you to notice?

**Suggested owner:** Compliance / Internal audit

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Cl. 9.2, 9.3 | GOVERN 1.1 | Art. 43 (conformity assessment), Art. 113 (application dates) | EN 18286:2026 (cited in the OJ on 14 Oct 2026; Art. 17(2)–(4) not covered); Australian Standards for AI (announced Jul 2026; bills expected 2027) |

### 12 · Generative AI usage rules created

- [ ] **Generative AI usage rules created** — Set clear rules for safe, responsible and compliant use of generative AI tools and models, including approved tools and data limits.

**Evidence an auditor will ask for:** Generative AI standard; approved-tools list; data classification rules for prompts; output review and labelling requirements.

**Quick test:** Do staff know which tools are approved, and what data they must never paste into them?

**Suggested owner:** Chief AI Officer / CISO

| ISO/IEC 42001 | NIST AI RMF | EU AI Act | Also maps to |
|---|---|---|---|
| Annex A.9, A.10 | NIST AI 600-1 (Generative AI Profile) | Art. 50 (transparency for certain AI systems), Art. 53 (GPAI providers) | ISO/IEC 27090:2026 (prompt injection; sensitive information in outputs) |

## How to use status

Track each control through: **Not started** → **In progress** → **Implemented** → **Evidenced**, or mark it **Not applicable** with a reason. A control only counts as done when it is **Evidenced** — implemented, and you can show an auditor the proof.

## Framework mapping note

Framework references are indicative mappings to help you find the relevant requirement. "Also maps to" covers ISO/IEC 27090:2026 (AI security), EN 18286:2026 (the EU AI Act harmonised quality-management standard), IEEE 2863-2026 (organisational AI governance) and Australia's Guidance for AI Adoption (AI6). Verify against the current official text of each standard or law before relying on them for compliance.

---

Strong governance builds trust. Responsible AI drives sustainable innovation.
