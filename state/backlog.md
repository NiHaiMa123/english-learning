# Learning Backlog

Items here are candidates, not assumptions that the learner does not know them. Test before teaching when appropriate.

## Priority A — Agent / coding / GitHub

- acceptance criteria — introduced 2026-09-11
- expected behavior / actual behavior — introduced 2026-09-13
- reproduce / reproduction steps — `reproduce the issue` introduced 2026-09-13
- regression — introduced 2026-09-13
- workaround — introduced 2026-09-13
- edge case — introduced 2026-09-13
- dependency — introduced 2026-09-13
- deterministic / nondeterministic — `nondeterministic` introduced 2026-09-13
- bottleneck — introduced 2026-09-13
- failure mode
- fallback — introduced 2026-09-13
- constraint — introduced 2026-09-13
- assumption / assume + clause — introduced 2026-09-11
- verify vs validate
- isolate the issue — introduced 2026-09-13
- narrow down the cause — introduced 2026-09-13
- root cause — introduced 2026-09-13
- address the root cause — introduced 2026-09-13
- trade-off / trade-off between A and B — introduced 2026-09-13
- scope
- backward compatibility
- branch / commit / pull request / diff / merge / rebase / revert

### Agent permissions / safety — introduced 2026-09-09
- have access to ...
- grant access
- revoke access
- sensitive action(s)
- require user approval / should require user approval
- explicit permission / without explicit permission

### GitHub PR / Agent context — introduced 2026-09-09
- merge-ready / make a pull request merge-ready
- fix failed checks
- resolve review feedback
- resolve merge conflicts
- content exclusion(s)
- sensitive code / sensitive files
- keep A out of B

### Agent evaluation / PR approval — introduced 2026-09-11
- count toward ... / count as ...
- dismissed / an approval is dismissed
- authorize A to do B
- assess whether ...
- assess whether ... vs verify that ...
- meet the acceptance criteria
- reassess whether ...
- request a new review

## Priority B — Blender / 3D / rendering

- rig / armature / bone hierarchy
- inverse kinematics (IK)
- retargeting
- weight painting / skinning
- topology
- UV mapping
- normals
- roughness / metallic / specular
- PBR material
- shader
- viewport / final render
- keyframe / interpolation
- cloth simulation
- collision
- camera framing
- focal length
- depth of field

### Cloth / collision — introduced 2026-09-09
- clip through ... / clipping
- collision / collision object / collider
- penetration / reduce penetration
- self-collision
- intersect with ... / intersect with itself
- prevent A from doing B
- add a small clearance between A and B
- increase collision quality

## Priority C — Generative image/video

- prompt adherence
- reference consistency
- temporal consistency
- artifact
- flicker
- motion continuity
- frame interpolation
- seamless loop
- seed
- upscale / super-resolution
- keyframe / endpoint
- visual fidelity

## Priority D — Hardware / gaming

- frame time
- stutter
- latency
- bottleneck — introduced in AI/performance context 2026-09-13
- frame generation
- upscaling
- VRAM
- thermal throttling
- utilization
- 1% low
- input lag
- refresh rate
- inference speed — introduced 2026-09-13
- throughput — introduced 2026-09-13
- increase parallelism — introduced 2026-09-13

## Priority E — Engineering / workplace

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
- nominal value
- upper / lower limit

## Priority F — Reusable discourse chunks

- What I mean is ...
- The issue is not X; it's Y.
- I'm not sure whether ...
- Could you verify ...?
- This seems inconsistent with ...
- My concern is that ...
- The main trade-off is ... — introduced 2026-09-13
- In practice, ...
- From what I've seen, ...
- The reason I prefer X is ...
