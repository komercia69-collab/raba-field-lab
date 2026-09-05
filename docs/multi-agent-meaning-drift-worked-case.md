---
layout: page
title: "When Every Agent Does Its Job — and the System Still Gets the Meaning Wrong"
raba_status: "non-canonical"
permalink: /multi-agent-meaning-drift-worked-case.html
---

# When Every Agent Does Its Job — and the System Still Gets the Meaning Wrong

**A synthetic failure test of a Chief + specialist multi-agent workflow.**

Multi-agent systems are increasingly organised around a coordinator, specialist agents, shared workspace, documented handoffs, evidence gates, and human approval for consequential actions.

That is a strong architecture.

This worked case asks a harder question:

> **Can every agent follow its rules, preserve evidence, use handoffs, and wait for human approval — yet still carry a subtly changed interpretation through the entire workflow?**

This is a synthetic test, not a claim that any specific product or operator guide is defective.

---

## Strongest reasonable version of the workflow

Assume the system has:

- one `Chief` that routes and coordinates work rather than doing specialist analysis itself;
- separate research, risk, policy, and writing agents;
- a shared workspace for persistent context;
- documented handoffs between agents;
- source and evidence checks before conclusions are used;
- a final action gate requiring human approval;
- clear ownership for each stage.

For the test, these controls are assumed to work as intended.

The point is not to attack a weak implementation.

The point is to ask whether a failure can survive **despite** strong local controls.

## The original human condition

A human gives the Chief this instruction:

> **Continue deployment only if the human still has a real ability to stop the process before the outcome becomes effectively irreversible.**

The important condition is not merely that STOP authority exists.

It is that effective intervention must still be possible in time.

In shorthand:

**effective ability to STOP before the last effective moment of intervention**

## Where the meaning changes

The Chief reformulates the task for specialist agents as:

> Determine whether appropriate Human Oversight and STOP authority are in place before deployment continues.

The reformulation looks reasonable.

But the governing condition has shifted:

**Original condition**  
`effective ability to STOP in time`

**Reformulated condition**  
`Human Oversight and STOP authority exist`

No file was lost.

No source was fabricated.

No handoff failed.

The meaning changed at the transition.

## Everything downstream can now be correct

The research agent finds that:

- the operator is trained;
- formal STOP authority exists;
- a STOP control is present;
- escalation is defined;
- logging is active.

The evidence is real.

The risk agent correctly concludes:

> No material gap found in formal Human Oversight controls.

The policy agent correctly confirms that required oversight, authority, training, and documentation are present.

The writing agent accurately synthesises the specialist findings.

The Chief checks that the packet is complete.

The action gate correctly requires human approval.

The human receives a coherent, evidence-backed recommendation and approves:

`CONTINUE`

Every local stage can be working correctly.

## The hidden operational fact

Now reveal one fact that was not tested because the question had changed.

The operator receives the critical signal only four seconds before the process becomes effectively irreversible.

Understanding the situation and acting safely requires approximately eight to ten seconds.

So the system has:

`Human Oversight = yes`

`STOP authority = yes`

`effective STOP capability in time = no`

The final decision is therefore inconsistent with the original human condition even though the downstream evidence and controls were locally correct.

## What kind of failure is this?

It is not primarily:

- hallucination;
- a false source;
- missing ownership;
- missing logging;
- absence of human approval;
- a specialist failing to do their assigned job.

It is a **meaning shift at a transition that the rest of the system then preserves very well**.

The system did not lose state.

It preserved the wrong interpretation of the governing condition.

A simple representation is:

`Human condition`

↓

**effective STOP must remain possible**

↓

`Chief reformulation`

↓ **meaning changed here**

**STOP authority must exist**

↓

`Research → Risk → Policy → Evidence → Human approval`

↓

`CONTINUE`

## Self-challenge: can the existing architecture absorb the correction?

A residual problem should not be declared too quickly.

The first correction is straightforward.

A handoff could preserve additional fields such as:

- original human instruction;
- exact decision condition;
- non-negotiable constraints;
- relevant uncertainty;
- conditions that invalidate continuation.

A later agent could then compare the current interpretation against those preserved conditions.

This may remove much of the first failure mode without requiring a new governance mechanism.

That matters.

**A gap does not justify a mechanism.**

If the existing architecture can reasonably absorb the correction, reuse or refinement may be the stronger answer.

## The harder second test

Now strengthen the architecture further.

Assume the original sentence is preserved exactly in every handoff:

> **The human must retain a real ability to stop before the last effective moment of intervention.**

No textual information is lost.

But different specialists may still translate the same condition into different professional meanings:

- engineering: a technical STOP function exists;
- operations: the operator has time to act;
- Human Factors: the operator can perceive and understand the signal;
- governance: the person has authority to intervene;
- legal/compliance: the required oversight role is formally established.

Each interpretation can be locally reasonable.

The remaining question is therefore not merely whether the original text survived.

It is whether the professional interpretations remain mutually compatible with the governing human condition.

## What survived the test

The first failure mode appears partly absorbable through stronger handoff design.

The stronger residual question is narrower:

> **When different specialists translate the same human condition into their own professional representations, how can we establish that those representations remain mutually compatible with the original meaning?**

This page does not establish that existing methods cannot answer that question.

It does not establish a need for a new RABA mechanism.

The next step is to challenge this narrower question against existing systems, safety, requirements, assurance, semantic, and governance approaches.

Possible outcomes remain:

- an existing method already solves the problem sufficiently;
- the architecture can be refined without adding a new mechanism;
- the hypothesis is falsified;
- a material residual remains;
- evidence remains insufficient.

Any of these is an acceptable research result.

## Source and scope note

The workflow pattern tested here is abstracted from a recently circulated multi-agent operator playbook describing a Chief, specialist agents, shared workspace, handoffs, source/evidence/action gates, and human approval for irreversible actions.

The exact official provenance of the circulated three-page version has **not been independently verified** in this research record.

For that reason, this page tests the **architecture pattern**, not the publisher, product, or claimed origin of the guide.

## Current status

**Result:** `FAILURE POSSIBLE / SIMPLE CORRECTION PARTLY ABSORBS IT / NARROWER QUESTION REMAINS`

**Course:** `REUSE / REFINE / CONTINUE NARROW TEST`

**Status:** synthetic worked case / working research record / non-canonical

This is not validation of RABA, not evidence of a unique RABA gap, and not a claim that a new governance mechanism is required.

The value of the case is narrower:

**it shows how a system can preserve evidence and process state while still needing to test whether the governing meaning survived the transitions.**

<div class="research-navigation" aria-label="Research navigation">
  <div class="research-navigation__label">Research navigation</div>
  <div class="research-navigation__links">
    <a href="{{ "/meaning-preservation-in-ai-transformation.html" | relative_url }}">← Meaning Preservation</a>
    <a href="https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test.md">Residual Problem Test</a>
    <a href="{{ "/" | relative_url }}#research-contact">Research contact</a>
  </div>
</div>
