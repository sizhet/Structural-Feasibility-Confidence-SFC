# SFC-004 — Function Tunnel Confidence Thickness

## Confidence Zones, Extension Boundaries, and the Shape of Feasible Reach

# 1. Introduction

Structural Feasibility Confidence (SFC) explains how an intelligent system can form disciplined confidence about a target that has not been completed before in exactly the same form.
Patchwork Feasibility Proof explains how that confidence can be supported by multiple partial but relevant sources of evidence.

This document introduces a third core concept:

# **Function Tunnel Confidence Thickness**

Function Tunnel Confidence Thickness describes **how far** a known tunnel, skill family, task family, or capability region can be extended with meaningful confidence before the target becomes speculative.

In plain terms, it asks:

* How far can a craftsman stretch beyond already completed commissions?
* How far can an engineer commit beyond already implemented systems?
* How far can a Task Calling Graph extend beyond already validated Action Calling Graphs?
* How far can a future AI system safely bridge a gap before it is no longer operating inside supported territory?

The answer is almost never binary.
A system rarely moves from “fully safe” to “fully impossible” in one step.
Instead, confidence tends to weaken gradually and unevenly as the target moves away from the core of already confirmed structure.

Function Tunnel Confidence Thickness exists to describe that graded and directional extension capacity.

# 2. From Tunnel Existence to Tunnel Thickness

A function tunnel, in the broad sense used here, is a structured family of workable trajectories, routines, decompositions, or transformations that preserve a viable path toward a class of outcomes.

A tunnel may be narrow or wide, rigid or flexible, local or general.
But once the idea of a tunnel is introduced, a new question immediately appears:

> Is the tunnel only valid for the exact points already traversed, or does it also support nearby unseen targets?

That question cannot be answered merely by saying “the tunnel exists.”
It requires an account of **tunnel thickness**.

A tunnel with no thickness would be a degenerate object:

* valid only at exact replay points,
* useless for extension,
* and unable to support real planning under novelty.

Real intelligence, however, depends precisely on the fact that tunnels usually possess some amount of **local extendability**.
A cabinetmaker’s skill tunnel is not one cabinet wide.
An engineer’s architecture tunnel is not one deployment wide.
A child’s assembly skill is not one toy wide.
And a meaningful task planning system cannot operate if every task edge requires exact historical execution before it may be represented.

Thickness names this extendability.

---

# 3. Definition of Function Tunnel Confidence Thickness

## **Function Tunnel Confidence Thickness**

**Definition.**
Function Tunnel Confidence Thickness is the extent to which a known function tunnel, skill family, task family, or capability region can support confident execution, planning, or commitment for **structurally adjacent unseen targets**, rather than only for already traversed targets.

It is therefore not a binary property.
It is a **thickness profile** over a structured task space.

This profile describes how confidence changes as a target moves away from:

* confirmed precedents,
* validated subgraphs,
* reusable modules,
* neighboring trajectories,
* and known mechanism support.

Thickness is therefore closely related to, but not identical with, SFC itself:

* **SFC** asks how much confidence a system has for a target.
* **Function Tunnel Confidence Thickness** asks how far a tunnel can continue to support that confidence as targets move outward.

In other words:

> SFC is a confidence judgment at a target.
> Tunnel thickness is a property of the surrounding support field that helps generate that judgment.

---

# 4. Why Thickness Matters

Thickness matters because practical intelligence does not operate only at the center of fully confirmed territory.

A system must routinely decide:

* whether a target is still close enough to a known tunnel,
* whether the current deviation is a small extension or a structural break,
* whether a quote should remain standard or include a large uncertainty premium,
* whether a task graph should be accepted as bridgeable or postponed as speculative,
* whether a gap should be attacked directly, probed first, or avoided.

Without a notion of thickness, feasibility becomes too crude.
The system can say only:

* “done before,” or
* “not done before.”

That loses the central middle region of real intelligence:

* **not yet done exactly, but still within supported reach**.

Thickness restores that region to the theory.

---

# 5. Three Core Confidence Zones

A useful first model of tunnel thickness is a three-zone picture.

---

# 6. Zone I — Confirmed Zone

## **Confirmed Zone**

The Confirmed Zone contains targets that are already directly supported by repeated or highly similar execution history.

Typical properties:

* the system has already completed these tasks or very close equivalents,
* failure modes are known,
* cost and timing are estimable with relatively low uncertainty,
* recovery strategies are available,
* commitment can be made with high confidence.

Examples:

* a craftsman repeating a standard commission,
* an engineering team deploying a familiar service template,
* an Action Calling Graph that has already been validated multiple times,
* a known procedure family in a familiar environment.

