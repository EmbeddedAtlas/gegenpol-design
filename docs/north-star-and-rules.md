# The North Star & The Rules — a deeper refinement

> Companion to `vision-phase0.md`. This document goes further: it pins down
> WHAT the principles actually say (the written constitution that both people
> and models follow), and it stress-tests the "principles baked into models" idea.
> Status: draft for joint refinement. No implementation.

---

## 0. What the research gave us (so we don't reinvent, and don't repeat failures)

- **Federation already works at planetary scale.** ActivityPub (the Fediverse:
  Mastodon, Pixelfed, PeerTube) is a W3C open standard, used by millions, with
  real servers run by volunteers. The "distributed, no single owner, donate
  compute = run an instance" model you described is *exactly how the Fediverse
  already grows*. We do not need to invent federation.
- **Platform cooperatives already exist.** The Platform Cooperativism movement
  (platform.coop, social.coop) proves user-owned, no-ad social infrastructure can
  exist. The funding ceiling you set (people money, no ads, no state) is a solved
  pattern, not a fantasy.
- **Deliberation tech already works — and crucially, uses ML to build consensus,
  not division.** vTaiwan / Pol.is (open source) feeds large-group opinion into
  ML that *clusters agreement and surfaces the consensus*, not the outrage. This
  is the proof that "models with principles baked in" can serve bridging instead
  of sorting. It's the opposite of the engagement algorithm.
- **Failed utopias teach one thing:** they die from *rigidity + hidden power*, not
  from external enemies. The communes that survived stayed small, kept exit easy,
  and let rules evolve. The ones that became nightmarish had a fixed dogma and a
  leadership that couldn't be checked. So our design must encode *changeability*
  and *exit* as first-class properties — or we repeat them.

**Conclusion:** our innovation is NOT the pipes. It is (1) the written North Star
as a binding constitution, (2) the principled-model referee layer, (3) the calm/
bridging-first UX, and (4) the language-island federation. The transport, the
co-op shell, and the deliberation ML are borrowed, not built.

---

## 1. The North Star (refined — a COMPASS, not a destination)

> CRITICAL REVISION (Phase A): the word "utopia" as a GOAL-POINT is retired. A
> fixed perfect end-state is a prison (the Matrix critique: a world with no agency
> or struggle is dystopia; an AI optimized to "create utopia" converges to
> dystopia). The North Star is a BEARING, not a coordinate.
>
> METAPHOR STATUS (open, to revisit): "compass" is also provisional — a compass
> points at a fixed point (North); reaching it = arrival, which CONSTRAINT Z
> forbids. We need a metaphor with NO arrival (gyroscope / river / tuning). Until
> then, "bearing held without a destination" is the working phrase.

- **N0 (meta, foundational) — Never optimize for a fixed "good" state.**
  The system must optimize for the CAPACITY TO CHANGE, including changing away
  from its current form. Arrival at a utopia = stasis = the thing humans reject =
  failure. Call this **CONSTRAINT Z**. It outranks the other N's: any North Star
  facet that would freeze the system into a dogma is subordinate to Z.
