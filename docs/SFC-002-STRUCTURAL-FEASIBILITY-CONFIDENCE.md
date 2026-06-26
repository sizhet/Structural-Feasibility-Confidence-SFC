# SFC-002 — Structural Feasibility Confidence

## Confirmed Feasibility, Extension Feasibility, and the Structure of Practical Commitment

# 1. Introduction

This document introduces the central concept of this repository:

# **Structural Feasibility Confidence (SFC)**

SFC is a framework for describing how an intelligent system forms confidence that a target task, artifact, trajectory, or plan is feasible **even when that exact target has not yet been fully executed before**.

The key idea is straightforward:

> Feasibility confidence should not be tied only to exact precedent.
> It should also depend on the **structural support** surrounding the target.

That support may come from:

* prior successful executions of similar tasks,
* reusable subtasks and modules,
* neighboring trajectories in the same function family,
* mechanism-level understanding,
* and known bridge strategies for local gaps.

SFC is therefore not a theory of optimism, and not a license for hand-waving.
It is a theory of **disciplined feasibility judgment under partial novelty**.

---

# 2. A First Definition

## **Structural Feasibility Confidence (SFC)**

**Definition.**
Structural Feasibility Confidence is the confidence that a target task, artifact, trajectory, or runtime behavior is achievable by a system, where that confidence is derived not only from direct completion of the exact same target, but from the broader structural evidence available around it.

This evidence may include:

* repeated execution history of similar tasks,
* validated subtasks,
* reusable modules and action clusters,
* adjacent trajectories in the same tunnel family,
* mechanism-level understanding,
* known fallback and recovery procedures,
* and bridgeable local gaps.

SFC is therefore **structural** in two senses:

1. It depends on the **structure of prior support**, not merely on raw self-confidence.
2. It depends on the **structure of the target itself**—which parts are already covered, which parts are novel, and how those parts connect.

---

# 3. Why “Confidence” Needs Structure

The word “confidence” can be misleading if left vague.
In everyday language, confidence often means little more than a subjective feeling.

That is not what SFC means.

In SFC, confidence is constrained by a support structure.
The relevant questions are not:

* “Do I feel good about this?”
* “Does this sound plausible?”

but rather:

* Which parts of the target have already been executed in similar form?
* Which subgraphs, modules, or operators can be reused?
* Which parts are only locally novel?
* Which parts require genuine invention?
* How many bridge steps are missing?
* How recoverable are likely failures?
* How asymmetric is the risk?

SFC is therefore not a psychological confidence score.
It is closer to a **structured feasibility judgment**.

---

# 4. The Two Main Forms of SFC

The most important distinction in the SFC framework is between **confirmed feasibility confidence** and **extension feasibility confidence**.

---

# 5. Confirmed Feasibility Confidence

## **Confirmed Feasibility Confidence**

**Definition.**
Confirmed Feasibility Confidence is the portion of SFC supported by direct execution history of the same task or of a highly similar task family.

This is the strongest and most stable form of feasibility confidence because the target is backed by actual traversal rather than by extrapolation alone.

Typical evidence includes:

* repeated successful execution,
* known input-output behavior,
* known cost and time distribution,
* known failure modes,
* known quality bounds,
* known recovery procedures.

Examples:

* A craftsman repeatedly building a standard cabinet design.
* A software team repeatedly shipping the same service pattern.
* A robotic action routine that has already been executed many times under similar conditions.
* An Action Calling Graph that has already been validated in runtime.

Confirmed confidence is the regime in which a tunnel has already been walked, tested, and stabilized.

---

# 6. Extension Feasibility Confidence

## **Extension Feasibility Confidence**

**Definition.**
Extension Feasibility Confidence is the portion of SFC supported not by exact prior completion of the target, but by the structural neighborhood around the target: validated subtasks, reusable modules, nearby trajectories, partial demonstrations, mechanism-level understanding, and bridgeable local gaps.

This is the confidence that allows an intelligent system to say:

* “I have not done this exact task before, but it lies within reach.”
* “This requires adaptation, not reinvention.”
* “The target is new, but it is supported.”

Examples:

* A craftsman taking a custom commission that differs in dimensions, material, or ornamentation from prior work.
* An engineer estimating a new system variant built from familiar components and familiar architectural constraints.
* A research team committing to a new experiment because the core mechanisms and surrounding methods are already in place.
* A Task Calling Graph being proposed before every underlying Action Calling Graph has been fully executed.

Extension confidence is where intelligence moves beyond repetition while still remaining disciplined.

---

# 7. Why the Distinction Matters

The distinction between confirmed and extension confidence prevents two opposite mistakes.

## Mistake 1 — Treating everything without exact precedent as unsupported

This collapses all novelty into one bucket.
It cannot distinguish between:

* a task that is one small variation away from a well-practiced tunnel, and
* a task that lies outside the system’s competence entirely.

That makes the framework too conservative and too blind to real skill transfer.

## Mistake 2 — Treating all adjacency as equivalent

This is the opposite error.
It assumes that if a target “feels related,” confidence should be high.

But adjacency is not enough.
Some variations are trivial; others destroy the assumptions that made the original tunnel work.

SFC needs to be able to say:

* this extension is safe,
* that extension is expensive but feasible,
* and another extension is currently speculative.

The confirmed/extension split is the first step toward that discrimination.

---

# 8. Structural Support: What Actually Contributes to SFC?

SFC can be understood as a function of multiple kinds of support.
The list below is not necessarily exhaustive, but it captures the main families.

## 8.1 Direct Precedent

The strongest support comes from direct completion of the same or nearly identical tasks.

## 8.2 Subtask Coverage

Even if the whole target is new, many of its subtasks may already be solved.

## 8.3 Module Reuse

