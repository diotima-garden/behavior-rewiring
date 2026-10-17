# Information Population Plan

*How this node gets filled. Written 2026-10-17, at creation, when the node holds nothing
but this file and `DAFNE.md`. Intended to be executed in its own context window — it
assumes no knowledge of the session that created it.*

> **Executed 2026-10-17.** §3's build order is history: `principles.md`, `sources.md`,
> `protocols/` and `open-questions.md` all exist — read them rather than rebuilding them.
> What stays live here is §2 (the seed source and its two hard rules), §3's
> multi-checkout warning, §4 (what stays out), and §5. Adding to this node still means
> reading those first.

---

## 1. What this node is for

Practice groves in this garden train a skill. This node holds what they all need and
none of them should own a private copy of: **how an understood intention becomes an
automatic behavior**, and what the evidence says about doing that deliberately.

The framing that makes it matter here: diotima's existing machinery is built around
*declarative* encoding — Anki, spaced repetition, recall of facts. This node is the
*procedural* counterpart, and the two have opposite scaling laws. SRS runs thousands of
cards in parallel; procedural rewiring appears to collapse above roughly one active
change at a time. A learning conductor that models only the first channel will give
confidently wrong advice about the second.

## 2. The seed source — and its serious caveat

A local, **unversioned** PDF sits at the garden root:
`$DIOTIMA_GARDEN/neuroplasticity.pdf` (the garden root is not itself a repo, which is
why the file stays unversioned where it is). It is the back half of a personal
conversation with Gemini and it is the reason this node exists.

Two hard rules about it:

1. **It is a source of hypotheses, not of facts.** It is unsourced LLM prose. It states
   specific figures with high confidence — success rates by number of simultaneous
   habits, months-to-consolidation ranges, named brain regions per stage. Treat every
   one as a claim to verify, not a finding to copy. Where the literature disagrees or is
   thinner than the PDF implies, that disagreement is itself worth recording.
2. **It is personal and stays out of this repo.** The document is a conversation about a
   real person by name, with relational detail. Extract the generic mechanism only.
   Never quote it, never copy a name, situation, date, or example from it, and never
   commit it or any excerpt. This node is public.

The concepts worth extracting and then checking (the PDF's own framing, restated
neutrally so this plan survives the file being gone):

- A four-stage path from comprehension to automaticity: intellectual understanding →
  catching the impulse in real time → repetition of the substituted behavior →
  consolidation into a default.
- The claim that understanding alone produces no behavioral change — that the bridge is
  real-time friction, not more reading.
- A sharp drop-off in success as the number of simultaneous behavior changes rises;
  hence sequential, single-target work over parallel self-improvement.
- "Keystone" behaviors: one change that dissolves several downstream ones — notably
  impulse inhibition, the pause between trigger and reaction.
- Deliberately simulated stress as a way to get reps without waiting for life to supply
  them, and physical/embodied practice as a faster route than verbal reasoning.
- Sleep as the consolidation step, not an afterthought.
- Implementation intentions ("if X, then Y") as the mechanism for not having to hold an
  abstract intention in working memory all day.

Several of these map onto real, well-studied literatures — implementation intentions
(Gollwitzer), habit formation and context-cue learning, inhibitory control, stress
inoculation, sleep-dependent consolidation. Those literatures, not the PDF, are what
this node should end up citing.

## 3. What to build

**Before editing: know which checkout you are in.** This repo is mounted as a
`parents/` submodule by each grove that consumes it, so several working copies of it
exist at once and none of them is canonical — `origin` is. Whichever copy you work in,
finishing means: commit, push to `origin`, then in each consuming grove bump the
submodule pointer (`git -C <grove> submodule update --remote parents/behavior-rewiring`,
then commit the pointer change there). Editing inside a submodule checkout and stopping
leaves the work invisible to everyone else.

Work in this order; stop when it's useful rather than when it's complete.

1. **`principles.md`** — the stance, the way `social-dynamics/principles.md` does it for
   that grove. Drill-agnostic, short, opinionated. The durable claims a child grove can
   design against: sequential over parallel, friction over comprehension, anchors over
   willpower, consolidation as a real step.
2. **`sources.md`** — what the claims actually rest on. Each entry: the claim, the real
   source, how strong the evidence is, and where it's weaker than popular treatments
   suggest. This is the file that makes the node trustworthy rather than merely
   plausible.
3. **`protocols/`** — one file per reusable procedure a child grove can instantiate
   (e.g. a single-target sprint with a daily catch-log; a delay rule that forces
   interception without relying on willpower). A protocol here is a template; the
   running of it, and its log, belong to the child grove.
4. **`open-questions.md`** — what remains genuinely unresolved, including where the
   seed PDF overstated its case. Keep this honest; it's what stops the node calcifying
   into confident folklore.

## 4. What deliberately stays out

- **Textbook restatement.** Any model reading this node already knows the general
  neuroscience — that is where the seed PDF came from in the first place. Content that
  tells the model what it already knows costs context and buys nothing. Weight this node
  toward *curation and decisions*: which claims survived scrutiny, which were discarded
  and why, what applies to this specific person's profile. Cite mechanism; don't
  re-explain it.
- **Practice logs, session history, personal evidence.** This node carries no memory
  bank, by design: `manifest.py:discover_banks` recurses into `parents/`, so a bank here
  would be read and written by every child grove's sessions. Longitudinal records live in
  the grove that owns the practice.
- **Anything identifying.** See §2.2. The repo is public.

## 5. How children use what's built here

A child grove mounts this node at `parents/behavior-rewiring/` and reads these files
directly. Compilation via `#include` is available but is one use of the relationship,
not a requirement — `language/queue-policy.md` is the existing precedent for a parent
file that is read in place and never spliced.

`social-dynamics` is the first and currently only child. Its
`improvement-plan.md` item #4 — promoting the leak-log from a someday-seam into a real
capture → review → feed-back-into-drills loop — is the concrete place this node's theory
first has to earn its keep. A good test of whether `principles.md` is any good: does it
tell that item how to be designed?
