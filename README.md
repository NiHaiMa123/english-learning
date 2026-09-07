# English Learning System

A persistent, agent-driven English learning repository.

The goal is not to follow a CET textbook from chapter 1. The system should prioritize English that the learner is likely to use in real life: AI/Agent workflows, programming and GitHub, Blender/3D, image/video generation, PC hardware/gaming, engineering work, and practical everyday English.

## Default daily session

Target duration: **30 minutes**.

A normal session should contain:

1. **Recall — 5 min**  
   Review due items from `state/review_queue.md`. Prefer active recall, cloze, translation, correction, or short production over recognition-only questions.

2. **Input — 7 min**  
   A short, realistic passage/dialogue/issue/README excerpt related to a high-priority domain. Keep it understandable but slightly above the learner's comfortable level.

3. **New language — 7 min**  
   Teach roughly 5–8 useful words, collocations, sentence patterns, or discourse chunks from the input. Prioritize reusable chunks rather than isolated vocabulary.

4. **Output — 8 min**  
   Require the learner to use the material: rewrite a prompt, explain a bug, summarize a technical choice, translate a real sentence, role-play a discussion, or answer follow-up questions.

5. **Wrap-up — 3 min**  
   Correct important errors, record what was learned, and schedule review.

## Time modes

- **Core:** ~30 min.
- **Quick:** ~10 min when busy. Do due review + one small production task. Do not introduce more than 2–3 new items.
- **Extended:** add 15–30 min when the learner has extra time. Prefer deeper output, listening/speaking, or an additional real-world task rather than doubling vocabulary.
- **Postpone:** if the learner says there is no time, do not treat it as failure. Let them choose a later time and keep the review queue intact.

## Learning priorities

Initial priority order, subject to diagnostic results:

1. AI / Agent / coding / GitHub English
2. Blender / 3D / rendering / generative-media English
3. PC hardware / gaming technology English
4. Engineering/workplace English
5. Practical general English
6. Exam-style English only when it supports the above goals

## State model

- `profile.md`: stable learner profile and goals.
- `curriculum/roadmap.md`: curriculum strategy and tracks.
- `state/learned.md`: items demonstrated with usable mastery.
- `state/review_queue.md`: items that should reappear through spaced review.
- `state/backlog.md`: useful items not yet learned/tested.
- `sessions/`: one concise log per completed session.

See `AGENTS.md` for the operating protocol.