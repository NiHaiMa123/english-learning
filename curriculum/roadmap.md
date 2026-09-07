# Curriculum Roadmap

This curriculum is adaptive rather than date-locked. Progress depends on demonstrated performance, not merely completing a lesson.

## Phase 0 — Diagnostic calibration (first 3 sessions)

Goal: establish the learner's practical English profile.

Each diagnostic session should test a different mode:

### Session A — Technical reading + explanation
- Read a short AI/Agent or GitHub-related passage.
- Answer comprehension questions.
- Explain the main point in English.
- Extract 5–8 useful chunks.

### Session B — Chinese -> English technical production
- Rewrite realistic Chinese instructions into natural English.
- Focus on constraints, sequencing, acceptance criteria, and debugging language.
- Identify repeated grammar/word-choice issues.

### Session C — Mixed practical communication
- Short dialogue or role-play.
- Explain a Blender/rendering/hardware/engineering problem.
- Optional voice/pronunciation component if enabled.

After Phase 0, update `profile.md` with observed strengths and weaknesses.

---

## Track A — Agent / coding / GitHub English

Core abilities:
- Give precise instructions and constraints.
- Describe bugs and reproduction steps.
- Discuss implementation choices and trade-offs.
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
- Rewrite an Agent instruction.
- Write a concise bug report.
- Summarize a PR.
- Explain why a pipeline step failed.
- Compare two implementation strategies.

---

## Track B — Blender / 3D / rendering English

Core abilities:
- Understand tutorials and technical discussions.
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
- Explain a rigging failure.
- Describe a desired pose precisely.
- Compare PBR and stylized rendering choices.
- Follow and summarize a short tutorial excerpt.

---

## Track C — Generative image/video English

Core abilities:
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
- Turn a Chinese visual request into a concise English prompt.
- Critique a generation.
- Explain a frame-rate or looping problem.

---

## Track D — Hardware / gaming technology English

Core abilities:
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
- Summarize a hardware review.
- Explain why average FPS can look smooth while frame-time spikes feel bad.
- Compare native rendering, upscaling, and frame generation.

---

## Track E — Engineering / workplace English

Core abilities:
- Describe physical observations, tolerances, evaluation criteria, and vehicle ergonomics.
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
- Explain a dimensional requirement.
- Distinguish nominal value, tolerance, and total allowed range.

---

## Track F — General practical English

This track prevents technical English from becoming too narrow.

Focus on:
- natural conversation chunks
- asking for clarification
- disagreement and correction
- uncertainty
- comparison
- explaining preferences
- making plans
- summarizing information

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

---

## Weekly balance guideline

Do not force a rigid weekday schedule. Across roughly 7 completed sessions, aim for:

- 2–3 sessions: Track A
- 1–2 sessions: Track B/C
- 1 session: Track D or E
- 1 session: Track F or mixed review

Review can replace any new-content session when the queue is heavy.

## Advancement rule

Move an item toward `learned.md` only when the learner can do at least one of the following without heavy prompting:

- explain it correctly in English,
- use it naturally in a new sentence,
- distinguish it from a confusable alternative,
- apply it correctly in a realistic task.
