# Execution Plan

## Objective

Build a daily, interactive English-learning routine that normally takes about 30 minutes, can shrink to ~10 minutes when busy, can be postponed without penalty, and can expand when extra time is available.

The repository is the persistent source of truth. Scheduled or manual lessons should read repository state before starting and write progress back after completion.

## Temporary one-month focus

Effective **2026-09-08 through 2026-10-07**, suspend planned listening and speaking practice and use the available lesson time to strengthen the lexical foundation first.

Reassess the plan **on or after 2026-10-08**.

During this phase:

1. **Vocabulary / chunks / sentence patterns / domain expressions** are the main target.
2. **Technical reading** supplies fresh context.
3. **Technical writing / prompting** is used to force active retrieval and reuse.
4. **Listening and speaking are deferred**, not abandoned permanently.

Do not automatically reintroduce Voice, listening passages, spoken output, shadowing, or pronunciation drills before the reassessment date unless the learner explicitly asks for them.

## Why this reset was made

The first multimodal lesson showed that dividing ~30 minutes among listening, vocabulary, writing, reading, and speaking made every component too shallow. Listening also exposed a limited active lexical base: many words that may be familiar in writing were not readily accessible enough to support audio comprehension.

The immediate goal is therefore to increase the amount of English that is **known well enough to recognize and retrieve**, so later listening/speaking practice has better input to work with.

## Default normal lesson (~30 min)

### 1. Spaced review — 5–7 min

Review roughly **4–8 due items**, depending on difficulty.

Preferred formats:
- Chinese -> English recall,
- cloze,
- choose between near-synonyms/collocations,
- correct an unnatural phrase,
- use an old item in a new domain/context.

### 2. Fresh context + new vocabulary — 10–12 min

Use one short fresh article/snippet, compact technical scenario, changelog excerpt, explanation, or set of connected examples.

Target about **6–10 new useful items** in a normal lesson when retention remains reasonable.

Use a mix of:
- individual words,
- phrases/collocations/chunks,
- reusable sentence patterns,
- technical/domain expressions.

Prefer units that can be reused directly in writing later.

### 3. Consolidation and distinctions — 6–8 min

Group related items and clarify:
- common collocations,
- grammar patterns,
- countable vs uncountable usage,
- near-synonym differences,
- register,
- common learner mistakes.

Use Chinese freely where it improves speed and clarity.

### 4. Written retrieval / practical reuse — 5–7 min

One compact output task using several of today's items, for example:
- rewrite an Agent instruction,
- complete a concise bug report,
- translate a technical observation,
- summarize a short article,
- compare two tools/options,
- correct several unnatural sentences.

One first attempt + focused feedback + at most one revision.

Then end and write state. **No default listening or speaking stage.**

## Quick / manual session (~10–15 min)

Use at most 3 stages:

1. review 3–5 due items,
2. learn 3–5 new useful items in one compact context,
3. one short written recall/reuse task.

Then stop and update state.

## What counts as “vocabulary”

The goal is not a large list of isolated translations.

Prefer this hierarchy:

1. **reusable chunks/collocations** — e.g. `narrow down the cause`, `meet the acceptance criteria`, `prioritize fixing ...`
2. **sentence patterns** — e.g. `The issue is not X; it's Y.`
3. **domain expressions** — e.g. `frame-time spike`, `weight painting`, `prompt adherence`
4. **individual words** when they are independently high-value.

For each new item, normally include:
- relevant Chinese meaning,
- usage/collocation or grammar note when useful,
- at least one natural example,
- one later retrieval/reuse opportunity.

## Fresh-input strategy

Use conversation history for interests and review targets, not as the default source of new passages.

When web access is available:

1. find a fresh relevant article, release, tutorial, technical post, review, or news item,
2. prefer roughly the last 7–30 days for fast-moving AI/hardware topics,
3. use strong evergreen material for concepts/tutorials,
4. recompose the source into original learner-appropriate English,
5. preserve useful terminology and facts,
6. avoid substantially repeating the same non-review topic for about 14 days when practical.

High-value source domains:
- AI models / Agents / coding / GitHub,
- Blender / 3D / rendering,
- image/video generation,
- GPU/display/game technology,
- engineering/automotive/workplace English,
- occasional general technology/science/practical English.

## Reading policy during this phase

Reading exists primarily to **supply vocabulary in context**.

- Normally one short passage/snippet.
- Rough target: 100–220 words, adjusted for lexical density.
- At most 1–2 comprehension questions when needed.
- Do not spend most of the lesson testing article comprehension.
- Extract useful language, then move to retrieval/reuse.

## Review and mastery

Suggested successful review intervals:

`1 day -> 3 days -> 7 days -> 14 days -> 30 days`

Shorten after failed recall; extend after natural use in a new context.

An item should enter `state/learned.md` only after the learner can actively retrieve or correctly use it in context. Recognition of a Chinese translation is not enough.

## Current carry-over review targets

From 2026-09-07:
- `fewer bugs` rather than `less bugs`
- singular `version` when referring to one version
- `suggest fixing ...`
- `stability issues`
- `prioritize fixing ...`
- spelling of `stability`

The spoken-pronunciation target for `prioritize` is deferred until listening/speaking returns. Written retrieval of `prioritize` may still be reviewed.

## Hard-stop rules

- Ask one meaningful task at a time.
- One exercise normally receives at most 2 feedback/retry cycles.
- Do not turn every mistake into another drill.
- One reading passage unless explicitly planned otherwise.
- One written production task + at most one revision.
- End after the planned stages and update state.

## Scheduled-task behavior

Actual-workday evening: around 20:30.
Actual-rest-day lesson: around 12:00.

Open with only:

1. Normal ~30 min
2. Quick ~10 min
3. Postpone
4. Extra time

During 2026-09-08 through 2026-10-07, Normal/Quick/Extra sessions are **text-only and vocabulary-centered by default**. Do not start Voice or listening/speaking merely because the session occurs in the evening or on a rest day.

## Reassessment checkpoint — 2026-10-08

At or after this checkpoint, review roughly one month of session/state data before deciding what to add back.

Evaluate:
- number of items introduced vs actually retained,
- active recall rate from `state/review_queue.md`,
- ability to use chunks naturally in Prompt/writing tasks,
- reading speed and unknown-word density,
- whether the learner feels the lexical bottleneck has eased.

Only then decide whether to:
- continue vocabulary-first,
- reintroduce very short listening,
- reintroduce speaking later,
- or rebalance the 30-minute lesson in another way.

Do not assume listening and speaking must both return at the same time.
