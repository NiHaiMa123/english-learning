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
