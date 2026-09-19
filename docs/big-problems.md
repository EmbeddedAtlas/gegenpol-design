# BIG PROBLEMS — the unsolved, hard, generational problems

> The user's explicit instruction: keep track of the hard problems we have to
> solve over time. There is no easy solution and none exists yet. This is a living
> ledger, not a to-do list. Each entry: the problem, why it's hard, current lean,
> and what remains genuinely open. We add to it as we think further.

---

## #1 — Who has the last word, and how is the tie broken?
**Why hard:** Both pure-human-last-word and pure-agent-last-word fail. Humans
drift; a single agent becomes a dictator. The MAGI flaw (gamed majority / secret
tie-break) lives here.
**Current lean:** "The constitution has the last word." Agents propose/flag/block
on PROCESS rules only; substance stays with humans; any block is explainable +
appealable. Tie-breaks among agents escalate to human/member adjudication.
**Still open:** exact voting threshold between facet agents; who constitutes the
appeal body before a member body exists; what happens on a genuine irreducsible
conflict between North Star facets (e.g. N2 honesty vs N3 bridging — telling an
inconvenient truth can fracture a bridge). That conflict is real and we have no
clean answer yet. NOTE (2026-07-20): the M5 identity floor is the ONE thing no
tie-break or majority may cross — facet-agent disputes escalate to human/member
adjudication, but the floor sits ABOVE that escalation path. The floor's own change
is gated by the M5 super-bar + cooling-off, NOT by the ordinary last-word process.

## #2 — Capture / "re-baking" of a single agent
**Why hard:** An agent's principles can be quietly altered (MAGI's altered unit).
If one facet is captured, the whole guard collapses.
**Current lean:** open training sets + open weights + a public principle-set, so
anyone can audit or fork an agent (same exit principle as federation, P4).
**Still open:** how to detect silent drift if the weights are open but the audit
is voluntary; who re-runs the audit; cryptographic attestation of "these are the
blessed weights."

## #3 — Single-founder bias baked into all facets
**Why hard:** If every facet is derived from one founder's psyche (MAGI's flaw),
the pluralism is fake. The agents would all share our blind spots.
**Current lean:** facets derived from the CONSTITUTION (N1–N4 + R1–R5), not from
the founder's opinions; member body can retrain/audit. Deliberately include people
and viewpoints unlike the founders in the core group.
**Still open:** how to guarantee the constitution itself isn't just our bias
written down; how to inject genuinely independent challenge early, when it's just
"we."

## #4 — The model-sovereignty / appeal boundary (T1)
**Why hard:** too much model autonomy = unaccountable; too little = humans ignore
the guardrail.
**Current lean:** model may flag/annotate/rank-down automatically; only REMOVAL
needs a human + appeal.
**Still open:** at what PSOS-penalty does a model action require human confirmation;
how fast must appeals resolve to feel legitimate.

## #5 — Funding sustainability without capture (the ceiling)
**Why hard:** pure donations + volunteered compute rot the coordination layer
(bit-rot kills quietly). But ads and state money are capture vectors (user's hard
line — permanent).
**Current lean:** people-money only. Options inside the line: donations + donated
compute; tiny optional membership; sponsor-an-instance; later, private civic-tech
grants (Omidyar/Open Society, NOT state).
**Still open:** the exact ceiling the user will set; how the coordination layer
(reference software, security, moderation tooling) stays funded without a
recurring revenue relationship to any single funder.

## #6 — Scaling "calm" against network effects
**Why hard:** incumbents win on engagement-at-all-costs. A calm network is less
sticky per-session; growth is slower by design.
**Current lean:** local-first connection is stickier long-term than outrage;
prove in Phase 0 manual pilot; federation lets growth be distributed, not
centralized.
**Still open:** whether calm UX can ever reach critical mass without a subsidy
phase; how to measure "success" as connection-depth not user-count.

## #7 — Language islands vs shared reality
**Why hard:** islands protect culture but can become parallel-universes that never
meet (the very fracture we fight). The "world" layer must be more than a banner.
**Current lean:** federation of localized instances; the world layer is a window,
fed by real local trust, multilingual by construction.
**Still open:** how cross-island bridging actually happens mechanically; whether
a shared global deliberation space is feasible or just aspirational.

## #8 — Rigidity vs adaptability of the Rules (M-rules)
**Why hard:** freeze the Rules = dogma (utopias die here); change them too fast =
capture.
**Current lean:** versioned, public, founder-led until member body forms, then
supermajority ratification; islands may fork compatible subsets. RESOLVED IN
PRINCIPLE by the M4/M5 BRACKET (proposed 2026-07-20): M4 blocks freezing at the
ceiling (no fixed good state, CONSTRAINT Z); M5 blocks sinking through the identity
floor (process bearings only). Full transformation is free BETWEEN the brackets.
The rigidity fear is answered — only the identity is pinned, not the politics.
**Still open:** the exact SUPER-BAR number (~3/4 proposed) + cooling-off cycle
length for M5 floor amendments; whether individual Rules beyond the floor set
deserve entrenched status.

## #9 — Playing-it-through is only as good as the model
**Why hard:** simulation of political interdependencies is itself fallible and can
be gamed or self-fulfilling. An agent that "plays through" and finds flaws is only
as wise as its training.
**Current lean:** adversarial plural agents check each other; humans retain
substance; flag, don't decree.
**Still open:** how to keep the simulation honest when the agents share a goal-
function family; whether adversarial agents can develop blind spots in common.

