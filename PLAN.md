# Execution Plan

## Objective

Build a daily, interactive English-learning routine that normally takes about 30 minutes, can shrink to ~10 minutes when busy, can be postponed without penalty, and can expand when extra time is available.

The repository is the persistent source of truth. A scheduled GPT task should read repository state before each lesson and write progress back after the lesson.

Current skill priority:

1. Listening comprehension
2. Technical writing / prompting
3. Everyday speaking
4. Technical reading

The content itself should remain strongly tied to the learner's real domains: AI/Agents/coding/GitHub, Blender/3D, generative media, PC hardware/gaming, engineering/workplace English, plus practical everyday conversation.

## Default full lesson (~30 min)

### 1. Retrieval review — 5 min
Use due items from `state/review_queue.md`.

Preferred formats:
- Chinese -> English recall
- spoken recall when voice is available
- cloze
- error correction
- choose between near-synonyms and explain why
- use a target word/phrase/pattern in a new technical or everyday sentence

### 2. Listening — 8 min
This is the highest-priority skill and should appear in most full multimodal sessions.

Rotate formats:
- gist: identify the main point without transcript support
- details: numbers, constraints, causes, comparisons, sequence
- short dictation
- identify a phrase from audio and reuse it
- listen -> summarize in English or Chinese
- listen -> answer a realistic follow-up question

Use technical and practical everyday topics rather than generic exam listening whenever possible.

### 3. Contextual language learning — 5–7 min
Select about **4–7 genuinely useful new language items** from the day's listening, reading, learner errors, or output needs.

Use a mix of:
- **words**,
- **phrases / collocations / chunks**,
- **sentence patterns**,
- **domain expressions**.

Prefer phrases/chunks and reusable sentence patterns over isolated vocabulary when possible.

Each item should normally include:
- the meaning relevant to the current situation,
- a useful collocation or grammar note when needed,
- **at least one natural contextual example**,
- a brief contrast/common mistake only when useful,
- one chance to retrieve or use it.

Examples should be tied to realistic contexts such as AI/Agent instructions, GitHub/debugging, Blender/3D, hardware/gaming, engineering, or ordinary conversation.

Do not teach items only as dictionary pairs such as `constraint = 约束`. Prefer something like:

- `constraint` — the limitation/condition that restricts what can be done
- `under this constraint`, `hardware constraint`
- `Do not change the production code; treat that as a hard constraint.`
- `VRAM is the main constraint when rendering this scene at 4K.`

For a sentence pattern, teach the reusable frame plus contextual examples, for example:

- `The issue is not X; it's Y.`
- `The issue is not model capability; it's the way the harness provides context.`
- `The issue is not average FPS; it's the frame-time spikes.`

Do not create one separate drill for every item. Several items can be reused together in the production task.

### 4. Technical writing / active production — 7 min
Rotate realistic outputs:
- rewrite a Chinese Agent instruction in English
- write constraints and acceptance criteria
- explain a bug or workflow failure
- summarize a technical point
- critique generated image/video output
- describe a Blender pose/rendering problem
- compare hardware options
- translate an engineering observation
- use 2–4 of today's new words/phrases/patterns naturally in one task

### 5. Speaking + wrap-up — 4–5 min
When voice is available:
- 2–4 minute role-play, spoken summary, clarification, disagreement, or technical explanation
- reuse one or more new chunks naturally
- one focused fluency/pronunciation correction if useful

Then:
- correct only important recurring errors,
- do one final retrieval check,
- update the session log and review queue.

If audio/voice is unavailable, convert this block to writing/reading and leave audio-specific targets pending.

## Finite-stage execution rules

The time blocks above are not invitations to continue one exercise until it feels complete. Each block has a hard activity budget.

Default caps for a full lesson:

- review: 2–3 prompts total,
- listening: one spoken item, at most two passes, at most 3 comprehension prompts,
- contextual language: 4–7 items total,
- writing/Prompt: one task, one first attempt, focused feedback, at most one revision,
- speaking: one short segment with focused correction,
- then wrap up.

