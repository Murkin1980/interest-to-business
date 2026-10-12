# A01 Nugget AI — CP-01 source register

**Accessed:** 2026-10-10. Public pages only. No login, no Mac app, no source clone.  
**Target:** [nggt.ai](https://nggt.ai/) (interview→evidence PM tool; maker Brodie / [@brodie_sv](https://www.producthunt.com/@brodie_sv)). **Not** nugget.ai (HR), nuggetz.ai, or Zomato Nugget.  
**Grades:** A = inspectable official page/legal/pricing; B = first-party operational claim; C = community; D = hypothesis.

## 1. Source register (10)

| ID | URL | Type | G | Why useful |
|---|---|---|---|---|
| S01 | https://nggt.ai/ | Site | A | Marketed loop, pricing, integration logos, MCP demo |
| S02 | https://nggt.ai/mcp | MCP guide | A | Hosted `mcp.nggt.ai`; 38 named tools / 10 domains |
| S03 | https://nggt.ai/download | Download | A | macOS 12+ Apple Silicon; v1.1.5 (2026-06-03); Win/Linux waitlist |
| S04 | https://nggt.ai/privacy | Privacy | A | Audio/transcripts collected; 90d after cancel; Google Limited Use |
| S05 | https://nggt.ai/terms | Terms | A | Consent to record; AL law; 30d delete (conflicts S04) |
| S06 | https://nggt.ai/ai-transparency | AI policy | B | OpenAI / Anthropic / Google; training opt-out (unverified) |
| S07 | https://www.producthunt.com/products/nugget-ai | PH | B | Maker Q&A on scoring/quality; 0 reviews; Alpha ~May 2026 |
| S08 | https://github.com/HunterHelms/nugget/releases | Releases | A | v1.0.0–v1.1.5 objects; README: source private |
| S09 | https://nggt.ai/the-mom-test-customer-interviews/ | Use-case | B | Not affiliated with Fitzpatrick; evidence preservation |
| S10 | https://www.producthunt.com/products/nugget-ai/built-with | Stack | B | AssemblyAI, Stripe, Claude Code (maker-authored) |

Sister pages (same grade B marketing): transcription, analysis, roadmap, repository, MCP-for-PMs.

## 2. Capability table

| Capability | Public claim | G | Evidence | Verified? |
|---|---|---|---|---|
| Capture | Live mic + system audio; upload Zoom / tickets / surveys / Slack | B | S01, S08 | Desktop not run |
| Transcribe | Real-time; AssemblyAI named | B | S01, S10 | Accuracy unknown |
| Nuggets | Pain, feature request, sentiment | B | S01, S07 | Extractor unseen |
| Synthesis | Themes by frequency, severity, recency | B | S01, S07 | Weights unpublished |
| Quality gate | Talk ratio, open/closed, sentiment, follow-up; flag low-signal | B | S07 maker only | Not on S01/S08 |
| Mom Test scripts | Pre-call non-leading generator | B | S07; S09 weaker | S09 defers to the book |
| Prioritize | Score vs PM strategic goals | B | S01, S07, S08 | Formula unknown |
| Thin sample | No pattern without source; surface thin n | B | S07 | UI unseen |
| Artifacts | Themes, priorities, insight reports, PRD + quotes | B | S01, S07, S08 | No sample files |
| Handoff | Linear / GitHub / Jira | B/C | S01 vs S07/S08 | S08: Linear/Jira/Slack “coming soon” |
| MCP | 38 tools; scoped tokens; Pro/Team | A names | S02 | Free-tier contradicts S01 |
| Pricing | Free 3 interviews; Pro $19.99/mo ($150/yr); Team $9.99/seat (5 seats $449/yr); 14-day trial | A | S01 | Not purchased |
| Platform | Sign-in desktop; Apple Silicon | A | S03, S08 | Blocks this sandbox |

Marketed loop (not authenticated UX): Capture → Synthesize → Prioritize → Spec → Ship.

## 3. BD-useful mechanisms (patterns; default REUSE_COMPONENT)

1. Provenance chain: claim → quote → interview → participant.
2. Quality gate *before* scoring (leading questions, talk ratio, closed questions).
3. Explicit thin-sample / low-signal flags.
4. Priority = frequency + severity + segment + recency × stated strategy; human keeps the weights.
5. Past behavior vs future intent as interview standard (Mom Test), not a cloned script engine.
6. Quote-backed artifacts (themes, ranked opportunities, memo/PRD) — do not add a second interview SaaS.

## 4. Unverified

Scoring math; quality thresholds; human-correction UX; live Linear/GitHub/Jira export; MCP on Free vs Pro; write-scope MCP; extraction calibration; consent UX; retention 30 vs 90 days; Slack/ticket ingest live vs planned.

## 5. Risks / limits for later CPs

- No Apple Silicon + no authorized account here → CP-02 needs owner-approved Mac session. No deceptive sign-up.
- Source private (`HunterHelms/nugget`); do not clone or infer algorithms.
- Terms: process only authorized recordings; no API abuse.
- Domain/email overlap with unrelated nugget.ai; robots.txt sitemap points at nugget.ai.
- PH: 0 reviews. Do not submit real PII to the competitor.
