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

Listening remains the highest-priority skill, but **it should not be the first difficult activity**. At the current stage, essential vocabulary/chunks should usually be previewed before listening.

## Calibration-driven reset after 2026-09-07

The first Voice lesson was too difficult at the beginning. A natural technical paragraph of roughly 80–100 words produced near-total comprehension failure. Repetition alone did not help; the learner needed Chinese explanation and much shorter English.

Therefore the plan now uses **successive difficulty ladders plus vocabulary-first scaffolding** rather than assuming intermediate listening/speaking from CET scores.

### Listening: current starting level L0

- One short sentence at a time, typically 5–10 words.
- Mostly familiar/high-frequency words or words previewed immediately before the listening.
- At most one low-risk new word or chunk in the sentence.
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
- pre-listening vocabulary/chunk explanation,
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

### 2. Pre-listening vocabulary / chunks — 5–6 min

Preview roughly **2–4 essential items** needed for the day's listening.

For each item, normally give:
- the relevant Chinese meaning,
- one short natural example,
- a useful chunk/collocation when relevant.

Do not pre-teach every word. The target is to make the listening roughly **80–90% known or just-previewed language**, while leaving a small amount that can be inferred from context.

At the current level, this stage is important because the main bottleneck is not only speed; it is also recognizing word boundaries and retrieving vocabulary from audio.

### 3. Listening — 5–7 min

Highest-priority skill, but use the current L-level and the vocabulary just previewed.

At L0:
- 2–4 separate short sentences total,
- one simple question per sentence,
- immediate Chinese support when needed,
- optionally repeat the simplified sentence once.

Do not spend the whole block trying to force understanding of one sentence that is clearly above level.

### 4. Contextual language expansion — 4–5 min

Add or clarify useful items that emerged from the listening/fresh source so the whole lesson contains about **4–7 useful language items total**, including the pre-listening preview.

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

### 5. Technical writing / Prompt — 6–8 min

One realistic task, one first attempt, focused feedback, at most one revision.

Examples:
- rewrite a Chinese Agent instruction,
- describe a bug or workflow failure,
- write a constraint or acceptance criterion,
- summarize a technical point,
- compare two options,
- use 2–4 language items learned earlier in the session.

### 6. Reading / fresh input — 3–5 min

Reading comes before speaking.

Use one short passage/snippet or integrate reading into the vocabulary/writing stages. Reading should remain finite:
- one passage,
- 2–3 questions maximum,
- optionally one reuse task,
- then exit.

### 7. Speaking — 3–5 min, always last

Current default is S0–S1.

Use only one short task such as:
- repeat one chunk,
- say one short sentence from a Chinese cue,
- combine two already-practiced chunks,
- read and slightly adapt a sentence learned earlier.

Do not end a normal lesson with a demanding spontaneous monologue. If speaking becomes blocked, simplify once, record the issue, and stop.

### 8. Wrap-up

Briefly summarize:
- what was learned,
- important errors,
- what goes to review,
- next session's difficulty level.

Then update repository state.

## Voice delivery and accent policy

The learner reported two separate problems:

1. Chinese Voice had a noticeable regional accent that reduced comfort and sometimes intelligibility.
2. English Voice sounded less clear than exam-style listening or carefully presented YouTube speech.

Current operating rule: treat accent/style requests as **best-effort steering**, not a guaranteed accent lock.

### Chinese

- Request **clear Mainland Standard Mandarin / standard Putonghua**.
- Keep explanations concise and easy to parse.
- If a Voice continues to have a strong regional accent that harms comprehension, **switch to another Voice** rather than repeatedly trying to prompt the same Voice into a different accent.
- Do not assume any named Voice is guaranteed to remain perfectly standard in Mandarin.

### English at L0–L1

For learning audio, request:

- **clear General American English**,
- slower-than-casual delivery,
- clear articulation,
- one short sentence at a time,
- minimal `uh / um / hmm` fillers,
- minimal unnecessary hesitation,
- clearer word boundaries than normal casual conversation.

Do not intentionally use fast connected speech yet. As listening improves, gradually reintroduce natural reductions, linking, fillers, and faster YouTuber/conversational rhythm.

### Pronunciation reference

Do not treat free-form Voice output as the sole canonical pronunciation source for individual words.

For a specific word:
- prefer a controlled pronunciation card or another standard-pronunciation reference when available,
- use Voice mainly for sentence-level listening, guided repetition, and conversation,
- only record pronunciation problems that were actually heard/identified in Voice; do not infer pronunciation from transcript spelling alone.

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
- Listening: if comprehension collapses, simplify/translate and step down in difficulty rather than extending endlessly.
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

- reliable understanding of short L0 sentences after a small vocabulary preview,
- gradual progression to L1 without heavy rescue,
- ability to recognize and reuse common chunks from audio,
- more automatic use of `fewer`, `suggest + -ing`, `prioritize fixing`, and similar structures,
- ability to produce one short spoken sentence with less hesitation,
- technical writing that becomes more natural and concise,
- reading that remains interesting through fresh external topics rather than recycled chat history,
- reduced dependence on extremely slow/over-articulated English before gradually returning toward natural conversational speech.
