# Sources

What the claims in `principles.md` actually rest on, and where they are thinner than
popular treatments imply. Graded, not exhaustive — the point is trustworthiness, so an
entry that says "this is folklore" is worth as much as one that says "this replicates."

**Grades:** **A** — large meta-analysis or multi-lab replication, direction not seriously
disputed. **B** — real literature, real effect, contested magnitude or scope.
**C** — single studies / indirect evidence; use as a frame, not a fact.
**F** — popular claim that does not survive contact with the literature.

---

## 1. Willpower as a depletable fuel — **F**

**The claim:** self-control draws on a finite resource (glucose); exerting it depletes
later self-control, so parallel behavior changes collapse the system.

**What happened:** a 24-lab Registered Replication Report (2016, N > 2,000) found
d ≈ 0.04. A second multi-lab RRR led by Vohs (*Psychological Science*, 2021; 36 labs,
N ≈ 3,531) used a paradigm Baumeister had pre-approved as the strongest version and found
d ≈ 0.06, non-significant. The glucose variant fared worse still; publication-bias-
corrected estimates land between ~0.04 and ~0.24, and cerebral glucose consumption is
roughly flat across effortful and idle cognition.

**Why it matters here:** this was the seed material's primary mechanism for
sequential-over-parallel. The conclusion survives; the reason does not. `principles.md` §2
re-grounds it in detection load, which also explains the active/passive asymmetry that the
fuel model cannot. Anything in a child grove that reasons about "spending willpower,"
decision fatigue, or doing hard things before the tank drains is inheriting a dead model.

## 2. If-then anchors (implementation intentions) — **A**

**The claim:** pre-specifying "when situation X arises, I will do Y" substantially raises
the rate at which Y actually happens, without needing the intention held in mind.

**Source:** Gollwitzer & Sheeran, *Advances in Experimental Social Psychology* 38 (2006) —
meta-analysis of 94 independent tests, N > 8,000, **d ≈ 0.65** on goal attainment. The
effect does not shrink toward zero as samples grow. Mechanism is cue-triggered
automaticity rather than added motivation.

**Caveat worth keeping:** later work suggests the pooled average is somewhat inflated, and
the strongest results come from behaviors with crisp, externally visible cues
(appointments, screenings). Our targets have *internal* cues — an impulse rising — which is
the harder case and under-represented in that corpus. Direction: solid. Magnitude for
interception specifically: assume less.

**This is the single best-evidenced lever in this node.** When in doubt, build the anchor.

## 3. Habit formation: cue-bound, slow, sleep-stabilized — **A/B**

**Cue→response structure — A.** Wood & Rünger, "Psychology of Habit," *Annual Review of
Psychology* 67 (2016): habits are cue-response associations in memory, acquired by
repetition in a *stable context*, activated by recurring context cues, and notably
insensitive to short-term goal changes. This is the basis for `principles.md` §3 — and for
why a trait-level target is not a target.

**Time to automaticity — B.** Lally et al. (2010), 96 participants adopting a daily
behavior over 12 weeks: median ~**66 days** to reach 95% of a modeled automaticity
plateau, individual range ~**18–254 days**, with simple behaviors fast and effortful ones
taking months. Two softeners the famous number usually sheds: the median comes from the
**39 participants whose curves fit the model** (82 of 96 gave analysable data at all), and
the behaviors were easy daily acts in a fixed context — generous conditions relative to
social interception. The range is the finding; the median is the part that got famous.

**Sleep consolidation — B, with the mechanism downgraded.** Sleep-dependent consolidation
of procedural/motor skill is well established (Walker & Stickgold, *Annu. Rev. Psychol.*
2006, and the NREM-reorganization literature since). But the careful framing is
**stabilization and retention rather than overnight enhancement**, and the popular
"slow-wave sleep myelinates the new pathway" line overstates it — myelination is a real
plasticity mechanism on a much longer timescale, not the overnight step. Protect sleep
because reps decay without it, not because of a myelin story.

