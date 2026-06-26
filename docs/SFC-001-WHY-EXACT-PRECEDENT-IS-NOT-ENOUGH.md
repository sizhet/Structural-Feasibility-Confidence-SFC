# SFC-001 — Why Exact Precedent Is Not Enough

## From Repetition to Structural Feasibility Confidence

# 1. Introduction

A large portion of real intelligence does **not** operate in the comfortable regime of exact repetition.

A craftsman is asked to build a piece he has never built before.
An engineer is asked to estimate a system she has never implemented end-to-end before.
A research team is asked whether a new technical direction is feasible before the final code, experiment, or product exists.
A task planning system must decide whether a target task is likely achievable even though its exact execution trace has not yet been observed.

In all of these cases, the critical question is not:

> “Has the exact same task already been completed before?”

but rather:

> “Given what has already been built, verified, understood, and practiced, how much confidence do we have that this new target is feasible?”

This repository studies that second question.

We call the resulting framework **Structural Feasibility Confidence (SFC)**.

SFC is motivated by a simple but far-reaching observation:

> **Exact precedent is often too strict a requirement for real-world intelligence.**
> Brains, craftsmen, engineers, organizations, and future AI agents must regularly act, plan, quote, commit, and allocate resources **before** exact precedent exists.

The point of SFC is not to replace direct proof or successful execution.
The point is to explain how intelligent systems operate in the much larger and more common region between:

* **fully confirmed repetition**, and
* **pure speculation**.

That intermediate region is where much of practical intelligence lives.

---

# 2. The Limitation of Exact Precedent

Suppose a craftsman has built one hundred standard cabinets.
Now a client asks for a new piece:

* different dimensions,
* different wood,
* a modified internal structure,
* and a decorative style the craftsman has not executed in exactly that combination before.

If we require **exact precedent**, then the answer must be:

> “No confidence is possible until the exact piece has already been built.”

But this is clearly wrong.
The craftsman is not operating in a vacuum. He already possesses:

* tool familiarity,
* material knowledge,
* joint construction experience,
* finishing experience,
* prior solutions to similar structural constraints,
* estimates of time, risk, and rework,
* and a sense of which parts are routine versus novel.

So although the target is new, the target is **not unsupported**.

The same pattern appears everywhere:

* a software engineer estimating a system variant she has not built before,
* a scientist judging whether an experiment is within reach,
* a surgeon deciding whether a rare case still lies within a known procedure family,
* a task planner proposing a new Task Calling Graph before every Action Calling Graph has been fully executed.

In all of these cases, exact precedent is too blunt a criterion.
It collapses the difference between:

1. a target that is **new but structurally adjacent** to many validated tasks, and
2. a target that is **genuinely unsupported**.

SFC exists to preserve that difference.

---

# 3. Real Intelligence Works in the Space Between Repetition and Speculation

A useful way to frame the problem is to distinguish three broad regions.

## 3.1 Confirmed Region

The task has already been completed before, or a very close equivalent has been completed repeatedly.
The system has direct evidence for:

* execution path,
* cost,
* duration,
* quality bounds,
* common failure modes,
* and recovery procedures.

This is the regime of **confirmed feasibility**.

## 3.2 Extension Region

The target has **not** been completed in exactly the same form, but it lies near already validated structures:

* known subtasks,
* known components,
* known action clusters,
* known tunnel families,
* known neighboring trajectories,
* and known mechanisms.

This is the regime of **extension feasibility**.

The target is new, but not unsupported.
Confidence here is not based on exact repetition. It is based on **structural support**.

## 3.3 Speculative Region

The target is too far from validated structures, or too many critical pieces are missing.
Local evidence is weak, bridgeability is unclear, and failure modes are poorly understood.

This is the regime where confidence should drop sharply, and commitment should become conservative.

---

# 4. Why This Matters for Brain Intelligence

The ability to operate in the extension region is not a niche engineering trick.
It is one of the ordinary powers of practical intelligence.

A brain that can only repeat previously executed actions is not a robust intelligence system.
It is a replay system.

Real intelligence must do more than replay. It must be able to answer questions like:

* “Can I probably do this?”
* “How different is this from what I already know?”
* “Which parts are routine, and which parts are risky?”
* “How much buffer should I add?”
* “Do I need a prototype first?”
* “Can I commit fully, or only stage-by-stage?”

These are not secondary questions.
They govern real decisions in education, craftsmanship, engineering, research, planning, and survival.

A hunter deciding whether a new path is traversable, a mechanic deciding whether a new repair is within reach, or a child deciding whether a toy can be assembled from known parts all rely on some form of structural feasibility judgment.

SFC therefore belongs not only to software planning or project estimation.
It belongs to the broader study of **ordinary brain intelligence**.

---

# 5. Why This Matters for AI

The same issue appears in AI systems, especially when moving from narrow execution to more autonomous planning.

An Action Calling Graph may record what has already been executed.
But a Task Calling Graph often needs to exist **before** all of its action paths have been fully validated.
If we forbid that, the system can only formalize what is already complete, and cannot act as a planner.

