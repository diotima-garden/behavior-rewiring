---
format: 0
requires: []
---

# behavior-rewiring — base node for deliberate behavior change

A bare DAFNE node: no memory, therefore not a grove. No parents.

The shared base for practice groves that train *procedural* change — replacing an
automatic behavior with a different one. Holds the theory, the sources, and the
curation decisions those groves draw on; holds no practice and no logs of its own.

**Status: near-empty by design.** Only this manifest and the population plan exist.
See `./information-population-plan.md` — populating this node is its own task, run in
its own context.

| File | What |
|---|---|
| `./information-population-plan.md` | How this node gets filled: sources to mine, the structure to grow into, and what deliberately stays out. Read this before adding anything here. |

## Why this is a base node and not a grove

Grove-ness is structural — a node carrying memory. This node deliberately carries
none, and that is load-bearing rather than incidental: `manifest.py:discover_banks`
recurses into `parents/`, so a bank declared here would be discovered, read at
orientation, and written into by **every** child grove's sessions. Since the intended
children are personal-practice groves, a bank here would be a shared write surface
across all of them. Practice logs stay in the grove that owns the practice.

## How children consume this node

By **reading**, primarily. A child mounts this node at `parents/behavior-rewiring/`
and its sessions refer to these files directly — same pattern as `language`'s
`queue-policy.md`, which is deliberately never `#include`d and read in place.

`#include ./parents/behavior-rewiring/...` is available for children that compile a
layered prompt, but it is one use of the relationship, not its definition and not a
prerequisite for mounting.

## Children

| Grove | Relationship |
|---|---|
| `social-dynamics` | First consumer. Frame-control and boundary drills; its `improvement-plan.md` item #4 (the leak-log) is the seam where this node's theory becomes a real-world rep loop. |

Anticipated siblings — one grove per practice, each with its own intake, drills, and
log: compulsive-use patterns, attention/doomscrolling, reactive anger, impulse
inhibition. None exist yet; this table grows as they do.
