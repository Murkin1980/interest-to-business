# A01 Nugget AI — CP-03 BD access probe (read-only)

**Date:** 2026-10-10. **MPE:** REUSE_COMPONENT. **Issue:** #2 / EXP-ITB-01 #8.  
**Rule:** repository-grounded only. No BD implementation claims from docs. No Nugget source copy. CP-02 remains BLOCKED.

## Access probe

| Target | Method | Result |
|---|---|---|
| `Murkin1980/interest-to-business` | `gh` + git push | Accessible (this repo) |
| `Murkin1980/business-discovery` | `gh api repos/…` | **403** `Resource not accessible by integration` |
| same | `git ls-remote https://github.com/Murkin1980/business-discovery.git` | **403** |
| same | listed under `users/Murkin1980/repos` | **Absent** |
| same | local clone | **None** |

Arena cannot read BD code, fixtures, or Stage 5 UI. Matrix code paths are therefore **not filled**.

## Reuse/gap matrix — blocked (no invented paths)

| Nugget mechanism (public, CP-01) | Existing BD component | Actual code path | Gap | Recommendation |
|---|---|---|---|---|
| Quote provenance / claim→source | unknown | **unverified** | no repo read | Grant Arena **read** on BD; Codex BD-EVIDENCE-01 first |
| Evidence vs Value score split | unknown | **unverified** | cannot confirm contracts | Reuse existing scores only; never mix |
| Consent / UNKNOWN / probing | unknown | **unverified** | cannot confirm | Keep UNKNOWN; no fake confidence |
| Independent-source dedup / conflicts | unknown | **unverified** | cannot confirm | No new scoring engine |
| Stage 5 Evidence Card surface | unknown | **unverified** | cannot confirm | Extend Stage 5 only if audit shows it |
| Thin-sample warning | unknown | **unverified** | cannot confirm | Visible n-warning; no invented n |
| Synthetic fixtures for MVP | unknown | **unverified** | cannot confirm | Demo on existing fixtures only |

## Unbound acceptance cases (EXP-ITB-01 #8 — not BD-path-bound)

Use after Codex maps real files. Do **not** treat as verified BD behavior.

1. **AC-PROVENANCE:** a card claim without a consent-appropriate quote/evidence link renders UNKNOWN, not a numeric score.
2. **AC-DEDUP:** two records of one source do not increase independent-source count.
3. **AC-THIN:** below-threshold n shows an explicit thin-sample warning; no invented confidence.
4. **AC-SCORES:** Evidence Score and Value Score stay separately labeled; if a contract is missing, omit that score rather than mixing.
5. **AC-CONSENT:** non-consented or non-synthetic-unauthorized text is not shown as a customer quote.

## Stop

No BD code change, migration, merge, or deploy. Next: owner grants BD read, or Codex posts a path-bound audit. Then re-run CP-03.
