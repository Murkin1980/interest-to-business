# Arena Recon — checkpoint and change-budget policy

**MPE decision:** EXTEND_EXISTING. Applies to research Issues #2 and #3 (Nugget AI and Audity). No implementation is authorized.

## Non-negotiable scope
Research, public UX observation, independent functional specification, and gap analysis ONLY. No executable code, generated application, new repository, production integration, schema changes, deployments or reverse engineering through restricted access. Publicly accessible and authorized materials only.

## Sequential checkpoints (run A01 and A02 separately)
| CP | Scope | Output | Acceptance |
|---|---|---|---|
| CP-01 | Source inventory and legality/quality | source register, verified claims vs marketing, limitations | 5–10 useful references where available; source grades |
| CP-02 | Public user journey and input/output | UX step map, screenshots/links when permitted, unknowns | Observations traceable to references; no guessed internals |
| CP-03 | Compare to existing BD/Murat House/MPE components | reuse/duplicate/gap matrix | evidence of existing functionality from actual repository docs; no speculative rewrites |
| CP-04 | Independent component specifications | generalized contract, 5 synthetic test cases, risks and ROI hypotheses | implementable spec without copying competitor code; owner gate before any coding |

Each checkpoint is STOP/GO. Arena must finish its report and await review before proceeding to the next checkpoint. If review is unavailable, stop at current CP. Never run both targets in the same checkpoint PR.

## Size budget per checkpoint
- **Research phase: executable LOC budget 0.** Do not create source files, scripts, tests or dependencies.
- Each CP: **max 2 new/changed Markdown files** and **max 180 net added lines**; ideally one evidence file + one small checkpoint summary.
- Each PR: **max 250 changed lines total** (additions + deletions), 2 Markdown files, one CP for one product. If larger, split by content and checkpoint; no budget waivers without explicit owner approval.
- Prefer links, compact tables and claims tied to original sources over lengthy copied materials.
- Do not modify initial strategy PR #1 as part of Arena execution. Open draft checkpoint PR against `strategy/initial-v0.1` (or agreed research integration branch). Await review before merging.
- Reuse or update existing findings by reference rather than copying; one evidence item → one stable ID → multiple references.

## Checkpoint return protocol
`PROJECT; CP; RESULT: PASS|PARTIAL|BLOCKED; SOURCE_COUNT; VERIFIED/UNKNOWN; ADDED_LOC; DELETED_LOC; CHANGED_FILES; DUPLICATION_CHECK; DELIVERABLE_LINKS; RISKS; NEXT_GO_NO_GO`.

Exceeding limits, absence of primary evidence, attempts to access restricted material or inferred internal algorithms => STOP and report BLOCKED or PARTIAL; ask owner before scope change.

## Future code (requires separate MPE New Idea Filter and owner's permission)
Only if implementation is later authorized: seek REUSE_COMPONENT first. Suggested **proposal-only** guardrail: <= 200 net executable LOC per implementation PR, <= 3 implementation files; changes larger than this need split and explicit approval. These figures are not current authorization to write code.