A new target may be largely assembled from known components, tools, routines, or operator clusters.

## 8.4 Adjacent Trajectories

A system may have traversed nearby paths in the same function family and therefore know how to approach the new target.

## 8.5 Mechanism-Level Understanding

The system may understand the underlying constraints, causal structure, and failure modes even if it has not executed the exact target.

## 8.6 Recovery and Bridgeability

Confidence is higher when missing pieces are bridgeable and failure is recoverable.

These ingredients do not contribute equally in every domain, but together they define the idea of **structural support**.

---

# 9. SFC Is About Commitment, Not Just Classification

A useful way to understand SFC is to ask what it is *for*.

SFC is not only about saying “likely feasible” or “unlikely feasible.”
Its deeper role is to support **commitment decisions**.

An intelligent system with SFC should be able to decide not only whether a target is possible, but also:

* whether to accept the task at all,
* whether to quote a full commitment or a staged commitment,
* whether to prototype first,
* whether to add a risk buffer,
* whether to call for extra tools, collaborators, or brain units,
* and when to refuse.

In this sense, SFC sits between **capability** and **action policy**.

It is the layer that asks:

> “Given the current support structure, what kind of commitment is justified?”

---

# 10. SFC and Function Tunnels

The SFC framework is closely related to the idea of function tunnels.

A function tunnel can be thought of as a family of structurally coherent trajectories, routines, or transformations that preserve a workable path toward a target class.

When a target lies inside a well-practiced tunnel, confirmed confidence is high.
When it lies near the tunnel boundary but remains bridgeable, extension confidence may still be high enough for a disciplined commitment.
When it lies beyond the supported neighborhood, confidence should fall.

This is why later documents in this repository will discuss:

* **Function Tunnel Confidence Thickness**
* **extension zones**
* **confidence decay**
* and **commitment boundaries**

But SFC itself is broader than any single tunnel formalism.
It is meant to capture the general feasibility judgment layer that can be instantiated in tunnel-based systems, task graph systems, human skill systems, and future AI runtimes.

---

# 11. SFC and Task Calling Graphs

Task Calling Graphs provide one of the clearest motivations for SFC.

An Action Calling Graph records actual action-level structure that has already been executed or implemented.
A Task Calling Graph, however, often needs to represent a target organization of work **before** all action-level details are fully realized.

This creates a fundamental asymmetry:

* Action graphs often inherit confidence from execution.
* Task graphs often need confidence **before** execution.

SFC provides a vocabulary for that asymmetry.
It allows us to say that a Task Calling Graph may be supported by:

* confirmed action subgraphs,
* reusable task modules,
* neighboring project precedents,
* known bridge steps,
* and patchwork feasibility proof.

In other words, a Task Calling Graph can function as a **feasibility scaffold**, not merely as a record of past action.

---

# 12. SFC Is Directional, Not Uniform

One of the most important implications of the framework is that feasibility confidence is usually **anisotropic**.

A craftsman may be able to extend very far along:

* material variation,
* dimension variation,
* and standard structural rearrangement,

while having much lower confidence along:

* embedded electronics,
* exotic joinery,
* or unfamiliar finishing requirements.

Similarly, an AI coding system may have strong extension confidence in:

* API design,
* CRUD services,
* data transformation pipelines,

but weak extension confidence in:

* distributed consensus protocols,
* compiler internals,
* or GPU kernel optimization.

SFC should therefore not be imagined as a single undifferentiated number.
It is better understood as a **profile over a structured task space**.

---

# 13. SFC as a Middle Layer in Intelligence

SFC occupies a useful middle position in the architecture of practical intelligence.

It is not the same as:

* low-level execution,
* world modeling,
* symbolic proof,
* or long-term value optimization.

Instead, it is the layer that mediates between what is already known and what may be committed next.

In that sense, SFC can be seen as part of a broader **extension intelligence**:

* the intelligence of moving from validated structure to adjacent novelty,
* without collapsing into either rigid conservatism or unsupported speculation.

---

# 14. A Compact Working Formula

A simple informal way to think about SFC is:

[
\text{SFC(target)} \approx
\text{support from confirmed precedent}

* \text{support from validated parts}
* \text{support from neighboring trajectories}
* \text{support from mechanism understanding}

- \text{penalty from unsupported gaps and risk}
  ]

This is not yet a formal metric.
It is only a conceptual decomposition.
But it captures the spirit of the framework:

SFC is a **balance between structural support and unsupported burden**.

---

# 15. Conclusion

Structural Feasibility Confidence is the central concept of this repository because it captures a basic but under-articulated fact about real intelligence:

> intelligent systems must often commit under partial novelty.

They must judge not only what has already been done, but also what is **close enough to the done** that a disciplined extension is justified.

SFC names that judgment layer.

It distinguishes:

* **confirmed feasibility confidence**, grounded in direct precedent, from
* **extension feasibility confidence**, grounded in structural support around a novel target.

That distinction allows us to study feasibility not as a binary yes/no property, but as a structured and graded relationship between a target and the support that surrounds it.

The next step is to explain one of the most important mechanisms behind extension confidence:

# **Patchwork Feasibility Proof**

---

# Key Takeaways

* **SFC** is confidence that a target is feasible, derived from **structural support**, not only exact precedent.
* SFC has two main forms:

  * **Confirmed Feasibility Confidence**
  * **Extension Feasibility Confidence**
* Structural support may come from:

  * direct precedent,
  * validated subtasks,
  * reusable modules,
  * neighboring trajectories,
  * mechanism understanding,
  * and recoverable bridge strategies.
* SFC is not just about “possible or impossible”; it is about **what kind of commitment is justified**.
* SFC is especially important for **Task Calling Graphs, engineering estimation, craftsmanship, and future AI runtime planning**.
