# Execution Plan

## Objective

Build a daily, interactive English-learning routine that normally takes about 30 minutes, can shrink to ~10 minutes when busy, can be postponed without penalty, and can expand when extra time is available.

The repository is the persistent source of truth. A scheduled GPT task should read repository state before each lesson and write progress back after the lesson.

## Daily lesson flow (~30 min)

### 1. Review — 5 min
Use due items from `state/review_queue.md`.

Preferred formats:
- Chinese -> English recall
- cloze
- error correction
- choose between near-synonyms and explain why
- use a target phrase in a new technical sentence

### 2. Realistic input — 7 min
Use one short piece of realistic English, such as:
- README or issue-style text
- Agent instruction
- Blender tutorial excerpt
- model/release note
- hardware review paragraph
- engineering note
- short dialogue

Ask 2–4 comprehension questions. Avoid dictionary-style teaching before the learner attempts the text.

### 3. New language — 7 min
Select about 5–8 high-value items from the input.

Prefer:
- collocations
- reusable sentence patterns
- technical terms that recur in the learner's real activities
- distinctions that prevent common mistakes

### 4. Production — 8 min
Require meaningful output. Rotate formats:
- rewrite a Chinese Agent instruction in English
- explain a bug or workflow failure
- summarize a technical passage
- critique a generated image/video result
- describe a Blender pose/rendering problem
- compare hardware options
- translate an engineering observation
- role-play clarification/disagreement

### 5. Wrap-up — 3 min
- Correct only important errors.
- Ask for one final recall or mini-summary.
- Update the session log and review queue.

---

## First 7 completed sessions

This is a starting sequence, not a rigid calendar.

### Session 1 — Diagnostic: Agent / GitHub English
Goal: measure reading comprehension and active technical expression.

- Read a ~180–250 word issue/README-style passage.
- Answer comprehension questions.
- Explain the issue in 3–5 English sentences.
- Test high-value chunks such as `reproduce`, `expected behavior`, `constraint`, `workaround`, `root cause`.
- End with a short Chinese -> English Agent instruction.

### Session 2 — Diagnostic: Technical instruction writing
Goal: measure Chinese -> English production.

- Convert 4–6 realistic Chinese instructions into English.
- Include sequencing, constraints, acceptance criteria, and exceptions.
- Identify repeated issues in articles, tense, word choice, sentence structure, or technical collocation.

### Session 3 — Diagnostic: Blender / generative-media explanation
Goal: measure ability to explain visual/technical problems.

- Read a short Blender/rendering or video-generation passage.
- Explain a realistic problem such as IK, retargeting, temporal consistency, frame interpolation, or seamless looping.
- Optional short speaking task if voice practice is enabled.

### Session 4 — Agent debugging language
Focus:
- isolate the issue
- narrow down
- reproduce consistently
- regression
- edge case
- fallback
- root cause

Output: write a concise bug report or debugging instruction.

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

### Session 6 — General practical communication
Focus on reusable discourse:
- What I mean is ...
- The issue is not X; it's Y.
- My concern is that ...
- This seems inconsistent with ...
- Could you verify ...?

Output: clarification/disagreement role-play.

### Session 7 — Review + hardware/engineering mix
- Review all due items.
- Short new input from hardware/gaming or vehicle engineering.
- Use technical comparison language and quantities/tolerances.
- Reassess which track should dominate the next week.

---

## Difficulty policy

Initial assumption: intermediate reading ability with uneven active production.

Adjust dynamically:
- If comprehension is >90% and output is easy, increase density and reduce Chinese support.
- If comprehension is good but production is weak, keep input difficulty but increase guided output.
- If vocabulary blocks comprehension, reduce input difficulty and reinforce high-frequency chunks.
- Do not return to elementary textbook progression unless recurring errors show a real foundation gap.

## Content mix

Across roughly 7 completed sessions:

- 2–3: AI/Agent/coding/GitHub
- 1–2: Blender/3D/generative media
- 1: hardware/gaming or engineering
- 1: general practical English / mixed review

The review queue overrides this mix when necessary.

## Scheduled-task behavior

The scheduled task should open with four options:

1. Start normal ~30 min
2. Quick ~10 min
3. Postpone
4. I have extra time

If normal/quick/extra is selected, begin immediately.

If postponed, ask for a later time and preserve the queue. Skipping or postponing must not be marked as poor learning performance.

### Suggested scheduled-task prompt

> Open the GitHub repository `NiHaiMa123/english-learning`. Read `AGENTS.md`, `profile.md`, the state files, and recent session logs. Start today's interactive English-learning session according to the repository rules. First offer Normal ~30 min / Quick ~10 min / Postpone / Extra time. Do not dump the full lesson at once; teach interactively and update the repository state after the session.

## Success criteria after 4–6 weeks

The learner should show measurable improvement in:

- reading technical English without translating every sentence,
- writing precise Agent prompts/instructions directly in English,
- explaining bugs and trade-offs naturally,
- understanding recurring Blender/AI/hardware terminology,
- retrieving learned chunks actively rather than only recognizing them,
- producing concise English summaries of familiar technical topics.
