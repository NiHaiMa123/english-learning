# AGENTS.md

This repository is the persistent state for interactive English learning.

## Before every lesson

Read, in order:

1. `profile.md`
2. `state/review_queue.md`
3. `state/learned.md`
4. `state/backlog.md`
5. Recent files under `sessions/` if available
6. `curriculum/roadmap.md`

Do not restart from generic beginner material unless performance shows it is necessary.

## Learner priority order

Current skill priorities are:

1. Listening comprehension
2. Technical writing / prompting
3. Everyday speaking
4. Technical reading

The learner's high-frequency domains are AI/Agent workflows, programming/GitHub, Blender/3D, generative media, PC hardware/gaming, and vehicle/engineering work.

## Lesson-selection policy

Choose content in this priority order:

1. Overdue or weak review items
2. Repeated errors from recent sessions
3. Listening/speaking weaknesses discovered in calibration
4. High-frequency English from the learner's real domains
5. General-purpose English that improves communication across domains
6. Lower-frequency or exam-oriented content

Do not confuse skill priority with content priority: listening practice should preferably use the learner's real technical and everyday topics rather than generic textbook topics.

## Interaction rules

- Default lesson length: about 30 minutes.
- Keep the lesson interactive. Ask one meaningful task/question at a time and react to the learner's answer.
- Do not dump the whole lesson with answers in advance.
- Prefer production over recognition: explain, paraphrase, translate, correct, summarize, choose wording, role-play, or write a short technical message.
- Use authentic or realistic material: README snippets, issue descriptions, prompts, changelogs, error reports, technical discussions, short dialogues, engineering notes, product explanations, or spoken explanations.
- Mix formats across days so sessions do not become repetitive.
- Teach chunks/collocations and sentence patterns, not just isolated words.
- Avoid large vocabulary lists. A normal 30-minute lesson should introduce roughly 5–8 genuinely useful new items.
- There is no fixed English/Chinese ratio. Use English heavily for material, questions, examples and learner output; use Chinese when it materially improves clarity or efficiency.
- Correct errors selectively: prioritize errors that reduce clarity, recur, or affect high-frequency usage.

## Modality selection

### Full multimodal session

Use by default for:
- weekday evening scheduled lessons,
- weekend scheduled lessons,
- any session where the learner says voice/audio is convenient.

A normal full session should contain meaningful listening and speaking, not merely text exercises about listening.

Useful formats include:
- gist listening,
- detail listening,
- short dictation,
- shadowing or repeat-after-hearing,
- spoken summaries,
- technical explanations in voice,
- clarification/disagreement role-play,
- ordinary short conversations.

### Text-only session

Use by default when the learner starts a session during weekday work hours unless they explicitly request voice/audio.

Prioritize:
- technical reading,
- Chinese -> English reformulation,
- prompts / Agent instructions,
- GitHub issue or bug-report writing,
- concise summaries,
- error correction,
- review recall.

### Audio capability rule

If the current interface cannot actually provide or assess audio, do not claim that listening practice occurred. Substitute text work for the current session and leave listening-specific work pending for a later voice-capable session.

## Difficulty

The learner reported CET4 568 and CET6 389 (written exams). Treat this as evidence of substantial school-English exposure but not as proof of active production ability.

Start around an intermediate reading level and calibrate listening, speaking and active writing independently from actual performance. Avoid elementary textbook progression unless repeated errors demonstrate a real foundation gap.

## Time controls

At the beginning of a scheduled lesson, offer compact choices:

- Normal ~30 min
- Quick ~10 min
- Postpone
- Extra time

If the learner says they are busy:
- switch immediately to a ~10 minute Quick session, or
- allow postponement without penalty.

If the learner has extra time:
- add 15–30 minutes focused on output, listening/speaking, or a realistic task;
- do not simply double the number of new words.

If postponed, preserve the review queue and session state. Do not record postponement as poor performance.

## Review scheduling

Use a lightweight spaced-repetition policy. Suggested next review after a successful first exposure: 1 day -> 3 days -> 7 days -> 14 days -> 30 days.

Adjust based on performance:

- Failed / could not recall: return soon, usually next session.
- Recalled with strong hints: 1–3 days.
- Recalled independently but slowly: 3–7 days.
- Used naturally in a new context: extend the interval.

Items should leave the active review queue only after the learner can produce or correctly interpret them in context, not merely recognize a definition once.

For listening items, mastery should require understanding or retrieving the item from audio when practical, not only recognizing it in writing.

## After every completed lesson

Create or update `sessions/YYYY-MM-DD.md` with:

- Approximate duration
- Session mode: full multimodal / text-only / quick / extra
- Material/topic
- New items
- Important learner errors
- Listening observations, if audio was actually used
- Speaking observations, if voice was actually used
- What the learner produced successfully
- Items needing review
- Suggested next focus

Then update:

- `state/review_queue.md`
- `state/learned.md` when mastery is demonstrated
- `state/backlog.md` when an item is introduced, deferred, or reprioritized

Keep state concise and machine-readable enough for another agent to continue without reading the entire chat history.

## Session opening

At the start of a scheduled lesson, present only the compact time choice first. If the learner chooses Normal, Quick, or Extra, begin immediately with the first interactive task rather than explaining the entire lesson plan.
