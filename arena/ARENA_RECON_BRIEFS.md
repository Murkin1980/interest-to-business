# Arena component reconnaissance briefs — owner review required

**Status: PREPARED, NOT ASSIGNED OR RUN.** These are technical investigations, not authorization to clone protected functionality, harvest private data, bypass access controls, or deploy.

## Common rules
- Analyze only public, intentionally accessible pages, official documentation, demonstration flows, openly licensed source, and permitted UI behavior.
- Never bypass logins, CAPTCHAs, rate limits, paywalls, or access restrictions. No deceptive accounts or harvesting real user data.
- Do not copy proprietary code, product branding, assets, datasets, or protected prompts.
- Reconstruction means independent specification of a **generalized pattern**, not replication of a competitor product.
- Use synthetic interview transcripts, synthetic business assessments and mock customer records.
- Record URLs, access date, screenshots/observations if lawful, network behavior only from an authorized session, confidence, limitations, alternatives and ToS risks.
- No production credentials, no Cloudflare deployment, no new repository, no schema/API changes, no merge.
- Deliver evidence only to this ITB repository as draft or PR; proposals affecting BD/Murat House/MPE require separate MPE review and owner's deep-change approval.

## A01 — Nugget AI: evidence-backed interview quality (P1)
Goal: understand the observable UX contract for interviews → traceable findings → synthesis → prioritized action.
Questions: leading-question prevention; confidence and sample-size display; source quote provenance; priority rationale; human corrections.
Deliverables: screen inventory, input/output schema proposal (synthetic), evidence grading rubric, 3 fake interviews showing bias, recommended BD reuse vs gap matrix, 5 acceptance tests.
Stop if only marketing descriptions are accessible: do not invent internal logic.
Adoption default: REUSE_COMPONENT from BD contracts, not reimplement interview service.

## A02 — Audity: qualifying assessment vs billable audit (P1)
Goal: study assessment intake, consultant review and report deliverables, and cost-based quotation framework.
Questions: vertical tailoring, lead qualification, public seven-factor pricing rubric, sample PDF/memo structure, audit scope gates, report traceability.
Deliverables: observable funnel and screenshots, synthetic assessment, independently developed report outline, simple pricing worksheet (not copied), time-to-complete experiment, BD reuse matrix.
Do not submit real business or personal information to competitor.
Adoption default: EXTEND_EXISTING Business Discovery only if unmet requirement demonstrated.

## A03 — Trend Seeker: evidence-linked market signals (P2)
Goal: map publicly observable signal → cluster → opportunity → sources UX.
Deliverables: source quality rubric, provenance graph example as flat table, duplicate/freshness and noise handling hypotheses, manual 10-signal sample. Do not scrape platform databases or replicate proprietary datasets.
No automated crawler or agent without separate gate.
Adoption default: EXPERIMENT, manual research only.

## A04 — Robynn: change approval/measurement/rollback (P2)
Goal: observe publicly documented UI approval gates and brand-context pattern.
Deliverables: proposed stage/approve/measure/rollback state machine, governance comparison with existing Cloudflare preview + MPE acceptance, experiment design for synthetic landing page, risk register.
No access to or changes to live sites.
Adoption default: REUSE_COMPONENT / HOLD pending governance review.

## A05 — Pillar: conversion flow benchmark (read-only)
Goal: evaluate clear offer → CTA → qualification → booking → payment messaging.
Deliverable: annotated funnel, top 5 copy/UX improvements for Murat House and proof needed. No storefront or payment integration.

## A06 — Idea Validator: onboarding benchmark (read-only)
Goal: blank canvas versus prefilled examples and templates.
Deliverable: 1-page UX critique and sample fictitious filled project. No product cloning.

## A07 — ValidatorAI: idea-scoring critique (read-only)
Goal: compare AI-generated confidence with evidence from interviews and customer actions.
Deliverable: falsifiable test matrix with 5 contrasting fictional ideas, confidence language recommendations, no copied scoring algorithms.

## Sequence and gates
CP-01: Source legitimacy/access and documentary inventory.
CP-02: Public UI walkthrough with explicit unknowns.
CP-03: Generalized behavior model + contract gap map against existing repositories.
CP-04: synthetic test cases and scored component recommendations.
**STOP** before implementation; do not open code PRs in consumer projects automatically.

## Return format
RESULT PASS / PARTIAL / BLOCKED; SOURCE_LINKS; VERIFIED_OBSERVATIONS; UNVERIFIED_CLAIMS; EXTRACTABLE_PATTERNS; DUPLICATION_CHECK; PRIVACY_TERMS_RISKS; PROPOSED_OWNER; MINIMAL_EXPERIMENT; ACCEPTANCE_TESTS; BLOCKERS; NEXT_GATE.
