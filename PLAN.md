# Execution Plan

## Objective

Build a daily, interactive English-learning routine that normally takes about 30 minutes, can shrink to ~10 minutes when busy, can be postponed without penalty, and can expand when extra time is available.

The repository is the persistent source of truth. Scheduled or manual lessons should read repository state before starting and write progress back after completion.

## Current priority order

1. **Listening comprehension**
2. **Technical writing / prompting**
3. **Technical reading**
4. **Everyday speaking**

Speaking is intentionally last because the first Voice calibration showed that spontaneous speaking is currently much weaker than written production and becomes difficult when too much English is used before sufficient scaffolding.

## Calibration-driven reset after 2026-09-07

The first Voice lesson was too difficult at the beginning. A natural technical paragraph of roughly 80–100 words produced near-total comprehension failure. Repetition alone did not help; the learner needed Chinese explanation and much shorter English.

Therefore the plan now uses **successive difficulty ladders** rather than assuming intermediate listening/speaking from CET scores.

### Listening: current starting level L0

- One short sentence at a time, typically 5–10 words.
- Mostly familiar/high-frequency words.
- At most one new word or chunk in the sentence.
- One simple task only: identify a keyword, choose the meaning, or state the main idea.
- If the first attempt fails, simplify or explain in Chinese quickly instead of replaying a dense sentence several times.
- Move to longer material only after repeated successful sessions.

Progression:

- **L0:** 1 sentence / 5–10 words
- **L1:** 2–3 short sentences / 20–40 words
- **L2:** 40–80 words
- **L3:** 80–140 words natural technical/everyday speech

### Speaking: current starting level S0–S1

- **S0:** repeat a chunk, choose an expression, finish a sentence frame, produce 3–7 words.
- **S1:** produce one short sentence from Chinese or a visible scaffold.
- **S2:** two connected sentences with support.
- **S3:** 20–60 second guided explanation.
- **S4:** longer spontaneous conversation.

Do not jump to S3/S4 until short sentence retrieval is stable.

## Chinese / English policy

At the current stage, Voice should be **Chinese-led**.

Use Chinese for:
- explaining what the task is,
- vocabulary/grammar explanations,
- corrections,
- rescue after failed listening,
- stage transitions.

Use English for:
- the exact target listening sentence,
- short examples,
- learner output,
- gradually longer interaction as performance improves.

The goal is not to maximize English exposure at all costs. The goal is comprehensible input plus successful output. Increase English only when the learner can follow it.

## Default normal lesson (~30 min)

### 1. Retrieval review — 4–5 min

Use 2–3 due items from `state/review_queue.md`.

Preferred formats:
- Chinese -> English recall,
- choose between two expressions,
- cloze,
- error correction,
- short spoken recall if Voice is active.

### 2. Listening — 6–8 min

Highest-priority skill, but use the current L-level rather than natural technical paragraphs by default.

At L0:
- 2–4 separate short sentences total,
- one simple question per sentence,
- immediate Chinese support when needed,
- optionally repeat the simplified sentence once.

Do not spend the whole block trying to force understanding of one sentence that is clearly above level.

### 3. Contextual language — 6–7 min

Teach about **4–7 useful items** from the day's listening, fresh reading, learner errors, or output needs.

Use a mix of:
- words,
- phrases/collocations/chunks,
- sentence patterns,
- domain expressions.

Each item should normally include:
- the relevant Chinese meaning,
- a useful usage/collocation note when needed,
- at least one natural contextual example,
- one chance to reuse or retrieve it.

Examples should come from realistic AI/Agent/GitHub, Blender/3D, generative media, hardware/gaming, engineering, or everyday contexts.

### 4. Technical writing / Prompt — 7–8 min

One realistic task, one first attempt, focused feedback, at most one revision.

Examples:
- rewrite a Chinese Agent instruction,
- describe a bug or workflow failure,
- write a constraint or acceptance criterion,
- summarize a technical point,
- compare two options,
- use 2–4 language items learned earlier in the session.

### 5. Reading / fresh input — 3–5 min

Reading comes before speaking.

Use one short passage/snippet or integrate the reading into the contextual-language/writing stages. Reading should remain finite:
- one passage,
- 2–3 questions maximum,
- optionally one reuse task,
- then exit.

### 6. Speaking — 3–5 min, always last

Current default is S0–S1.

Use only one short task such as:
- repeat one chunk,
- say one short sentence from a Chinese cue,
- combine two already-practiced chunks,
- read and slightly adapt a sentence learned earlier.

Do not end a normal lesson with a demanding spontaneous monologue. If speaking becomes blocked, simplify once, record the issue, and stop.

### 7. Wrap-up

Briefly summarize:
- what was learned,
- important errors,
- what goes to review,
- next session's difficulty level.

Then update repository state.

## Quick / manual work-break session (~10–15 min)

Default to text-only unless audio is explicitly requested.

Use no more than 3 stages:

1. up to 2 review prompts,
2. one short fresh input/context + 2–4 useful words/phrases/patterns,
3. one active output task with at most one revision.

No speaking stage by default during work hours. Then stop and update state.

## Fresh-input strategy

History is used to infer interests and review targets, not to generate most new passages.

When web access is available:

1. find a fresh relevant article, release, tutorial, technical post, review, or news item,
2. prefer roughly the last 7–30 days for fast-moving AI/hardware topics,
3. use good evergreen sources for concepts/tutorials,
4. recompose the source into original learner-appropriate English,
5. keep facts and useful terminology,
6. avoid substantially repeating the same non-review topic for about 14 days when practical.

The key constraint is: **fresh information, but simplified enough for the current L-level**.

## Hard-stop rules

- One activity: at most 2 feedback/retry cycles by default.
- A follow-up question counts toward the same activity budget.
- Do not convert every error into another drill.
- Reading: one passage only unless explicitly planned otherwise.
- Writing: one task + at most one revision.
- Listening: if comprehension collapses, step down in difficulty rather than extending endlessly.
- Speaking: one short final task at current S-level.
- When planned stages are complete, end the lesson.

## Current concrete review targets from 2026-09-07

- `fewer bugs` rather than `less bugs`
- singular `version` when referring to one version
- `suggest fixing ...`
- `stability issues`
- `prioritize fixing ...`
- spelling of `stability`
- spoken retrieval/pronunciation of `prioritize`

These should be reviewed in new contexts rather than repeating the same Blender-release sentence.

## Scheduled-task behavior

Actual-workday evening: around 20:30.
Actual-rest-day lesson: around 12:00.

Open with only:

1. Normal ~30 min
2. Quick ~10 min
3. Postpone
4. Extra time

If Normal, Quick, or Extra is selected, begin immediately. If postponed, preserve the queue and do not record failure.

## Success criteria for the next 2–4 weeks

Before trying long spontaneous conversations, look for:

- reliable understanding of short L0 sentences,
- gradual progression to L1 without heavy rescue,
- ability to recognize and reuse common chunks from audio,
- more automatic use of `fewer`, `suggest + -ing`, `prioritize fixing`, and similar structures,
- ability to produce one short spoken sentence with less hesitation,
- technical writing that becomes more natural and concise,
- reading that remains interesting through fresh external topics rather than recycled chat history.
