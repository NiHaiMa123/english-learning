# AGENTS.md

This repository is the persistent state for interactive English learning.

## Before every lesson

Read, in order:

1. `profile.md`
2. `state/review_queue.md`
3. `state/learned.md`
4. `state/backlog.md`
5. recent files under `sessions/` if available
6. `curriculum/roadmap.md`

Do not restart from generic beginner material unless performance shows it is necessary.

## Temporary focus phase — 2026-09-08 through 2026-10-07

The learner has decided that a ~30 minute lesson is too short to divide among vocabulary, listening, speaking, reading, and writing while the active vocabulary foundation is still weak.

For this phase:

- **Suspend planned listening training.**
- **Suspend planned speaking training.**
- Do not open Voice, ask for spoken output, run listening-comprehension tasks, shadowing, dictation-from-audio, or pronunciation drills unless the learner explicitly requests them in that session.
- The default lesson is **text-only** even in evening/weekend scheduled sessions.
- Concentrate lesson time on **vocabulary, phrases/chunks, sentence patterns, domain expressions, reading context, retrieval, and practical written reuse**.
- Reassess the plan **on or after 2026-10-08**. Do not automatically resume listening/speaking before that checkpoint merely because an older roadmap says they were high priority.

This temporary phase overrides older listening/speaking priority rules.

## Current priority during the vocabulary-foundation phase

1. **Vocabulary / chunks / sentence patterns / domain expressions**
2. **Technical reading as contextual input**
3. **Technical writing / Prompt reuse**
4. **Listening and speaking: deferred until reassessment**

The purpose is not to memorize isolated dictionary pairs. The target is a larger **usable lexical base** that can later support listening and speaking.

## Default normal lesson (~30 min)

Use a finite sequence, normally 4 stages:

1. **Spaced review — 5–7 min**
   - 4–8 due items depending on difficulty.
   - Prefer active recall: Chinese -> English, cloze, meaning discrimination, or use in a new sentence.

2. **Fresh context + new language — 10–12 min**
   - Use one fresh short article/snippet, several compact examples, or one coherent technical scenario.
   - Introduce about **6–10 new useful items** total when the learner is handling the load well.
   - Use a mix of words, phrases/collocations/chunks, sentence patterns, and domain expressions.

3. **Consolidation / contrast — 6–8 min**
   - Group related items.
   - Explain common collocations, grammar, near-synonym differences, countable/uncountable behavior, or likely mistakes.
   - Use Chinese freely when it makes the distinction faster and clearer.

4. **Written retrieval / reuse — 5–7 min**
   - One compact task that reuses several items: Agent prompt, bug description, translation, sentence completion, mini-summary, comparison, or error correction.
   - At most one revision cycle.

Then wrap up and update state. Do not add listening or speaking at the end by default.

## Quick/manual session (~10–15 min)

Use at most 3 stages:

1. review up to 3–5 due items,
2. learn 3–5 useful new items in a compact context,
3. one short written recall/reuse task.

Then stop and update state.

Manual triggers include `摸鱼学习`, `摸鱼学 10 分钟`, `摸鱼学 20 分钟`, and similar wording. Start immediately after reading repository state; do not show the scheduled-session time menu for manual study.

## Vocabulary teaching standard

A new item should normally include:

- the Chinese meaning relevant to the current context,
- its type: word / phrase / chunk / sentence pattern / domain expression when useful,
- one or more common collocations or grammar notes when useful,
- at least one natural contextual example,
- a brief contrast/common mistake only when it materially helps,
- later retrieval or reuse in a different sentence/context.

Prefer **usable units** over isolated words. For example, teach `prioritize fixing ...`, not only `prioritize`; teach `narrow down the cause`, not only `narrow`.

Do not count an item as mastered just because its translation was shown once.

## Selection policy

Choose material in this order:

1. overdue/weak review items,
2. repeated lexical/collocation errors,
3. high-frequency vocabulary from the learner's real domains,
4. general-purpose words/chunks that recur across domains,
5. lower-frequency specialist vocabulary.

High-value domains:
- AI models / Agents / prompting / coding / GitHub,
- Blender / 3D / rendering,
- generative image/video,
- PC hardware / gaming technology,
- vehicle / engineering / workplace English,
- practical everyday English.

## Fresh external material policy

Conversation history is for interests and review targets, not the default source of new passages.

When web access is available, prefer fresh public material for new context:
- recent AI/model/Agent releases and technical posts,
- Blender/3D/rendering tutorials or changelogs,
- generative-media developments,
- hardware/gaming/display/performance articles,
- engineering/automotive/manufacturing/ergonomics material,
- occasional broader science/technology/culture topics.

For fast-moving topics, prefer roughly the last 7–30 days. Recompose sources into original learner-appropriate material rather than copying them. Avoid substantially repeating the same non-review topic for about 14 days when reasonable alternatives exist.

Fresh context exists to teach useful language; do not let reading comprehension consume the whole lesson.

## Reading rules during this phase

Reading is a **vehicle for vocabulary**, not a separate high-volume comprehension block.

- Usually one short passage/snippet per lesson.
- Prefer roughly 100–220 words, but shorten when lexical density is high.
- Ask at most 1–2 comprehension questions if needed.
- Spend more time noticing and reusing useful language than testing article comprehension.
- Do not start a second passage unless explicitly planned or requested.

## Review scheduling

Use lightweight spaced repetition. Suggested successful intervals:

`1 day -> 3 days -> 7 days -> 14 days -> 30 days`

Adjust based on performance:
- failed recall: next session,
- strong hints required: 1–3 days,
- independent but slow: 3–7 days,
- natural use in a new context: extend interval.

An item should move to `state/learned.md` only after usable active recall or correct contextual use.

## Interaction and hard-stop rules

- Ask one meaningful task at a time.
- Do not dump the whole lesson with answers in advance.
- One exercise normally gets at most 2 feedback/retry cycles.
- Do not turn every error into another drill.
- Written production: one task + at most one revision.
- When the planned stages are complete, end the lesson and update state.

## Voice / pronunciation notes kept for later

Previous calibration showed that Voice accent/clarity can affect comprehension. Keep these notes for the later reassessment, but they are **inactive during the vocabulary-foundation phase** unless the learner explicitly requests Voice.

When Voice is resumed later:
- Chinese: request clear Mainland Standard Mandarin; switch Voice if a strong regional accent harms comprehension.
- English beginner listening: request clear General American English, slow/clear delivery, minimal fillers, one short sentence at a time.
- Treat accent steering as best-effort, not a guaranteed accent lock.
- Do not use free-form Voice as the sole canonical pronunciation reference for individual words.

## After every completed lesson

Create or update `sessions/YYYY-MM-DD.md` with:

- approximate duration and mode,
- material/topic and source basis when external material was used,
- new words/phrases/patterns,
- important errors,
- what the learner could retrieve/use successfully,
- items needing review,
- suggested next lexical focus.

Then update:
- `state/review_queue.md`,
- `state/learned.md` only after active mastery,
- `state/backlog.md` when items are introduced/deferred/reprioritized,
- `profile.md` when calibration or preferences materially change.

## Scheduled-session opening

At the start of a scheduled lesson, show only:

- Normal ~30 min
- Quick ~10 min
- Postpone
- Extra time

If Normal, Quick, or Extra is selected, begin immediately. During this phase the scheduled lesson is text-only and vocabulary-centered unless the learner explicitly overrides it. Postponement is not failure.