This creates a core challenge:

> **How can a system judge the feasibility of a task graph that is not yet fully backed by executed action graphs?**

That challenge is not an implementation detail.
It is one of the main motivations for SFC.

Without a framework like SFC, planning systems are pushed toward two bad extremes:

1. **Over-conservatism**
   Only tasks with exact precedent are accepted.

2. **Hallucinated confidence**
   Tasks are accepted without disciplined structural support.

SFC is intended to formalize the middle ground:

* neither blind refusal,
* nor unsupported optimism,
* but **structured confidence grounded in prior tunnels, validated subgraphs, reusable modules, and local bridgeability**.

---

# 6. The Core Shift: From “Have We Done It?” to “How Well Is It Structurally Supported?”

The main conceptual shift of this repository is simple.

Instead of treating feasibility as a binary question answered only by exact precedent, SFC asks:

* How much of the target lies inside already confirmed structures?
* Which subparts are already covered?
* Which gaps are small and bridgeable?
* Which missing parts require new construction?
* How far is the target from known tunnel families?
* What is the expected cost of extension?
* What is the risk if extension fails?

This changes the unit of analysis.

The unit is no longer just **the exact historical task instance**.
The unit becomes the broader **structural neighborhood** around the target.

That neighborhood may include:

* previously completed tasks,
* reusable operators,
* nearby trajectories,
* solved subtasks,
* known failure-and-recovery routines,
* and mechanism-level understanding of how the target works.

This is the space in which SFC operates.

---

# 7. SFC as a Response to a Common Blind Spot

Modern technical culture often oscillates between two misleading ideals.

The first ideal is **proof by exact repetition**:

> “If it has not been done before in exactly this form, confidence is unjustified.”

The second ideal is **confidence by vague intuition**:

> “It feels adjacent enough, so we should just proceed.”

SFC rejects both.

It does not reduce feasibility to exact precedent.
But it also does not replace evidence with vibes.

Instead, it asks a more disciplined question:

> **What is the structure of support around the target?**

That support may be strong, weak, partial, anisotropic, modular, or brittle.
It may support some variations and not others.
It may justify a full commitment, a staged commitment, or only a prototype.

In that sense, SFC is not just a theory of confidence.
It is a theory of **confidence with structural accountability**.

---

# 8. What This Repository Proposes

This repository develops a framework around four closely related ideas.

## 8.1 Structural Feasibility Confidence (SFC)

A general framework for judging how feasible a target is, not only from exact prior completion, but from the surrounding structural evidence.

## 8.2 Confirmed vs Extension Confidence

A distinction between:

* **confirmed feasibility confidence** — grounded in direct execution history, and
* **extension feasibility confidence** — grounded in structural support around a not-yet-exactly-completed target.

## 8.3 Patchwork Feasibility Proof

A proof-like justification assembled from multiple partial but relevant sources of support:

* validated subtasks,
* reusable modules,
* neighboring trajectories,
* mechanism-level understanding,
* and recoverable gap-bridging strategies.

## 8.4 Confidence Thickness

A way to describe how far a known tunnel, skill family, or task family can be extended with meaningful confidence before it becomes speculative.

---

# 9. The Scope of the SFC Program

The SFC program is intentionally cross-domain, but structurally unified.

Its target examples include:

* **craftsmanship** — quoting and delivering work not previously executed in exactly the same form,
* **engineering** — estimating unseen implementations from reusable architecture and prior projects,
* **research** — committing to new technical directions based on prior conceptual and experimental support,
* **Task Calling Graphs** — proposing task structures before every action path has been fully verified,
* **AI agents** — deciding when to accept, decompose, prototype, or refuse tasks.

The common problem is the same:

> **How should an intelligent system act when the target is not fully confirmed, but is not unsupported either?**

---

# 10. Conclusion

Exact precedent is important, but it is not enough.

If intelligence were restricted to exact repetition, much of ordinary planning, engineering, craftsmanship, and adaptive action would become unintelligible.
Real systems routinely operate in a broader regime where targets are partially new, partially supported, and unevenly connected to prior success.

Structural Feasibility Confidence is an attempt to study that regime directly.

It is an attempt to explain:

* how feasibility can be judged without exact precedent,
* how confidence can remain disciplined rather than speculative,
* how extension can be supported by structure rather than wishful thinking,
* and how brains, engineers, craftsmen, and future AI systems may all rely on related mechanisms when facing unseen but adjacent tasks.

The rest of this repository develops that framework.

---

# Key Takeaways

* **Exact precedent is too strict** for much of real intelligence.
* Real systems often need to judge tasks that are **new but structurally adjacent** to validated ones.
* SFC studies how feasibility confidence can arise from **confirmed tunnels, validated subgraphs, reusable modules, neighboring trajectories, and mechanism understanding**.
* The core distinction is between **confirmed feasibility confidence** and **extension feasibility confidence**.
* This problem matters for both **ordinary brain intelligence** and **future AI planning/runtime systems**.
