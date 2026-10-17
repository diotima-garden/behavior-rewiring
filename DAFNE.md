---
format: 0
requires: []
---

# behavior-rewiring — base node for deliberate behavior change

The shared base for practice groves that train **procedural** change — replacing an
automatic behavior with a different one. It answers one question for all of them: how an
understood intention becomes an automatic behavior, and how much of that can be run at
once. It holds theory, evidence grades, and reusable protocols; it holds no practice and
no logs.

Start with `./principles.md`. It is the stance everything else serves, and it is short.

## Files

| File | What |
|---|---|
| `./principles.md` | The stance a child grove designs against. Opinionated, drill-agnostic. **Read first.** |
| `./sources.md` | What each claim rests on, graded A–F, including which popular claims fail. Consult before repeating any mechanism as fact. |
| `./protocols/` | Reusable procedure templates. `single-target-sprint.md` (one active target + catch-log) and `delay-rule.md` (forced interception without willpower). |
| `./open-questions.md` | What is genuinely unresolved, and where the seed material was invented. |
| `./information-population-plan.md` | How this node came to be filled, and what deliberately stays out. Read before adding anything. |

## No memory bank — load-bearing, not incidental

This node declares no `banks:`, so it is a bare node and not a grove. That is deliberate:
bank discovery recurses into `parents/`, so a bank here would be read and written by every
child grove's sessions — a shared write surface across unrelated personal practices.
Practice logs stay in the grove that owns the practice. Full rationale:
`information-population-plan.md` §4.

## How children use it

Mount at `parents/behavior-rewiring/` and **read these files in place**. The relationship
is semantic reference, not compilation — `#include` is available for a grove that compiles
a layered prompt, but it is one use of the relationship, not its definition.

| Grove | Relationship |
|---|---|
| `social-dynamics` | First consumer. Frame-control and boundary drills; its `improvement-plan.md` item #4 (the leak-log) is where this node's theory becomes a real-world rep loop. |

Anticipated siblings, none yet existing: compulsive-use patterns, attention/doomscrolling,
reactive anger, impulse inhibition.

## Editing this node

It is mounted as a `parents/` submodule by each consumer, so several working copies exist
and none is canonical — `origin` is. Finishing means: commit on `main`, push, then in each
consuming grove `git submodule update --remote parents/behavior-rewiring` and commit the
pointer. Stopping inside a submodule checkout leaves the work invisible to everyone else.