The Confirmed Zone is the core of the tunnel.
This is where confidence is strongest and least controversial.

---

# 7. Zone II — Extension Zone

## **Extension Zone**

The Extension Zone contains targets that are not exact precedents but remain structurally supported by the tunnel’s neighborhood.

Typical support sources include:

* validated subtasks,
* reusable modules,
* adjacent trajectories,
* mechanism understanding,
* recoverable bridge steps,
* and patchwork feasibility proof.

In the Extension Zone:

* the target is new, but not unsupported;
* commitment may still be justified, though often with more caution;
* quotes, plans, or acceptance decisions may include buffers, staged validation, or narrower promises.

This is the most important zone for the SFC program, because it captures the region where intelligent extension happens.

A craftsman accepts a new commission.
An engineer agrees to a novel system variant.
A Task Calling Graph is proposed before every action path exists.
A gap-bridging system decides that a missing structural link is within reach.

All of these are Extension Zone phenomena.

---

# 8. Zone III — Speculative Zone

## **Speculative Zone**

The Speculative Zone begins when the target moves beyond the region where available structural support can justify a disciplined commitment.

Typical signs include:

* too many unsupported gaps,
* weak subtask coverage,
* absent reusable modules,
* no nearby trajectories,
* shallow mechanism understanding,
* high coupling between unknown pieces,
* or catastrophic failure cost if bridging goes wrong.

In the Speculative Zone, the correct response may be:

* refuse,
* delay,
* narrow the scope,
* require a prototype,
* escalate to additional experts or tools,
* or reframe the target as a research problem rather than a deliverable.

Speculative does **not** mean impossible.
It means that the tunnel no longer provides enough thickness to justify ordinary commitment.

---

# 9. Thickness Is Not Uniform

One of the most important properties of tunnel thickness is that it is usually **anisotropic**.

That means confidence does not decay equally in all directions.

A cabinetmaker may have strong thickness along:

* size variation,
* wood species variation,
* standard drawer-count variation,

but weak thickness along:

* hidden lighting integration,
* motorized mechanisms,
* embedded electronics,
* or unfamiliar metalwork.

An AI coding system may have strong thickness along:

* CRUD backends,
* REST APIs,
* test scaffolding,
* and ETL pipelines,

but weak thickness along:

* distributed consensus,
* GPU kernels,
* compiler optimization,
* or hardware-software co-design.

A Task Calling Graph system may have strong thickness for:

* rearranging known subtasks,
* adding standard orchestration steps,
* replacing one known operator with another equivalent operator,

but weak thickness for:

* inserting entirely new task families,
* handling adversarial failure modes,
* or bridging across unknown dependency regimes.

This means tunnel thickness should not be imagined as a circle of equal radius around a known point.
It is better understood as a **directional support field**.

---

# 10. Thickness Depends on Distance, but Not on Distance Alone

It is tempting to think of thickness as just “distance from precedent.”
Distance is important, but it is not enough.

A target’s confidence thickness depends not only on how far it is from confirmed examples, but also on **what kind of distance** is involved.

Two targets may be equally distant in a naive metric sense but very different in feasibility:

* one may differ only in dimensions,
* another may differ in causal mechanism.

So tunnel thickness depends on a richer profile, including:

* distance from confirmed precedent,
* proportion of covered subtasks,
* availability of reusable modules,
* adjacency of trajectories,
* mechanism familiarity,
* bridgeability of missing pieces,
* recoverability of failure,
* and cost of extension.

This is why thickness is best thought of as a structured confidence geometry rather than a simple scalar radius.

---

# 11. Thickness and Patchwork Feasibility Proof

Patchwork Feasibility Proof (PFP) is one of the main mechanisms that allows tunnel thickness to exist in the first place.

If a tunnel had to rely only on exact replay, it would have no meaningful extension region.
Thickness becomes possible because a system can support nearby targets through a patchwork of:

* solved subtasks,
* reusable modules,
* neighboring trajectories,
* and mechanism-level understanding.

In that sense:

* **PFP explains how extension can be justified locally**, and
* **tunnel thickness describes how much of that local extension capacity the tunnel possesses overall**.

PFP is the micro-level support logic.
Thickness is the macro-level shape of the supported region.

---

# 12. Thickness and Commitment Behavior

Tunnel thickness becomes especially visible when it is projected into behavior.

A system with high thickness in a region tends to behave differently from a system with low thickness in that region.

Typical behavioral consequences include:

## 12.1 Acceptance vs Refusal

A thick region supports acceptance.
A thin region triggers caution or refusal.

## 12.2 Quote and Time Buffer

