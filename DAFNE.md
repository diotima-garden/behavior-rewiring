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

Start with `./principles.md`. It is the stance everything else serves, and it is short —
including its scope block, which rules three common targets out of bounds (substance
dependence, changing what you feel, and "applying" an idea that names no cue).

## Files

| File | What |
|---|---|
| `./principles.md` | The stance a child grove designs against. Opinionated, drill-agnostic. **Read first.** |
| `./sources.md` | What each claim rests on, graded A–F, including which popular claims fail. Consult before repeating any mechanism as fact. |
| `./protocols/` | Reusable procedure templates. `single-target-sprint.md` (one active target + catch-log) and `delay-rule.md` (forced interception without willpower). |
| `./open-questions.md` | What is genuinely unresolved, and where the seed material was invented. |

## No memory bank — load-bearing, not incidental

This node declares no `banks:`, so it is a bare node and not a grove. That is deliberate:
`manifest.py:discover_banks` recurses into `parents/`, so a bank declared here would be
discovered, read at orientation, and written into by **every** child grove's sessions — a
shared write surface across unrelated personal practices. Practice logs stay in the grove
that owns the practice.

## How children use it

Mount at `parents/behavior-rewiring/` and **read these files in place**. The relationship
is semantic reference, not compilation — `#include` is available for a grove that compiles
a layered prompt, but it is one use of the relationship, not its definition.

| Grove | Relationship |
|---|---|
| `social-dynamics` | First consumer. Frame-control and boundary drills; its `improvement-plan.md` item #4 (the leak-log) is where this node's theory becomes a real-world rep loop. |

Anticipated siblings, none yet existing: compulsive-use patterns, attention/doomscrolling,
reactive anger, impulse inhibition.

## Contributing

**The seed source.** This node grew from an unversioned local PDF of a personal LLM
conversation (`$DIOTIMA_GARDEN/neuroplasticity.pdf`). Two rules survive it: it is a source
of *hypotheses, not facts* — its confident figures are unsourced prose and several are
untraceable (`open-questions.md` §1) — and it is personal, so it stays out of this public
repo. Extract generic mechanism only; never quote it or copy a name, situation or example.

**What deliberately stays out.** Textbook restatement (any model reading this already
knows the general neuroscience — weight this node toward *curation*: which claims survived
scrutiny, which were discarded and why). Practice logs and personal evidence (no bank, by
design — see above). Anything identifying.

**Mechanics.** Several working copies exist (one per consumer) and none is canonical —
`origin` is. Finishing means: commit on `main`, push, then in each consuming grove
`git submodule update --remote parents/behavior-rewiring` and commit the pointer. Stopping
inside a submodule checkout leaves the work invisible to everyone else.