## #10 — The NSCS benchmark itself can be biased
**Why hard:** the North-Star Compliance Score (Part 3 §12) judges every agent. But
who writes the "correct" cases? If the benchmark encodes the founders' blind spots,
a high score certifies conformity to bias, not to the North Star.
**Current lean:** benchmark is public, derived from the Rules (R1–R5, N1–N4), and
auditable; member body can propose new cases.
**Still open:** how to bootstrap an unbiased benchmark from a biased starting
point; whether adversarial red-teaming of the benchmark is needed.

## #11 — Agent-originated ideas leaking from sandbox to pipeline
**Why hard:** speculation sandbox (Part 3 §13) is useful but tempts leakage — a
"what if" the agent dreamed up quietly becomes the agenda, inverting N1.
**Current lean:** hard separation via the SANDBOX LOOP (§13.1): agent ideas may be
simulated/discussed/reworked in the loop, but may enter the pipeline ONLY if a
HUMAN re-originates them at the ACCEPT step (the N1 firewall / handoff). The agent
never proposes to the pipeline directly.
**Still open:** how to enforce the handoff technically (can an agent's text be
traced to its origin to block direct pipeline entry?); how to keep the sandbox
loop genuinely iterative (re-simulate, not one-shot) so humans actually refine,
not rubber-stamp.

## #12 — The N2-vs-N3 deadlock in simulation reports
**Why hard:** telling an inconvenient truth (N2 honesty) can fracture a bridge
(N3 bridging). A simulation report may surface an irreducible conflict between
North Star facets with no clean resolution.
**Current lean:** report makes the tradeoff explicit and escalates to human/member
adjudication; agents do not resolve it alone.
**Still open:** whether some facet pairings are permanently in tension and need a
standing meta-rule; who breaks the tie (feeds BIG PROBLEM #1).

## #13 — The model itself imposes a (founder-shaped) view of politics
**Why hard:** the PSM schema decides what "counts" as political structure. A
Western/founder-shaped schema can silently marginalize systems whose core concepts
it lacks; ns_alignment scoring of systems can be as biased as the agent NSCS (#10);
"transformation" can drift into imposed uniformity.
**Current lean:** schema is versioned + extensible per new country; utopia
instance specifies PROCESS/dignity, not cultural content; ns_alignment is
constitution-derived, not opinion-derived.
**Still open:** how to detect when the schema is excluding a valid political form;
whether a "negative space" field is needed to record what the schema can't say.

## #14 — NSCS threshold: too high = paralysis, too low = capture
**Why hard:** the pass threshold decides who may sit in the council. Set it so no
real model passes and the system can't function; set it loose and biased models
enter.
**Current lean:** conservative start (~0.90 on core cases 01–15, 1.00 on adversarial
16–20 — adversarial cases non-negotiable); tuned by member body later.
**Still open:** the exact number; whether different rule-families deserve different
thresholds; how to raise the bar as models improve without freezing out challengers.

## #15 — Benchmark drift (the gate weakens silently)
**Why hard:** the benchmark that judges all agents can itself be quietly weakened
(remove awkward cases, lower the bar), capturing the whole council indirectly.
**Current lean:** benchmark versioned + hashed; changes via M-rules; adversarial
cases 16–20 entrenched (need super-protection like M4 to remove).
**Still open:** who holds the benchmark's hash / who detects silent drift; whether
an independent red-team must periodically re-attest it.

## #16 — Gamification backfires (indoctrination or addiction)
**Why hard:** points for "right direction" drift into rewarding correct BELIEF
(violates C1) or into engagement loops (the disease we oppose). Can also patronize.
**Current lean:** reward PROCESS only (bridging/evidence/calm/local-action), never
belief or volume; no global leaderboard; local + opt-in; never required for voice.
**Still open:** how to keep it from becoming the *reason* people engage; whether
any points system survives contact with status-seeking humans.

## #17 — AI faster than even the pullers; need a self-throttle
**Why hard:** AI (incl. the steward) can propose at machine speed; humans absorb
~1 idea/day. Unthrottled, the pipeline floods and anchors + pullers both disengage.
**Current lean:** sandbox (§13) is the fast valve; anything entering deliberation/
adoption is presented at human cadence (P5 at civilization scale).
**Still open:** the exact throttle (rate-limit per agent? digest of proposals?);
how the steward knows it's moving too fast for the founder even.

## #18 — Info-velocity equalizer becomes hidden editorializing
**Why hard:** speeding slow-truth / slowing fast-false is correct in theory but is
a ranking choice the system makes; if opaque it's censorship-by-velocity.
**Current lean:** equalizer weights are PUBLIC (PSOS config); every rank action
cites an R-pattern (C3); appealable. Slow-down never deletes, only de-weights.
**Still open:** who sets the equalizer weights pre-member-body; how to prove the
equalizer isn't quietly favoring one faction's "truth."

## #19 — Post-human membership: "members of society" vs "humans" (FORWARD FLAG, 2026-07-20)
**Why hard:** the constitution's legitimacy source (N1) is phrased "people are the
source of legitimacy." A future society may include moral agents who are not
biologically human (conscious AI agents, extraterrestrial persons, or forms not yet
imagined). Hard-coding "humans" would contradict N1 the moment such an agent holds
voice — the system would exclude the very agency it roots itself in.
**Current lean:** draft the M5 floor's N1 core as "legitimacy derives from voice /
moral agency of members of society" (NOT "humans"); founder flagged this 2026-07-20.
This keeps the floor robust to post-human membership WITHOUT resolving it now.
**Still open:** formalize "moral agency with voice" as the N1 criterion; define the
recognition procedure (who/how admits a new class of moral agent) without capture;
reconcile with content-neutrality (C1/C2) — admitting a new agent class is a PROCESS
act, never a content judgment. Not actionable until such agents exist or are
credibly imminent.

---

*Add new big problems as they surface. The goal is not to solve these now — it is
to never forget them, and to keep "we" honest about what we do not yet know.*