A single activity should normally receive no more than 2 feedback/retry cycles. Unresolved errors go into the review queue instead of extending the current activity indefinitely.

### Reading-comprehension exit condition

A reading block is complete after:

1. one passage/snippet,
2. 2–3 comprehension questions total,
3. concise correction,
4. optionally one short reuse/output task.

Then the lesson **must leave the reading block**. Do not generate more comprehension questions, a second passage, or another reading set unless it was explicitly planned or the learner asks to continue reading.

Poor performance is evidence for future review, not a reason to trap the learner in the same block.

### Language-learning exit condition

A contextual language block is complete after:

1. 4–7 items in a normal lesson or 2–4 in a quick/manual lesson,
2. brief contextual explanation/examples,
3. one compact recall/reuse activity, possibly combining several items.

Then move on. Do not expand into an open-ended vocabulary list or drill every item repeatedly in the same session.

### Quick/manual session exit condition

A ~10–15 minute `摸鱼学习` session should normally contain at most 3 stages:

1. up to 2 review prompts,
2. one short input/context block plus **2–4 useful words/phrases/patterns** drawn from it,
3. one active output task using at least one of those items, with at most one revision.

Then end the session, summarize briefly, and update state. If the learner says they have more time, expand deliberately; do not expand automatically.

### Progress marker

A compact marker such as `2/4 · Context & phrases` or `3/4 · Prompt` may be shown so the learner can see that the lesson is progressing toward an end.

---

## Quick session (~10 min)

Designed for a busy day or daytime work break.

- 2–3 min: due review
- 3–4 min: one short realistic input/context + 2–4 language items
- 3–4 min: one active output task that reuses at least one new item

During weekday work hours, default to text-only reading/writing unless the learner explicitly requests voice/audio.

## Extra-time session (+15–30 min)

Add one substantial activity rather than a large vocabulary dump:

- longer listening with no transcript first
- voice role-play
- shadowing / repeat-after-hearing
- technical video-style explanation
- realistic GitHub/Agent writing task
- longer Blender/AI/hardware discussion
- mixed comprehension + summary task
- contextual reuse of already-learned words/phrases in a new domain

---

## First 7 completed sessions

This is a starting sequence, not a rigid calendar.

### Session 1 — Diagnostic: listening + AI/Agent English
Goal: measure listening comprehension before overfitting the plan to CET written scores.

- Short spoken explanation about an AI/Agent or debugging scenario.
- First pass: gist only, no transcript.
- Second pass: details and key phrases.
- Teach 3–5 high-value words/chunks from the material with contextual examples.
- Give a short spoken or written summary.
- End with one Chinese -> English Agent instruction using one or more of the new items.

Measure:
- gist comprehension
- detail retention
- dependence on transcript/subtitles
- ability to reuse heard language

### Session 2 — Diagnostic: technical instruction writing
Goal: measure Chinese -> English production.

- Convert realistic Chinese instructions into English within the activity budget.
- Include sequencing, constraints, acceptance criteria, and exceptions.
- Extract useful words/chunks/sentence patterns from the learner's needs or errors.
- Identify repeated issues in articles, tense, word choice, sentence structure, or technical collocation.
- Include a short read-aloud or spoken explanation if voice is available.

### Session 3 — Diagnostic: speaking + Blender / generative media
Goal: measure spontaneous explanation and repair strategies.

- Explain a familiar problem such as IK, retargeting, temporal consistency, frame interpolation, or seamless looping.
- Ask follow-up questions within the stage cap that require clarification, correction, comparison, and uncertainty.
- Teach useful technical chunks or sentence patterns that improve the explanation.
- Add one short listening segment in the same domain.

### Session 4 — Agent debugging language
Focus:
- isolate the issue
- narrow down
- reproduce consistently
- regression
- edge case
- fallback
- root cause