## 4. Keystone habits / general inhibition training — **C for the concept, F for the training**

**The claim:** fix one upstream behavior — canonically impulse inhibition, the pause
between trigger and reaction — and three or four downstream flaws resolve on their own.

**Concept — C.** "Keystone habit" is a popularization (Duhigg, *The Power of Habit*),
carried by vivid cases rather than a tested causal chain; several of its showcase examples
have no peer-reviewed support, and it leans on the ego-depletion work in §1. Some genuine
spillover exists — e.g. new exercise routines coinciding with reduced smoking and drinking
in small longitudinal samples — so the phenomenon is not empty, just unquantified.

**Training the faculty — F.** This is the decisive finding. Lab training of general
response inhibition improves the trained task and does not transfer:

- Enge et al., *JEP: Learning, Memory & Cognition* (2014) — no true training *or* transfer
  effects from inhibitory-control training in healthy young adults; the adaptive group
  improved on the task but did not differ from an active control at post-test or
  follow-up.
- A domain-general cognitive-control training trial in children (*Nature Neuroscience*,
  2024) changed neither brain nor behavior.
- Inhibitory-control training aimed at unhealthy behaviors: no significant short- or
  long-term behavioral benefit versus control.
- The wider pattern it sits in: Sala et al., "Near and Far Transfer in Cognitive
  Training: A Second-Order Meta-Analysis," *Collabra: Psychology* 5(1):18 (2019) — 14
  independent meta-analyses, ~22,000 participants, near transfer real but far transfer
  negligible-to-null once placebo and publication bias are handled. Note this covers
  cognitive training broadly (working memory, music, chess, video games), not inhibition
  specifically; it is the prior, while the three entries above are the direct evidence.

**Ruling for this node:** keep "one change with wide reach" as a *selection heuristic* —
prefer a cue that genuinely precedes several behaviors — and discard "train inhibition in
general." Leverage comes from the cue being upstream, not from a strengthened faculty. If
a grove claims keystone leverage, it must name the shared cue.

## 5. Simulated stress and behavioral rehearsal — **A/B**

**Stress inoculation training — A.** Saunders & Driskell et al.'s meta-analysis (37
studies, 70 hypothesis tests, N ≈ 1,837) found SIT effective at reducing performance
anxiety and state anxiety *and* at improving performance under stress; broader reviews put
treated participants above ~76% of untreated controls, effects maintained to follow-ups out
past a year. Rehearsing under manufactured arousal is a real, evidenced route to reps.

**Transfer to our medium — B at best.** That corpus is clinician-led role-play, graded
exposure, and VR with genuine physiological presence. A text chat graded by an LLM is the
lightest and least validated point on that spectrum. The consuming grove already states
this gap explicitly (`social-dynamics/research/does-low-stakes-simulation-build-boundary-
skills.md`) and the honest position is: *mechanism well evidenced, our implementation
unvalidated.*

**Embodied practice — C.** That physical disciplines change people faster than reading is
plausible and consistent with §5's arousal argument, but the specific comparison is
untested. Keep it as a bet, not a finding — see `open-questions.md` §3.

## 6. Attention/working-memory limits — **B**

The "3–4 chunks" working-memory figure (Cowan) is real and widely replicated, but it
describes short-term storage, not a day-long monitoring budget, and importing it directly
to "how many habits can I track" is an analogy rather than a result. What does carry: a
primed, specific expectation beats diffuse vigilance, and simultaneous monitoring of many
distinct triggers degrades each. `principles.md` §2 uses the direction, not the number.

---

## Deliberately not cited

The seed document this node grew from (see `information-population-plan.md` §2) is
unsourced LLM prose and is **not a source**. Several of its confident figures are not
traceable to any study — the success-rate table by number of simultaneous habits most of
all. See `open-questions.md` §1.
