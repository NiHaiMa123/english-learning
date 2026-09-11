# Review Queue

This file is the active spaced-review queue.

| Item | Type | Domain | Due | Interval | Status / last result | Source session |
|---|---|---|---|---|---|---|
| `fewer bugs` (not `less bugs`) | phrase / grammar | general technical | 2026-09-12 | 3 days | On 2026-09-09 evening independently produced `The new version has fewer crashes.` in changed context | 2026-09-07 |
| `stability issues` | phrase | software / Agent | 2026-09-12 | 3 days | Retrieved correctly in review; keep one more changed-context check | 2026-09-07 |
| singular `version` + `has` | grammar / phrase | general technical | 2026-09-12 | 3 days | On 2026-09-09 used `The new version has ...` correctly | 2026-09-07 |
| `have access to ...` | chunk | Agent / permissions | 2026-09-10 | 1 day | Produced correctly: `This agent has access to your email.` | 2026-09-09 |
| `grant access` / `revoke access` | contrast pair | Agent / permissions | 2026-09-12 | 3 days | On 2026-09-09 evening independently used `revoke the agent's access at any time`; `grant` not retested | 2026-09-09 |
| `sensitive action(s)` | phrase | Agent / safety | 2026-09-12 | 3 days | On 2026-09-09 evening independently produced `These are sensitive actions.` with correct spelling | 2026-09-09 |
| `should require user approval` | chunk / sentence pattern | Agent / safety | 2026-09-12 | 3 days | On 2026-09-09 evening independently produced `This operation should require user approval.` | 2026-09-09 |
| `without explicit permission` | chunk | Agent / permissions | 2026-09-12 | 3 days | Produced correctly in two written contexts | 2026-09-09 |
| `collision` vs `clipping` | contrast pair | Blender / cloth | 2026-09-12 | 1 day | On 2026-09-11 used both concepts, but the phrase `Even with collision enabled` needed correction; keep one more contrast check | 2026-09-09 manual |
| `penetration` | noun | Blender / cloth | 2026-09-12 | 1 day | On 2026-09-11 again produced plural `penetrations`; corrected to mass-noun use in `reduce penetration` | 2026-09-09 manual |
| `self-collision` / `intersect with itself` | chunk | Blender / cloth | 2026-09-12 | 1 day | Recalled `self-collision`, but wrote `self-collision enabled` and `clip through itself`; needs `Enabling self-collision ... intersect with itself` | 2026-09-09 manual |
| `merge-ready` | adjective | GitHub / Agent | 2026-09-11 | 1 day | Correctly produced in `make the pull request merge-ready` | 2026-09-09 scheduled |
| `fix failed checks` | chunk | GitHub / CI | 2026-09-11 | 1 day | Correctly retrieved and reused in final prompt | 2026-09-09 scheduled |
| `resolve review feedback` | chunk | GitHub / PR review | 2026-09-11 | 1 day | Correctly retrieved and reused in final prompt | 2026-09-09 scheduled |
| `resolve merge conflicts` | chunk | GitHub / Git | 2026-09-11 | 1 day | Initially wrote `solve the pull conflicts`; later corrected and reused | 2026-09-09 scheduled |
| `content exclusion(s)` | domain expression | GitHub / Agent safety | 2026-09-11 | 1 day | Produced `Content exclusions ...`; needs later contextual recall | 2026-09-09 scheduled |
| `keep A out of B` | sentence pattern / chunk | Agent / permissions | 2026-09-11 | 1 day | Correctly produced after contrast with `prevent A from doing B`; final task reverted to unnatural `make ... into` | 2026-09-09 scheduled |
| `count toward ...` / `count as ...` | chunk / contrast | GitHub / requirements | 2026-09-12 | 1 day | Initially interpreted `count toward` as replace; then independently produced `This approval can count toward one of the two required approvals.` | 2026-09-11 |
| `dismissed` / `approval is dismissed` | word / passive chunk | GitHub / PR review | 2026-09-12 | 1 day | Correctly recognized meaning and produced passive form in later integrated task | 2026-09-11 |
| `authorize A to do B` | sentence pattern | Agent / permissions | 2026-09-12 | 1 day | Initial noun-phrase form needed correction; then correctly produced `authorize the agent to modify these files` | 2026-09-11 |
| `assess whether ...` vs `verify that ...` | contrast pair | Agent / evaluation | 2026-09-12 | 1 day | Initially confused `assess`; later correctly chose and used `assess whether ...` in several changed contexts | 2026-09-11 |
| `meet the acceptance criteria` | chunk | Agent / GitHub | 2026-09-12 | 1 day | Used correctly several times; one spelling error in `criteria` occurred | 2026-09-11 |
| `assume + clause` | sentence pattern | general technical | 2026-09-12 | 1 day | Initial `assume this plan working` was incorrect; final task correctly used `Don't assume the new commit still works.` | 2026-09-11 |
| `reassess whether ...` | sentence pattern | Agent / evaluation | 2026-09-12 | 1 day | Correctly reused in final integrated Agent instruction | 2026-09-11 |
| `request a new review` | chunk | GitHub / PR review | 2026-09-12 | 1 day | Meaning understood; final output had spelling error `requirst`; needs clean recall | 2026-09-11 |
| `prioritize` | pronunciation / retrieval | speaking | deferred | next voice session | Pronunciation-specific review deferred during vocabulary-foundation phase | 2026-09-07 |

## Rules

- Due and overdue items normally come before new material.
- Recognition alone is not enough for mastery; prefer active recall or use in context.
- If recall fails, shorten the interval.
- If the learner uses the item naturally in a new context, extend the interval.
- For pronunciation items, use Voice evidence when available; do not infer pronunciation solely from transcript spelling.
