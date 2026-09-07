# Curriculum Roadmap

This curriculum is adaptive rather than date-locked. Progress depends on demonstrated performance, not merely completing a lesson.

Current skill priority:

1. Listening comprehension
2. Technical writing / prompting
3. Everyday speaking
4. Technical reading

Topic choice should still favor the learner's real domains.

## Phase 0 — Diagnostic calibration (first 3 sessions)

Goal: establish the learner's practical English profile across listening, writing, speaking, and reading.

### Session A — Listening + AI/Agent explanation
- Hear a short AI/Agent/debugging explanation without transcript first.
- Identify gist, cause/effect, and important details.
- Re-listen if needed and recover key chunks.
- Give a short summary.
- Finish with one Chinese -> English Agent instruction.

Measure subtitle/transcript dependence, detail retention, and reuse of heard language.

### Session B — Chinese -> English technical production
- Rewrite realistic Chinese instructions into natural English.
- Focus on constraints, sequencing, acceptance criteria, exceptions, and debugging language.
- Identify repeated grammar/word-choice/collocation issues.
- Add a brief spoken explanation or read-aloud when voice is available.

### Session C — Speaking + Blender / generative-media communication
- Explain a familiar Blender/rendering/video-generation problem in English.
- Handle follow-up questions requiring clarification, correction, comparison, and uncertainty.
- Add a short listening segment in the same domain.

After Phase 0, update `profile.md` with observed strengths and weaknesses for each skill independently.

---

## Mandatory language-learning layer

Every normal lesson should deliberately teach a small set of reusable language items from the day's context. Do not rely on comprehension questions alone.

### Item types

Use a mix of these four types:

1. **Word** — a high-value individual word whose meaning or usage is not yet stable.
2. **Phrase / collocation / chunk** — preferred whenever a reusable multi-word unit exists, such as `narrow down the cause` or `meet the acceptance criteria`.
3. **Sentence pattern** — a reusable grammatical/discourse frame, such as `The issue is not X; it's Y.` or `This seems inconsistent with ...`.
4. **Domain expression** — a technical expression that is useful as a unit, such as `frame-time spike`, `weight painting`, or `maintain backward compatibility`.

Phrases/chunks and sentence patterns are generally more valuable than isolated vocabulary because they can be retrieved directly during speaking and writing.

### Quantity limits

- Normal ~30 minute lesson: about **4–7 new language items total**.
- Quick/manual ~10–15 minute lesson: about **2–4 new language items total**.
- Extra-time sessions may add more only when the learner is handling the current set easily; do not turn extra time into a large vocabulary dump.

### Context requirement

Never teach a new item as only `English = Chinese meaning`.

For each new item, normally provide:

- the meaning that matters in the current context,
- its grammatical role or common collocation when useful,
- **at least one natural contextual example**,
- a brief contrast/common mistake only if it prevents likely misuse,
- one opportunity for the learner to recognize, retrieve, or use it.

Examples should preferably come from the learner's real domains or a realistic everyday situation.

Example:

- `constraint` — 限制条件 / 约束
- useful chunk: `under this constraint`, `hardware constraint`
- Agent context: `Do not change the production code; treat that as a hard constraint.`
- Blender context: `VRAM is the main constraint when rendering this scene at 4K.`

For a sentence pattern:

- pattern: `The issue is not X; it's Y.`
- Agent context: `The issue is not model capability; it's the way the harness provides context.`
- Hardware context: `The issue is not average FPS; it's the frame-time spikes.`

The purpose of examples is to make the learner understand **when and how the expression is actually used**, not merely to decorate a definition.

### Source-from-context rule

Whenever practical, select new language from something the learner just:

- heard in a listening item,
- read in a short passage,
- tried to express in English,
- misunderstood,
- or needed in a realistic task.

This creates a loop:

`context -> notice useful language -> understand it -> reuse it -> review it later in a different context`

Do not introduce unrelated vocabulary merely to fill a quota.

### Active-use rule

An item is not considered learned because the learner read its explanation once.

Use at least one of:

- Chinese -> English recall,
- fill the item into a new sentence,
- choose between two near-synonyms and explain the choice,
- paraphrase using the target phrase,
- write a new Agent/Blender/hardware/everyday sentence with it,
- recognize it from audio,
- say it naturally in Voice.

For a batch of 4–7 items, not every item needs a separate exercise immediately. Combine several naturally in one output task to avoid bloating the lesson.

### Contextual review rule

Spaced review should change the surrounding sentence or scenario. Avoid reviewing only by repeating the exact original example.

Good progression:

1. understand `root cause` in a debugging passage,
2. recall it next day from Chinese,
3. use it in a different Blender or pipeline problem,
4. recognize it in spoken English,
5. use it spontaneously in a later explanation.

Move an item toward mastery only when the learner can retrieve or interpret it in context, not merely recognize a memorized translation.

---

## Track A — Agent / coding / GitHub English

Core abilities:
- Give precise instructions and constraints.
- Describe bugs and reproduction steps.
- Discuss implementation choices and trade-offs.
- Understand spoken and written explanations of technical workflows.
- Read README, issue, PR, changelog, and error-log language.