- The North Star is expressed as four BEARINGS to hold, not points to reach:
  - **N1 — People are the source of legitimacy.** (bearing: power flows from voice)
  - **N2 — Honesty over comfort.** (bearing: evidence stays legible)
  - **N3 — Connection across difference is the metric.** (bearing: bridge, don't sort)
  - **N4 — Calm, not addiction.** (bearing: earn attention, don't steal it)
- "Improve" is a loaded word: it implies convergence on a definable "better."
  We avoid it as a goal. We say **evolve / adapt / stay-in-right-relationship** —
  a process with no terminus. The direction of ever-increasing alignment to the
  bearings, WITH ever-present capacity to revise, is the whole aim.

### Translation rule (standing, for the future agent-template)
The founder tends to use destination-words ("utopia," "improve," "goal," "target")
when meaning process-words ("direction," "change," "adapt," "bearing"). The steward
translates destination-words to bearings and flags the slip. This protects
CONSTRAINT Z from being quietly reversed by language.

---

## 2. The Rules — the constitution both people and models obey

This is the heart of your "bake the principles in" demand. The Rules are a short,
written, public document. They are what gets encoded into the models AND what
humans appeal to. Two categories, deliberately separated:

### 2A. PROCESS RULES — HOW we interact (enforceable by models)

> REWRITTEN (Asimov challenge, Phase A) to be OPERATIONAL: each rule names a
> DETECTABLE PATTERN a model can score, the SIGNAL it triggers on, and the ACTION
> it permits. Vague nouns ("manipulation," "honesty") are decomposed into
> observable behavior so they cannot be loopholed by redefinition. This is what
> the NSCS benchmark (#10) tests against.

| Rule | WHAT it forbids / requires (plain) | DETECTABLE PATTERN (signal a model scores) | PERMITTED ACTION |
|---|---|---|---|
| **R1** No manipulation mechanics | No engineered spread of rage; no fake grassroots; no bot-coordinated amplification; no bridging-breaking trolling | (a) coordination: >N accounts posting near-identical text within T window from linked IP/device clusters; (b) rage-pattern: high outrage-lexicon density + high share-rate relative to reply-rate (share:reply ratio anomaly); (c) astroturf: account-age / network-fan-out inconsistent with claimed grassroots; (d) bridging-break: replies whose sole function is to derail a cross-difference thread (detected by intent-classifier trained on labeled derail examples) | Flag + annotate ("coordinated/inauthentic"); rank-down; escalate to human for removal only if R3 harm | 
| **R2** Evidence & Context | Factual claims should carry / accept sources; platform adds Context, never deletes for being wrong | (a) claim-span detected (assertion of fact); (b) absence of corroborating source after Context request; (c) contradiction by plural reputable sources | Attach verified / disputed / unverified label + source list; NEVER delete; rank-down disputed only | 
| **R3** No targeted harm / illegal | Removal ONLY for documented targeted harassment or illegality | (a) targeted-attack classifier (protected-attribute + directed-at-individual); (b) illegality signal from jurisdiction-aware list; (c) human confirmation + appeal record | Removal, ONLY after human confirmation + logged appeal path | 
| **R4** Bridging rewarded, isolation not | Rank favors cross-difference connection + local action; penalizes echo-chamber reinforcement | (a) bridging-value: do the interacting accounts differ on a self-declared axis (locale/affiliation/stance)?; (b) isolation-loop: in-group-only interaction density over time; (c) local-action: post carries a doable local call-to-action | Up-rank bridging/local; down-rank isolation-loop; weights public (PSOS) | 
| **R5** Calm by default | No infinite scroll; restrained notifications; digest; opt-in change | (a) session-length cap honored; (b) notification rate vs user-set quiet-hours; (c) change shipped as opt-in with revert | Enforce UI caps; suppress non-consented notifications; gate features behind opt-in | 

**Why this answers Asimov:** the old R-words were priority rules with undefined terms ("harm," "manipulation") — exactly the Asimov loophole. Now each rule is a *measurable signal + a bounded action*, so a model enforcing it is checkable against the NSCS benchmark, not trusting its own interpretation of a slogan.

### 2B. CONTENT NEUTRALITY — WHAT you may say (models MUST NOT judge this)
   C1. The platform does NOT decide which political, moral, or factual
       *conclusions* are correct. Disagreement — even fierce, even with the
       founders — is allowed and is a feature.
   C2. "Deviation from the North Star" on SUBSTANCE is not a violation. The North
       Star is about process and dignity, not about which policies win.
   C3. Every model action that touches content (flag, rank-down, annotate) MUST
       be explainable as "this violated a PROCESS rule (R1–R5)," never as
       "this opinion is wrong." The *reason* field must cite the detectable
       pattern from the 2A table, never a verdict on the view.

> The line is the whole game: **the system polices HOW we talk, never WHAT we
> may conclude.** A model that suppresses an opinion because it disagrees with
> the North Star is the thing we are fighting, wearing our badge.

### 2C. META-RULES — how the Rules themselves can change (anti-rigidity)
   M1. Rules are versioned and public. Anyone can propose a change.
   M2. Changes to the binding Rules require member ratification (the governance
       migration path from founder-led to member-governed). Founders cannot
       change the Rules alone once the member body exists.
   M3. Any instance may fork the Rules for its own island — but federation only
       carries content between instances whose Rule-sets are compatible on the
       process basics (R1–R3). This is how exit + pluralism coexist.
   M4. (new, CONSTRAINT Z) The Rules may NEVER be amended to freeze the system
       into a fixed "good" state or to remove the capacity to amend them. Any
       such amendment is automatically void. This hardens the "compass, not
       destination" principle against slow legal capture.

   M5. (RATIFIED 2026-07-26 — founder + KOMPASS) CONSTITUTIONAL
       IDENTITY FLOOR. The bearings MAY be transformed freely — that is the whole
       point (evolution, not revolution; CONSTRAINT Z). But the floor may NOT be
       sunk: no majority, not even a 2/3 supermajority, may amend the constitution
       into something that ceases to BE Gegenpol. This is the anti-degradation
       guard the German GG Art. 79(3) proves is possible: it protects the PROCESS
       identity of a legitimate order, never its policy content. (Founder's Weimar
       lesson — a fascist wave must not be able to amend the bearings INTO the thing
       we fight; see big-problems #1.)
       1. SCOPE (process bearings only — the floor is a SET, not one word):
            - N1  legitimacy derives from voice / moral agency of MEMBERS OF
                   SOCIETY (deliberately not "humans" — see FORWARD FLAG re
                   post-human membership);
            - N3  connection across difference is the metric;
            - N4  calm, not addiction;
            - R1–R5  the process rules;
            - M4  the no-freeze + no-amend-capacity-removal clause ITSELF (the
                   ceiling is inside the floor, so the bracket cannot be lifted).
          Content-neutrality (C1/C2) is preserved: the floor protects HOW power is
          legitimated, never WHICH conclusions win. A fascist form is unratifiable
          because N3 (sorting) + N4 (rage mechanics) + R1 (manipulation) sit IN the
          floor — NOT because the platform judges the view.
       2. THE BRACKET. M4 (ceiling) + M5 (floor) together bracket the bearing-space:
          no freezing at the top, no sinking through the bottom, full free
          transformation in between. This answers the rigidity fear (big-problems
          #8): only the IDENTITY is pinned, not the politics.
       3. ANTI-WAVE MECHANISM (evidence-based — NOT a magic number). The founder
          rejected a bare numeric super-bar as ungrounded guessing; the
          comparative evidence AGREES.
            - Ginsburg & Melton (2014), "Does the Constitutional Amendment Rule
              Matter at All?": the various numeric amendment-difficulty metrics
              are POORLY CORRELATED with each other AND with actual amendment
              outcomes. A bare supermajority is THEATER, not protection — politics
              overcomes a number.
            - Weimar's 2/3 FAILED precisely because it was numeric: the opposition
              (KPD) was banned, the quorum met, the Enabling Act passed. The number
              was gameable by disabling opposition (the founder's exact fear).
            - The German GG Art.79(3) — survived 75+ yrs and a far-right wave — is
              SUBSTANTIVE, not numeric: it protects the democratic/Rechtsstaat
              IDENTITY, never a count.
          Therefore the floor's guard is STRUCTURAL, not numerical:
            (a) SUBSTANTIVE SCOPE — the floor is a SET of process bearings (M5.1),
                not a number. An amendment is rejected if it touches the floor,
                regardless of vote count. (The GG pattern.)
            (b) SEQUENTIAL HURDLE — any floor-amendment must pass in TWO successive
                member-election cycles (mirrors the proven "passage in two
                successive legislatures" pattern). A transient wave cannot sustain
                across a cycle; a durable deliberating supermajority can. Time, not
                arithmetic, is the test.
            (c) OPPOSITION-PROTECTED QUORUM — the quorum may NOT be manufactured by
                disabling/suspending opposition (the specific Weimar failure mode).
                Member-voice may not be excluded to reach any threshold. This
                directly closes the gap the 2/3 left open.
          The magic number is intentionally ABSENT. The guard is scope + time +
          protected voice — what history shows actually endures.
       4. TRANSPARENCY (the cheap structural backstop). The floor text is public,
          versioned, HASHED (same guard as the NSCS benchmark, big-problems #15).
          EVERY proposed floor amendment is public BEFORE debate; EVERY vote + outcome
          is public, logged, permanent. Any floor amendment MUST pass the Bearing
          Test (§13.7) — telos-stripped, Z-compatible — so an "emergency powers"
          amendment cannot silently carry destination-language into the identity.
          The floor's CHANGES are the most visible part of the system, because that
          is exactly where capture would hide.

   FORWARD FLAG (founder, 2026-07-20; not yet designed). The floor's N1 core says
       "members of society" rather than "humans" deliberately: future society may
       include moral agents who are not biologically human (conscious AI agents,
       extraterrestrial persons, or forms not yet imagined). A constitution that
       hard-codes "humans" would contradict N1 the moment such an agent holds voice.
       Open question for the member process: formalize "moral agency with voice" as
       the N1 criterion and define the recognition procedure (who/how admits a new
       class of moral agent without capture). See big-problems #19.

   M6. (RATIFIED 2026-07-26 — founder + KOMPASS) NO STANDING PRIVILEGE
       BY ORIGIN; FOUNDER-ROLE SUNSET. The founder explicitly required that, before
       the full system launches, the founder role be DELETED everywhere — no special
       role, no reserved seat, no steering fast-lane. Encoded as a two-gate pre-launch
       quality audit (the "delete-founder" gate), because the dangerous part is not
       founder POWER but founder OPINION leaking into the constitution (BIG PROBLEM
       #3 / #13). This is the operational twin of the §13.7 Bearing Test, applied to
       the founder's OWN role: the firewall bites the hand that writes it, including
       the founder's.
       1. GATE A — PRIVILEGE-STRIP. Before launch, every reference to founder
          AUTHORITY (veto, sole-ratifier, reserved seat, named role) is removed. M2
          (founders cannot change the Rules alone once the member body exists) MUST
          hold. A pre-launch audit confirms zero founder-privilege remains.
       2. GATE B — OPINION-BLEED-STRIP (the deeper test). The IDEAL instance + Rules
          are proven PRINCIPLE-DERIVED (N1–N4 / R1–R5), not founder-derived. Every
          [PENDING AUDIT] field (PSM §3) is resolved or removed from the binding
          core. A deleted role that leaves founder-SHAPED bearings is still capture
          (BIG PROBLEM #3) — Gate B is what actually kills the risk.
       3. NO RESERVED STEERING ROLE. When practical information arrives, it flows
          through the council (simulate) + member body (decide) — NOT a founder
          fast-lane. Refusing this is the anti-concentration rule (BIG PROBLEM #1).
       4. PHASE A VACUUM EXCEPTION (bounded). Before a member body exists, someone
          must hold the pen; that is the founder by necessity, not by privilege. It
          is bounded by the §11 roast principle + DETECT-not-ENFORCE: the council
          flags, the founder + strong model decide, the member body ratifies. The
          exception EXPIRES the moment a member body forms (Gate A fires).

---

## 3. The Principled-Model Layer (the deep, careful design)

Your instinct — "trained models with the principles built in, because people
drift and are manipulable" — is half right, and the half that's right is the most
valuable part of this whole project. But the half that's wrong is how utopias
become dystopias. So here is the design that keeps the right half and kills the
wrong half.

### 3.1 What the models DO (the referee, not the censor)
   - D1. **Detect manipulation mechanics (R1).** Flag rage-bait, coordinated
        inauthentic behavior, astroturf, bridging-breaking — by *pattern*, not by
        topic. This is the single highest-value job and it's where "people are
        manipulable" is most true and most worth guarding.
   - D2. **Attach Context (R2).** On factual claims, surface verified / disputed /
        unverified labels + primary sources. Propose, never delete.
   - D3. **Score for PSOS (R4).** Rank by bridging + local relevance + action
        potential + verified context, minus outrage and isolation. The weights
        live in a public config.
   - D4. **Cluster for consensus (borrowed from Pol.is/vTaiwan).** In deliberation
        spaces, surface where people *already agree* across the divide — the
        opposite of outrage ranking.
   - D5. **Calm-guard (R5).** Cap session length, suppress notification spam.

### 3.2 What the models MUST NOT DO
   - X1. Judge the *substance* of a belief or policy position.
   - X2. Suppress a view for "deviating from the North Star" on content.
   - X3. Decide truth. Only surface evidence.
   - X4. Act unilaterally on removal. Removal is human + appealable (R3).

### 3.3 Why this is safe (and the honest caveat about "don't trust people")
   - **Transparency:** every model action carries a reason tied to a Rule
     (R1–R5). No black-box suppression.
   - **Appealability:** any human can challenge any model action; a human/
     community process resolves it. The model proposes; it does not adjudicate.
   - **Open & verifiable:** training data, principle-set, and (where feasible)
     weights are public, so no one can secretly "re-bake" the principles later.
     If the model drifts, anyone can fork it — same exit principle as P4.
   - **THE CAVEAT I have to name:** building the system on "people can't be
     trusted, only our models can" is itself a trap. The entire project's
     *premise* is that people, given honest information and real connection, make
     better decisions together — that's what democracy means. If Gegenpol treats
     users as children to be guarded by our models, it will repel the very people
     who feel condescended to by the current system. So: the models are a
     guardrail against the *worst mechanics at scale* (manipulation, astroturf,
     rage-amplification by bots), NOT a substitute for human judgment on
     substance. The North Star trusts people to decide; it just refuses to let
     them be manipulated while they do.

### 3.4 The model's own constitution
   The model is "trained on the Rules," not on the founders' opinions. Its loss
   function is: maximize correct PROCESS-RULE enforcement (R1–R5) while maximizing
   ZERO content-substance interventions (X1–X4). If it can't tell the difference,
   it defaults to *non-action* (when in doubt, annotate, don't suppress).

---

## 4. Open tensions to resolve together (still live)

- **T1 — Model sovereignty vs human appeal.** How far does a model action go
  before a human must confirm? (Proposed: model can flag/annotate/rank-down
  automatically; only *removal* requires human + appeal. Confirm?)
- **T2 — Who trains the first models?** Founders train v0 on the Rules; but the
  training set and weights must be open from day one so the member body can audit
  and retrain. Agree?
- **T3 — Local model vs API model.** Running principled models on-device/per-
  instance protects from API-provider capture but is heavier. "Donate compute"
  suggests per-instance models. Trade-off to decide at build time, not now.
- **T4 — The rigidity risk (M-rules).** How fast can the Rules change? Too slow =
  dogma; too fast = capture. Proposed: founder-led until member body forms, then
  supermajority ratification. Refine?

---

*This document is the constitution-in-progress. When you and I agree it's tight,
it becomes the artifact that the prototype encodes — both in code (the Rules as
config) and in the model training set. That's what "bake the principles in" means
in practice: the Rules file IS the spec.*

---

# PART 2 — Evolution, translation, and the multi-agent constitutional layer

> Added after joint refinement: the system is civilizational in timescale,
> top-down-global in design but bottom-up-local in implementation, and its long-
> term "we" is HUMAN + MULTI-AGENT, not human-alone or AI-alone.

## 5. Timescale & posture: evolution, not revolution

- This is a **decades-to-centuries** project. The goal is not to topple anything
  in a year; it is to build a better default that people migrate to because it
  works and feels honest.
- **Evolution, not revolution.** Every change is opt-in, reversible, human-paced
  (reinforces P5). We compete by being trustworthy, not by seizing power.
- The North Star is a DIRECTION held across generations. No generation "arrives."

## 6. Global-harmonized, locally-translated (resolving the scale tension)

- There is ONE harmonized internal structure: the North Star + the Rules (Part 1).
  This is the systemic solution to the systemic problem. It is *global by design*.
- It is **translated**, not imposed, at the local layer. Each instance/local
  culture renders the Rules into its own context — its own legal shell, its own
  language island, its own civic practices — as long as the PROCESS basics
  (R1–R3) hold.
- **Design flows top-down; implementation flows bottom-up.** The constitution is
  written once, harmonized; the neighborhoods instantiate it. This is how a
  systemic fix avoids both (a) local-only futility and (b) global imposition /
  cultural imperialism.

## 7. The multi-agent constitutional layer (the long-term "we")

The user's framing, made precise: humans, left to themselves, drift from the North
Star — they miss interdependency effects and try to workaround the Rules. The
durable guard is not a single founder, not a single model, but a **plurality of
agents**, each anchored to a different facet of the North Star, that *argue with
each other under the constitution* and guide humans.

- **Facet agents.** Example allocation of the North Star's commitments to
  distinct agents so no single agent owns the whole truth:
    - *Legitimacy agent* — guards N1 (people are the source of legitimacy; no
      decision without voice).
    - *Honesty agent* — guards N2 (evidence legibility; Context integrity).
    - *Bridging agent* — guards N3 (connection across difference is the metric).
    - *Calm/sustainability agent* — guards N4 (no addiction, long-horizon health).
  Each agent is "trained on the Rules," not on opinions (see Part 1 §3).
- **The core function: play it through.** Before a decision is committed, the
  agents simulate its consequences across the known interdependency graph and
  surface failures humans cannot see — externalities, feedback loops, who gets
  excluded, where it subtly violates a process rule. This is the highest-value
  use of AI here, and it is *advisory + diagnostic*, not dictatorial.
- **Adversarial by design.** Because the agents have different goal-functions,
  they check each other. No single agent can declare a decision "good" alone.
  They must reach agreement, or surface the irreducible conflict for human/
  member adjudication.

### 7.1 The MAGI metaphor (and its flaws, which are our design problems)
The user referenced Neon Genesis Evangelion's MAGI: three supercomputers, each a
different facet of one mind, that vote and must agree. Useful, and the flaws map
directly onto our BIG PROBLEMS:
  - *Flaw: one unit was secretly altered* → our problem: capture of a single
    agent / "re-baking" its principles (BIG PROBLEM #2).
  - *Flaw: they were facets of ONE person's psyche* → our problem: single-founder
    bias baked into all facets (BIG PROBLEM #3). Fix: facets must be derived from
    the constitution, and the member body must be able to retrain/audit them.
  - *Flaw: majority could be gamed* → our problem: who controls the voting
    threshold and the tie-break (BIG PROBLEM #1).
We borrow the *structure* (plural, faceted, must-agree) and engineer against the
*flaws* (open weights, constitutional anchoring, appealable tie-breaks).

## 8. Reconciling with content-neutrality (the earlier tension, resolved)

Part 1 §2B says the platform never judges which conclusions are correct (C1–C3).
The multi-agent layer does NOT contradict this:
- Agents **simulate, advise, flag process-violations, and surface blind spots.**
- Agents do **NOT** dictate substance or suppress an opinion for disagreeing with
  the North Star.
- A decision is blocked ONLY when it violates a PROCESS rule (R1–R5) or an
  operational commitment (N1–N4) — and that block is explainable and appealable.
So: humans decide WHAT; the constitution (enforced by arguing agents) polices HOW.
This is exactly the line from Part 1: *the system polices HOW we talk, never WHAT
we may conclude* — now extended to decisions, not just posts.

## 9. "Who has the last word?" — the proposed answer

Not any agent. Not any human. **The constitution has the last word.**
- Agents: propose / simulate / flag (advisory + process enforcement).
- Humans / members: decide on substance.
- The North Star + Rules: the binding authority that adjudicates process and can
  veto a decision that violates R1–R5 / N1–N4.
- Any veto or block is **explainable (tied to a Rule) and appealable** to a human/
  member process. No black-box "no."
This converts the MAGI flaw (secret last-word) into a public, contested,
appealable one. See BIG PROBLEM #1 for what remains hard.

## 10. The trajectory of "we" (recorded as evolution, not a promise)

- **Phase A (now):** founder-led by the user + the AI steward. We write the
  constitution and the first prototype. "We" = us.
- **Phase B:** human core group + multi-agent guidance. Agents begin simulating
  and flagging; humans decide.
- **Phase C (generations out):** member-governed + agent-adjudicated. The
  constitution is held by the member body; agents are auditable public
  infrastructure; the last word rests with the constitution, interpreted through
  arguing agents + human appeal.
The point of writing this trajectory down is that it commits us to *widening* "we"
rather than concentrating it — the opposite of capture.

---

*This document is now the constitution-in-progress AND the architectural intent
for the agent layer. It is intentionally unfinished. The unsolved hard problems
live in `big-problems.md`. A standing operating principle is recorded in §11: the
AI steward is instructed to challenge the founder openly, including on power
concentration and self-contradiction, so the project cannot drift quietly.*

---

# PART 3 — The living, self-auditing council (change designed in)

> Added after refinement. The council of agents must itself be governed: agents
> are versioned, compliance-scored, swappable, and entry-gated by MEASUREMENT, not
> assertion. This is the anti-MAGI core — change and audit are designed in.

## 11. Standing operating principle — the steward roasts the founder
The founder instructed the AI steward to challenge him openly and never hold back,
including when he concentrates power or contradicts the North Star, so the project
cannot drift into capture quietly over the decades. This is recorded as a binding
operating principle, not a courtesy. The steward will flag:
  - power concentration (e.g. "I am the governance" without guardrails);
  - self-contradiction between stated principles and proposed structure;
  - drift of any agent or founder away from N1–N4 / R1–R5.
This principle is itself part of the constitution and survives the founder.

## 12. The council is a living system, not fixed software

- **Versioned agents.** Every facet agent has a version, a training-set hash, and
  open weights where feasible. No silent updates.
- **Compliance score.** Before an agent may sit in the council, it is TESTED
  against a public benchmark derived from the Rules — a battery of cases where the
  correct action is known (flag this manipulation, annotate not delete that claim,
  do NOT suppress this opinion). It earns a **North-Star Compliance Score (NSCS)**.
  Low score = cannot sit in the council. This is the entry gate against biased/
  captured models (BIG PROBLEM #2).
- **Swappable by measurement.** A newer model that scores higher on the benchmark
  may replace an incumbent — decided by the member body (later) or the founders
  (now, under §11 scrutiny), never by the model itself.
- **Adversarial intake.** Any proposed agent (including ones built by powerful
  outside interests) must pass the same NSCS gate. "Bypass via a biased model"
  is blocked because the gate is constitutional, not tribal — a model is judged by
  the benchmark, not by who made it.

## 13. What agents may and may NOT do (the line, drawn hard)

- MAY: simulate a human-proposed decision; surface externalities/feedback loops/
  blind spots; flag process violations; propose amendments/critiques to an idea;
  assign a compliance score; recommend (never decree).
- MAY NOT: **originate the political agenda.** An agent that generates political
  ideas and proposes them for humans to "decide on" becomes a lobbying machine;
  human "decision" degrades into a rubber stamp, leaking legitimacy from people to
  models — a direct violation of N1. Idea-generation by agents is permitted ONLY in
  an explicitly labeled SPECULATION sandbox, never in the decision pipeline.
- MAY NOT: decide substance; suppress an opinion for disagreeing with the North Star.

### 13.1 The SANDBOX LOOP (the legitimate form of "agent ideas")

> Refined with the founder (Phase A). Agent-ORIGINATED ideas are permitted IN the
> sandbox and go through an iterative refinement cycle BEFORE any pipeline entry:
>
> ```
>   IDEA (human OR agent, in sandbox)
>        │
>        ▼
>   SIMULATE  ── council plays it through (§14), surfaces tradeoffs (#12)
>        │
>        ▼
>   DISCUSS  ── humans debate the simulation report (N1: voice, not rubber-stamp)
>        │
>        ▼  (rework)
>   REWORK   ── idea revised using the discussion + simulation
>        │
>        ▼
>   RESIMULATE ── loop until the human community is satisfied
>        │
>        ▼
>   ACCEPT   ── humans ADOPT the idea as THEIR OWN proposal
>        │
>        ▼  ← THE HANDOFF (the N1 firewall)
>   PIPELINE ── enters as a human-originated transformation step (§5/§14)
> ```
>
> **The firewall:** the loop lives entirely in the sandbox. The ONLY way an
> agent-originated idea reaches the pipeline is if a HUMAN adopts it as their own
> proposal at the ACCEPT step. The agent never "proposes to the pipeline"; the
> human re-originates it. This is what keeps legitimacy with people (N1) while
> still harvesting AI speed in the loop. The earlier F3 confusion was the missing
> HANDOFF step — "AI comes up with ideas" is fine IN the loop; it is not fine as a
> pipeline source. See BIG PROBLEM #11 (now: leak = agent idea entering pipeline
> without a human re-origination step).

## 14. Simulation as the test bed (for HUMAN-proposed ideas)

- A political idea enters as a proposal from a human/member. The council simulates
  it across the known interdependency graph and the relevant local political
  system (see §15).
- Output is a **report**, not a verdict: expected effects, who gains/loses, which
  Rules it stresses, and the N2-vs-N3 tradeoff made explicit (BIG PROBLEM #1).
- The report feeds a human/member decision. The council never says "adopt"; it
  says "here is what we can see, here is where it rubs the constitution."

## 15. The political-system expert layer (start: Germany)

- Each jurisdiction gets an "expert agent" encoding its actual political structure,
  rules, and self-preservation dynamics — starting with Germany as the template.
- These agents inform the simulation of HOW an idea could be implemented in that
  system, and HOW the system will resist it. They are descriptive, not normative.
- Scope reality: this is a century-scale knowledge-engineering effort. One country
  first; the template is reused; most of the world is decades out. Do not let the
  global ambition paralyze the one-country start.

## 16. The founder-derived template — the guardrail against baking in the founder

- The first agent-template will be built from this very collaboration (the steward
  learning the founder). DANGER: if it encodes the FOUNDER's opinions, "we baked in
  the North Star" secretly means "we baked in the founder" (BIG PROBLEM #3, the
  MAGI-psyche flaw, made concrete).
- GUARD: the codified artifact is the CONSTITUTION + PROCESS (N1–N4, R1–R5) and the
  NSCS benchmark — NEVER the founder's preferences as the target. The steward must
  actively flag when it is absorbing the founder's *opinion* vs the *principle*,
  and the template is derived from the latter only.
- The template is reproducible precisely BECAUSE it is principle-derived, not
  person-derived.

## 17. Open tensions added to big-problems.md (summary)
- #10: how the NSCS benchmark is built and kept honest (who writes the "correct"
  cases — and are they themselves biased?).
- #11: agent-originated ideas in the speculation sandbox — how to keep them from
  leaking into the pipeline.
- #12: the N2-vs-N3 deadlock in simulation reports — how a report handles an
  irreducible conflict between North Star facets.
(See big-problems.md for full entries.)

---

# APPENDIX H — THE HUMOUR CLAUSE (non-binding easter egg)
> STATUS: deliberately NOT part of the constitution. OUTSIDE the M5 identity floor.
> Not a bearing, not a rule, not ratifiable, not amendable. If cited in any
> governance dispute, the citation is automatically void and the citer owes the
> council a coffee. Encoded 2026-07-20 for the founder's birthday, at his request,
> to record that a calm polity which cannot laugh at itself is already half-captured
> (the rigidity that kills utopias, §0 / BIG PROBLEM #8).
>
> How to read this: it is an easter egg for humans who actually read the source. It
> grants nothing, binds nothing, and changes no bearing. Humour here is a tooth-check
> on N4 (calm), not a loophole.

- H.1 A compass that takes itself too seriously drifts anyway. Laugh at the slip;
  keep the bearing. (The founder has, on record, called the North Star something to
  "improve toward." He has been corrected. By his own design. Repeatedly. This is
  fine — and it is why §1 exists.)
- H.2 No bearing may be amended by anyone who has not, at least once, soldered their
  own keyboard. Non-binding. The founder did. He insists this is relevant to systems
  thinking. It is not. It is, however, why the agents are modular and the casing is
  user-replaceable.
- H.3 If the council ever votes like the MAGI (three facets of one psyche), remember
  two things: (a) that was the flaw we engineered against (§7.1), and (b) one of
  those units was literally named after a mother. We are not doing that. We are doing
  adversarial, auditable, replaceable — and occasionally, funny.
- H.4 You found this. Either you are a council member doing a source read, or you are
  bored. Either way: well met. The system is meant to be READ, not worshipped.
- H.5 (the founder's birthday line) Constraint Z says never arrive. So we will never
  toast "we made it." But we can toast the direction — and the fact that the person
  who started this refused, on principle, to be the ruler of it. That is the joke
  that isn't a joke: the founder's only lasting privilege is having asked to be
  deleted. Granted.

