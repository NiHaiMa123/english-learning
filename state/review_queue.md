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
| `penetration` / `reduce penetration` | noun / chunk | Blender / cloth | 2026-09-16 | 3 days | On 2026-09-13 independently produced `Increasing collision quality may reduce penetration.` correctly after earlier countability errors | 2026-09-09 manual |
| `self-collision` / `intersect with itself` | chunk | Blender / cloth | 2026-09-14 | 1 day | Not actively retrieved on 2026-09-13; answer was shown after learner skipped the prompt, so keep high priority | 2026-09-09 manual |
| `merge-ready` | adjective | GitHub / Agent | 2026-09-11 | 1 day | Correctly produced in `make the pull request merge-ready` | 2026-09-09 scheduled |
| `fix failed checks` | chunk | GitHub / CI | 2026-09-11 | 1 day | Correctly retrieved and reused in final prompt | 2026-09-09 scheduled |
| `resolve review feedback` | chunk | GitHub / PR review | 2026-09-11 | 1 day | Correctly retrieved and reused in final prompt | 2026-09-09 scheduled |
| `resolve merge conflicts` | chunk | GitHub / Git | 2026-09-11 | 1 day | Initially wrote `solve the pull conflicts`; later corrected and reused | 2026-09-09 scheduled |
| `content exclusion(s)` | domain expression | GitHub / Agent safety | 2026-09-11 | 1 day | Produced `Content exclusions ...`; needs later contextual recall | 2026-09-09 scheduled |
| `keep A out of B` | sentence pattern / chunk | Agent / permissions | 2026-09-11 | 1 day | Correctly produced after contrast with `prevent A from doing B`; final task reverted to unnatural `make ... into` | 2026-09-09 scheduled |
| `count toward ...` / `count as ...` | chunk / contrast | GitHub / requirements | 2026-09-14 | 1 day | On 2026-09-13 used `count into` for `count toward`, then correctly produced `count as a sensitive operation`; contrast remains unstable | 2026-09-11 |
| `dismissed` / `approval is dismissed` | word / passive chunk | GitHub / PR review | 2026-09-16 | 3 days | On 2026-09-13 correctly reused `If the previous approval is dismissed ...` | 2026-09-11 |
| `authorize A to do B` | sentence pattern | Agent / permissions | 2026-09-16 | 3 days | On 2026-09-13 correctly produced `authorize the agent to modify these files`; only `administrator` word choice/spelling needed correction | 2026-09-11 |
| `assess whether ...` vs `verify that ...` | contrast pair | Agent / evaluation | 2026-09-14 | 1 day | `assess whether` was retrieved, but surrounding lexical choice drifted to `verification criteria`; keep contrast active | 2026-09-11 |
| `meet the acceptance criteria` | chunk | Agent / GitHub | 2026-09-14 | 1 day | On 2026-09-13 later used the chunk correctly, but initially wrote `verification cirteral`; lexical/spelling reinforcement still needed | 2026-09-11 |
| `assume + clause` | sentence pattern | general technical | 2026-09-16 | 3 days | On 2026-09-13 correctly produced `Don't assume the new commit still works.` and reused `assume` in final task, though final grammar needed `don't assume` | 2026-09-11 |
| `reassess whether ...` | sentence pattern | Agent / evaluation | 2026-09-14 | 1 day | When explicitly prompted on 2026-09-13, learner used `assess whether` instead of `reassess whether`; needs direct recall | 2026-09-11 |
| `request a new review` | chunk | GitHub / PR review | 2026-09-16 | 3 days | On 2026-09-13 independently produced `request a new review` cleanly after previous spelling error | 2026-09-11 |
| `reproduce the issue` | chunk | debugging / Agent | 2026-09-16 | 3 days | Correctly retrieved and reused several times on 2026-09-13 | 2026-09-13 |
| `narrow down the cause` | chunk | debugging / Agent | 2026-09-14 | 1 day | Correct on first retrieval; final integrated task had spelling error `narraw`, so keep short interval | 2026-09-13 |
| `root cause` | phrase | debugging / Agent | 2026-09-16 | 3 days | Retrieved correctly in several changed contexts on 2026-09-13 | 2026-09-13 |
| `workaround` / `use a workaround` | noun / chunk | debugging / Agent | 2026-09-14 | 1 day | First wrote `wordaround`; final task recalled `workaround` but used `take a workaround`; collocation still unstable | 2026-09-13 |
| `address the root cause` | chunk | debugging / Agent | 2026-09-16 | 3 days | Correctly produced `doesn't address the root cause` in a changed context | 2026-09-13 |
| `isolate the issue` | chunk | debugging / Agent | 2026-09-14 | 1 day | Target chunk retrieved correctly, but surrounding structure `before judge whether caused by ...` needed correction | 2026-09-13 |
| `dependency` | noun | debugging / software | 2026-09-14 | 1 day | Meaning understood; article and passive structure needed support | 2026-09-13 |
| `edge case` | domain expression | debugging / software | 2026-09-14 | 1 day | Meaning retrieved, but learner used `on one edge case`; later sentence needed passive `is triggered` | 2026-09-13 |
| `regression` | noun | debugging / software | 2026-09-14 | 1 day | Initial production `bug of regression` was unnatural; later `a truly regression` showed adjective/form issue | 2026-09-13 |
| `expected behavior` / `actual behavior` | contrast pair | debugging / software | 2026-09-16 | 3 days | Cleanly produced `Determine the expected and actual behavior before reproducing the issue`; later comparison grammar needed `the same as` | 2026-09-13 |
| `fallback` | noun / domain expression | software / Agent | 2026-09-14 | 1 day | Meaning understood; conditional tense/article needed correction | 2026-09-13 |
| `constraint` | noun | engineering / software | 2026-09-14 | 1 day | Meaning understood; spelling/article errors occurred in first production | 2026-09-13 |
| `trade-off between A and B` | chunk | general technical | 2026-09-14 | 1 day | Learner omitted `between`; fixed form needs active recall | 2026-09-13 |
| `bottleneck` | noun | performance / AI | 2026-09-16 | 3 days | Correctly retrieved in `The main bottleneck now is ...` | 2026-09-13 |
| `throughput` | noun | performance / systems | 2026-09-16 | 3 days | Correctly retrieved in a workflow bottleneck sentence; `workflow` spelling was corrected | 2026-09-13 |
| `nondeterministic` | adjective | debugging / systems | 2026-09-16 | 3 days | Correctly retrieved twice, including the final integrated task | 2026-09-13 |
| `increase parallelism` | chunk | performance / systems | 2026-09-14 | 1 day | Target phrase understood; learner omitted subject after `even if` | 2026-09-13 |
| `prioritize` | pronunciation / retrieval | speaking | deferred | next voice session | Pronunciation-specific review deferred during vocabulary-foundation phase | 2026-09-07 |

## Rules

- Due and overdue items normally come before new material.
- Recognition alone is not enough for mastery; prefer active recall or use in context.
- If recall fails, shorten the interval.
- If the learner uses the item naturally in a new context, extend the interval.
- For pronunciation items, use Voice evidence when available; do not infer pronunciation solely from transcript spelling.