High-value language themes:
- reproduce / reproduce consistently
- expected vs actual behavior
- acceptance criteria
- regression
- workaround
- edge case
- dependency
- deterministic / nondeterministic
- bottleneck
- failure mode
- fallback
- scope
- constraint
- assumption
- verify / validate
- isolate / narrow down
- root cause
- trade-off
- maintain backward compatibility

Representative tasks:
- Listen to a short debugging explanation and identify the root cause.
- Rewrite an Agent instruction.
- Write a concise bug report.
- Summarize a PR or spoken implementation explanation.
- Explain why a pipeline step failed.
- Compare two implementation strategies.

---

## Track B — Blender / 3D / rendering English

Core abilities:
- Understand tutorials and spoken technical explanations.
- Describe pose, rigging, materials, camera, lighting, and animation problems.
- Give precise instructions to an Agent or artist.

High-value themes:
- rig / armature / bone hierarchy
- inverse kinematics (IK)
- retargeting
- weight painting / skinning
- topology
- UV mapping
- normals
- roughness / metallic / specular
- PBR materials
- shader
- viewport vs final render
- keyframe / interpolation
- cloth simulation
- collision
- camera framing
- focal length
- depth of field
- lighting setup

Representative tasks:
- Listen to and summarize a short tutorial segment.
- Explain a rigging failure.
- Describe a desired pose precisely.
- Compare PBR and stylized rendering choices.

---

## Track C — Generative image/video English

Core abilities:
- Understand English demos/reviews of image and video tools.
- Write precise prompts.
- Describe visual defects and temporal problems.
- Compare generations and workflows.

High-value themes:
- prompt adherence
- reference consistency
- temporal consistency
- artifact
- flicker
- motion continuity
- frame interpolation
- loop / seamless loop
- seed
- upscale / super-resolution
- keyframe
- endpoint
- motion speed
- visual fidelity

Representative tasks:
- Listen to a short workflow explanation and extract the sequence.
- Turn a Chinese visual request into a concise English prompt.
- Critique a generation.
- Explain a frame-rate or looping problem.

---

## Track D — Hardware / gaming technology English

Core abilities:
- Understand review videos and community explanations.
- Read reviews and community reports.
- Explain performance symptoms and compare hardware/software techniques.

High-value themes:
- frame time
- stutter
- latency
- bottleneck
- frame generation
- upscaling
- VRAM
- thermal throttling
- utilization
- 1% low
- input lag
- refresh rate
- image quality trade-off

Representative tasks:
- Listen to a short review segment and recover the conclusion plus evidence.
- Summarize a hardware review.
- Explain why average FPS can look smooth while frame-time spikes feel bad.
- Compare native rendering, upscaling, and frame generation.

---

## Track E — Engineering / workplace English

Core abilities:
- Describe physical observations, tolerances, evaluation criteria, and vehicle ergonomics.
- Understand concise technical explanations.
- Write concise technical notes.

High-value themes:
- gap and flush
- tolerance
- deviation
- reference / datum
- clearance
- interference
- line of sight
- visibility
- steering column
- A-pillar
- ergonomic / reachability
- subjective evaluation
- acceptance range
- nominal value
- upper/lower limit

Representative tasks:
- Translate a vehicle evaluation note.
- Explain a dimensional requirement orally or in writing.
- Distinguish nominal value, tolerance, and total allowed range.

---

## Track F — General practical English

This track prevents technical English from becoming too narrow and supports the third-ranked goal: everyday speaking.

Focus on:
- natural conversation chunks
- asking for clarification
- disagreement and correction
- uncertainty
- comparison
- explaining preferences
- making plans
- summarizing information
- conversational repair when a word is missing

Useful discourse patterns:
- What I mean is ...
- The issue is not X; it's Y.
- I'm not sure whether ...
- Could you verify ...?
- This seems inconsistent with ...
- My concern is that ...
- The main trade-off is ...
- In practice, ...
- From what I've seen, ...
- The reason I prefer X is ...

Representative tasks:
- listen-and-respond mini-dialogues
- clarification role-play
- spoken preference comparison
- repair a misunderstood statement
- summarize what another speaker meant

---

## Weekly balance guideline

Do not force a rigid weekday syllabus. Across roughly 7 completed sessions:

- Listening should appear in most full multimodal sessions.
- Technical writing/prompting should appear in several sessions.
- Speaking should appear regularly in evening/weekend voice-capable sessions.
- Reading should support all tracks and can dominate daytime text-only sessions.
- Contextual word/phrase/sentence learning should appear in virtually every completed lesson, but remain small enough that the lesson still includes real comprehension and output.

Topic rotation guideline:
- 2–3 sessions: Track A
- 1–2 sessions: Track B/C
- 1 session: Track D or E
- 1 session: Track F or mixed review

Review can replace any new-content session when the queue is heavy.

## Advancement rule

Move an item toward `learned.md` only when the learner can demonstrate appropriate active mastery without heavy prompting, for example:

- understand it from audio when listening mastery matters,
- explain it correctly in English,
- use it naturally in a new sentence,
- distinguish it from a confusable alternative,
- apply it correctly in a realistic task.

Written recognition alone is not enough for items whose main goal is listening or speaking.