When thickness is lower, uncertainty premiums and time buffers rise.

## 12.3 Prototype Requirements

When the target lies near the edge of thickness, the system may request a prototype, dry run, or staged rollout.

## 12.4 Scope Narrowing

If the full target is outside thickness but a sub-target remains inside it, the system may accept only the narrowed scope.

## 12.5 Escalation

Thin support may trigger a request for:

* additional tools,
* collaborators,
* domain experts,
* or specialized brain units.

This is important because it shows that thickness is not only a theoretical object.
It is an operational determinant of commitment policy.

---

# 13. Thickness and Gap Bridging

Thickness is also central to gap bridging.

A detected gap is not automatically a problem of equal status.
Some gaps lie well inside supported extension territory; others sit near the boundary; others are far outside it.

Thickness helps answer:

* Is this gap bridgeable within current support?
* Does it require a local patch, a staged bridge, or a major new construction?
* Is the system still operating in extension mode, or has it drifted into speculation?

This matters because the practical question in gap bridging is rarely just “does a gap exist?”
The real question is:

> **What kind of gap is this relative to the thickness of the current tunnel?**

That is where thickness becomes algorithmically useful.

---

# 14. Thickness as a Confidence Field

A productive way to formalize the idea is to think of tunnel thickness as a **confidence field** over a task or capability space.

Let the target space contain candidate tasks, artifacts, decompositions, or trajectories.
Then a tunnel does not merely contain a set of executed points.
It also induces a surrounding field of extension support:

* stronger near confirmed cores,
* weaker near boundaries,
* and broken or absent beyond them.

This field need not be smooth, convex, or uniform.
It may be:

* thick in one dimension,
* thin in another,
* disconnected across different mechanism families,
* and sharply discontinuous at certain causal boundaries.

This is why the term **thickness** is helpful.
It preserves the geometric intuition that a tunnel is not a zero-width line, while still leaving room for highly nonuniform structure.

---

# 15. Thickness and LLM/Transformer Scoring

The idea of thickness also helps interpret some aspects of LLM/Transformer behavior.

When a model scores or ranks candidate continuations, it often behaves as if it were evaluating whether a candidate lies within a statistically supported neighborhood of prior patterns, contextual cues, and local coherence constraints.

This is not the same as explicit tunnel thickness.
The model usually lacks explicit commitment boundaries, explicit gap typing, and explicit bridgeability reasoning.

But the analogy is still useful:

* high-probability continuations often correspond to regions of dense support,
* low-probability continuations often correspond to thinner or poorly supported regions,
* and ranking behavior may be viewed as a primitive, implicit form of support-field evaluation.

In that sense, tunnel thickness can be seen as a more explicit, inspectable, and structurally grounded counterpart to statistical confidence fields already present in modern generative systems.

---

# 16. Limits of Thickness

Function Tunnel Confidence Thickness is a useful concept, but it should not be over-romanticized.

Thickness does not guarantee success.
A thick region may still contain failures.
A thin region may still be traversable by luck, genius, or brute force.

What thickness does is not eliminate uncertainty, but organize it.

It tells us:

* where extension is likely to be disciplined,
* where extension should be cautious,
* where commitment should become conditional,
* and where speculation begins to dominate.

That is already a major upgrade over binary precedent thinking.

---

# 17. Conclusion

Function Tunnel Confidence Thickness describes one of the most practical aspects of Structural Feasibility Confidence:

> not just whether a system can do what it has already done, but how far it can extend beyond that with justified confidence.

This requires more than the existence of a tunnel.
It requires a view of:

* confidence zones,
* extension boundaries,
* directional support,
* patchwork-backed local extension,
* and commitment behavior near the edge of competence.

Thickness therefore plays a central role in craftsmanship, engineering, Task Calling Graph planning, gap bridging, and future AI runtime governance.

It is the concept that turns a tunnel from a historical trace into a **field of feasible reach**.

---

# Key Takeaways

* **Function Tunnel Confidence Thickness** describes how far a known tunnel or skill family can support confidence beyond exact precedents.
* A useful first model is a three-zone structure:

  * **Confirmed Zone**
  * **Extension Zone**
  * **Speculative Zone**
* Thickness is usually **directional and anisotropic**, not uniform in all directions.
* Thickness depends on:

  * direct precedent,
  * subtask coverage,
  * module reuse,
  * adjacent trajectories,
  * mechanism understanding,
  * and bridgeability.
* Thickness strongly affects commitment behavior:

  * acceptance,
  * quoting,
  * staging,
  * scope narrowing,
  * and escalation.
* In practice, thickness turns a tunnel from a replay path into a **supported region for disciplined extension**.