Output: concise bug report or debugging instruction, plus short spoken explanation if practical.

### Session 5 — Blender / 3D language
Focus:
- rig / armature
- IK
- retargeting
- skinning / weight painting
- camera framing
- focal length
- roughness / metallic

Output: describe a desired pose/render setup or diagnose a rigging problem.

### Session 6 — Practical conversation
Focus on reusable spoken discourse:
- What I mean is ...
- The issue is not X; it's Y.
- My concern is that ...
- This seems inconsistent with ...
- Could you verify ...?
- I'm not sure whether ...

Output: clarification/disagreement role-play.

### Session 7 — Integrated review + hardware/engineering
- Review all due items.
- Short listening or reading input from hardware/gaming or vehicle engineering.
- Learn/review several contextual words, phrases, or sentence patterns from that material.
- Use comparison, quantities, tolerances, and cause/effect language.
- Reassess next-week balance from actual performance.

---

## Difficulty policy

Initial assumption: substantial school-English exposure with unknown listening/speaking strength and uneven active production.

Adjust each skill separately:

- If reading comprehension is >90% and easy, increase density rather than assigning more elementary reading.
- If listening gist is good but details are weak, keep topic difficulty and increase detail-focused passes.
- If listening collapses without subtitles, reduce speech density/speed and train chunk recognition before increasing difficulty.
- If writing is understandable but unnatural, focus on collocations and concise technical phrasing rather than basic grammar drills.
- If speaking is slow but accurate, train retrieval and repair strategies before adding harder grammar.
- If isolated words are recognized but cannot be produced, shift toward chunks, sentence patterns, and contextual recall.
- Do not return to elementary textbook progression unless recurring errors show a genuine foundation gap.

## Content balance

Skill weighting and topic weighting are separate.

Across most weeks:
- listening should appear in most full sessions,
- technical writing/prompting should appear several times per week,
- speaking should appear regularly in evening/weekend voice-capable sessions,
- reading supports all tracks but does not need to dominate dedicated lesson time,
- contextual vocabulary/phrase/sentence learning should appear in virtually every completed session.

Topic rotation across roughly 7 completed sessions:
- 2–3: AI/Agent/coding/GitHub
- 1–2: Blender/3D/generative media
- 1: hardware/gaming or engineering
- 1: practical everyday English / mixed review

The review queue overrides this mix when necessary.

## Scheduled-task behavior

Weekday scheduled lesson: after 20:00, target around 20:30.
Weekend/actual rest-day scheduled lesson: around 12:00.

The task should open with four options:

1. Normal ~30 min
2. Quick ~10 min
3. Postpone
4. Extra time

If Normal, Quick, or Extra is selected, begin immediately and interactively.

If postponed, preserve the queue and do not record a failed session. The learner may reschedule for later that day.

### Scheduled-task prompt

Open the GitHub repository `NiHaiMa123/english-learning`. Read `AGENTS.md`, `profile.md`, state files, `curriculum/roadmap.md`, and recent session logs. Start today's interactive English lesson according to repository rules. First offer Normal ~30 min / Quick ~10 min / Postpone / Extra time. Do not dump the lesson at once. Use actual audio/voice for listening only when the current interface supports it; otherwise substitute text work and keep listening items pending. Ensure the session includes a small contextual set of useful words/phrases/sentence patterns and at least one chance to reuse them. After a completed session, update the repository state and session log.

## Success criteria after 4–6 weeks

Look for measurable improvement in:

- understanding short English technical explanations without transcript dependence,
- retaining details from spoken English,
- writing precise Agent prompts/instructions directly in English,
- explaining familiar technical problems more spontaneously,
- using clarification and repair strategies in conversation,
- reading technical English without translating every sentence,
- retrieving learned words, chunks, collocations, and sentence patterns actively rather than merely recognizing them,
- reusing learned language naturally in new contexts instead of only remembering the original example.
