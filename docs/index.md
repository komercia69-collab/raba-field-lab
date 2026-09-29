---
layout: page
title: "RABA Field Lab"
permalink: /
raba_status: "non-canonical"
---

# RABA Field Lab

## What I show here

I use structured analysis to examine difficult questions at the boundary between business processes, AI systems, human decisions, and real-world consequences.

The work shown here demonstrates four things:

- **Structured problem analysis** — separating the actual problem from assumptions and attractive explanations.
- **Comparison against existing solutions** — checking standards, security controls, governance approaches, and adjacent methods before proposing something new.
- **Evidence-based decisions** — documenting why a direction should continue, change, be reused, or stop.
- **Negative results** — treating “do not build a new mechanism” as a valid outcome when existing approaches already solve the problem well enough.

This is a research portfolio, not a claim that every question requires a new framework.

---

## Three examples of how I work

### 1. External instructions → AI agent action

**What I tested:**  
Whether risks arising when an AI agent receives external instructions require a new governance mechanism.

**What I found:**  
Existing controls — provenance, trust boundaries, authorization, policy enforcement, sandboxing, restricted capabilities, audit trails, and human approval — already cover the tested problem to a substantial degree.

**Decision:**  
**REUSE / STOP — no new RABA-specific mechanism justified in the tested scenario.**

[Read the worked example](https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test-llms-txt-worked-example.md)

---

### 2. Meaning preservation across AI transformation

**What I tested:**  
Whether information can remain technically traceable while losing meaning that later matters for a human decision.

**What I found:**  
The relevant question is not only whether data is preserved, but whether decision-relevant meaning survives transformation and handoff.

**Decision:**  
**CONTINUE — bounded unresolved research question.**

[Read the research note]({{ "/meaning-preservation-in-ai-transformation.html" | relative_url }})

---

### 3. Multi-agent meaning drift

**What I tested:**  
Whether several agents can each follow their local rules while a changed interpretation propagates through the full workflow.

**What I found:**  
Local compliance and preserved handoffs do not automatically prove that the original meaning remained intact end-to-end.

**Decision:**  
**RESEARCH CASE — synthetic worked example, not a live-system validation.**

[Read the worked case]({{ "/multi-agent-meaning-drift-worked-case.html" | relative_url }})

---

## How I approach a problem

`Question → Existing solutions → Strongest counterexample → Evidence → Residual problem → Decision`

Possible decisions include:

`CONTINUE / MODIFY / REUSE / REASSESS / STOP`

A useful analysis may end with:

**“The existing solution is already strong enough. Do not build another mechanism.”**

That is a successful result when the evidence supports it.

---

## Evidence boundary

Some material on this site is based on public research, standards, and worked examples rather than deployment inside a live production system.

Where evidence has not been independently reproduced or a case is synthetic, it is labelled explicitly.

I treat that limitation as part of the analysis, not something to hide.

---

## Explore deeper

The sections below preserve the fuller research trail, current unresolved work, methods, evidence boundaries, and governance context behind the portfolio examples.

A reader can stop at the portfolio summary above or continue into the research layer below.

---

## Latest Research Transition

### From Preserving Meaning to Preserving Governing Relationships

Recent work has narrowed the question beyond whether information or provenance survives an AI-supported transformation.

A process may preserve the original artifacts, evidence, and even the original wording while still changing what a governing condition means in practice.

The current research question is:

> **When evidence, observations, interpretations, and decisions move through an AI-supported process, what must remain invariant so that a downstream representation does not acquire meaning or authority that the original condition never gave it?**

A useful shorthand is:

**Reality → Observation → Evidence → Interpretation → Decision → Action**

The question is not only whether each element is present or locally correct.

It is also:

> **What is allowed to change at each transition — and what must not?**

Several distinctions are being pressure-tested:

- evidence is not the same as the claim it supports;
- observation is not the same as a determination of materiality;
- materiality is not the same as authority;
- technical capability is not the same as business or normative authority;
- authority to suspend is not authority to redefine the underlying decision;
- an unknown or unverified state is not automatically equivalent to “no change” or “safe to proceed.”

This extends an earlier Physical AI / Human Oversight investigation.

That investigation asked what a human was actually able to know before the last effective moment of intervention, and whether the chain could be reconstructed:

**system-known → AI-mediated → human-visible → effective intervention window → human decision → physical action**

The newer question is broader but still bounded: even where the chain is reconstructable, can the **type, direction, and consequence of the relationships between its states** be inspected well enough to detect a silent change in governing meaning?

This is currently a research question, not a finished RABA mechanism.

It does not establish that existing requirements, assurance, safety, provenance, or governance methods are insufficient.

**Current status:** publicly unresolved research question.

**Course:** `CONTINUE / REUSE / PRESSURE-TEST`

### [Meaning Preservation in AI Transformation]({{ "/meaning-preservation-in-ai-transformation.html" | relative_url }})

The research note now extends from preserving information and intent to a narrower transition question: whether governing relationships themselves remain intact as observations, evidence, interpretations, and decisions move through a process.

### [Worked Case — Multi-Agent Meaning Drift]({{ "/multi-agent-meaning-drift-worked-case.html" | relative_url }})

The synthetic worked case shows why preserving the original text is not always sufficient: different locally valid representations can remain individually defensible while no longer preserving the same governing condition.
---

## An Investigation We Stopped

### External Instructions and AI Agent Action

We tested whether risks arising when an AI agent receives instructions from an external source, such as `llms.txt`, require a new RABA-specific mechanism.

Before treating this as a new governance gap, we compared the problem against existing classes of controls, including:

- provenance and instruction-source control;
- trust boundaries;
- separation of trusted and untrusted sources;
- authorization before action;
- policy enforcement;
- sandboxing;
- capability restriction;
- logging and audit trails;
- observability;
- human approval and escalation for sensitive actions;
- organisational controls around agent deployment.

We then applied the **Residual Problem Test**.

Instead of asking:

> “Is there a new problem here?”

we asked a harder question:

> **If the strongest reasonable combination of existing technical and organisational controls is used, does a material governance problem still remain that actually requires a new mechanism?**

Within the tested scenario, we did not establish such a residual.

**Research status:** `NO MATERIAL RESIDUAL FOUND`

**Course:** `REUSE / STOP`

This does not mean the risk does not exist.

It means we did not find sufficient grounds to create a new RABA-specific mechanism for a problem class already covered by existing approaches.

**Sources and full analysis →**  
[Public Residual Problem Test worked example](https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test-llms-txt-worked-example.md)

---

## When a Negative Result Is the Best Result

Research does not have to produce a new framework, mechanism, or proprietary concept.

Sometimes the best result is to establish that a problem is already addressed well enough by existing approaches.

That can help us:

- avoid building a duplicate mechanism;
- avoid presenting an existing solution as a new development;
- avoid continuing a direction simply because time has already been invested in it;
- focus research on genuinely unresolved boundaries;
- preserve resources for questions where a material residual really remains.

So a result such as:

**`NO MATERIAL RESIDUAL FOUND / REUSE / STOP`**

does not mean the research failed.

It means the hypothesis was tested and **did not provide sufficient grounds for new development**.

**Sometimes the best new mechanism is the one research shows we do not need to build.**

---

## Research Trail

This site makes it possible to follow how research questions change over time.

Not only what conclusions were reached, but also:

- what we initially suspected;
- which existing approaches we found;
- what we tested;
- what did not survive the challenge;
- what remained;
- why an investigation continued, changed direction, or stopped.

This is not just a list of publications.

It is:

**a chronology of how the research position changes under pressure from evidence.**

---

## How to Read the Research

Each investigation is organised around a small set of questions.

### Question

What are we actually trying to understand?

### What we checked

Which existing approaches, standards, research, and adjacent solutions were examined?

### What failed

Which part of the original hypothesis did not survive comparison?

### What survived

What remained after the strongest reasonable challenge?

### Result

`CONTINUE / MODIFY / REUSE / REASSESS / STOP`

### Sources

Which public materials and evidence support the result?

A reader can stop at the short summary.

Or go deeper into the full worked example, sources, and research trail.

---

## Methods & Evidence

One method used in this work is the **Residual Problem Test**.

Its purpose is to avoid moving too quickly from an observed problem to the development of a new RABA mechanism.

The central question is:

> **If an external or existing solution works in its strongest reasonable form, together with available technical and organisational controls, what material governance problem still remains?**

Possible outcomes include:

- RABA adds nothing;
- an external approach is stronger;
- an existing solution has already been found;
- the hypothesis is falsified;
- no material residual remains;
- evidence is insufficient;
- a residual remains and deserves another test.

The absence of a new mechanism is a valid and useful outcome.

[Read the Residual Problem Test](https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test.md)

[Research area](https://github.com/komercia69-collab/raba-field-lab/tree/main/research)

[Case area](https://github.com/komercia69-collab/raba-field-lab/tree/main/cases)

[Research templates](https://github.com/komercia69-collab/raba-field-lab/tree/main/templates)

<div class="research-navigation" aria-label="Research navigation">
  <div class="research-navigation__label">Research navigation</div>
  <div class="research-navigation__links">
    <a href="https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test.md">← Method</a>
    <a href="https://github.com/komercia69-collab/raba-field-lab/blob/main/docs/index.md">Open source</a>
    <a href="https://raw.githubusercontent.com/komercia69-collab/raba-field-lab/main/docs/index.md">Raw / download</a>
    <a href="https://github.com/komercia69-collab/raba-field-lab/blob/main/research/residual-problem-test-llms-txt-worked-example.md">Worked example →</a>
  </div>
</div>

---

## Field Lab Boundary

RABA Field Lab is a public research environment.

Material here may challenge existing RABA hypotheses.

It does not automatically change RABA.

Publication here does not mean:

- canon;
- validation;
- adoption;
- endorsement;
- partnership;
- certification;
- compliance;
- commercial readiness;
- automatic architectural change.

**Field Lab can challenge RABA.  
Field Lab cannot modify RABA.**

External evidence may challenge an assumption.

It does not itself authorize a replacement architecture.

[Read the Field Lab governance boundary](https://github.com/komercia69-collab/raba-field-lab/blob/main/GOVERNANCE.md)

---

## Human Owner Authority

AI may assist with:

- research;
- comparison;
- evidence mapping;
- structuring;
- drafting;
- review;
- language and editing support.

Final decisions about:

- research direction;
- publication;
- architectural change;
- status promotion;
- canonicalization

remain with the Human Owner.

---

## Research contact

Relevant prior work, challenge cases, and bounded research questions are welcome.

[LinkedIn](https://www.linkedin.com/in/oleksandr-shuliak-49039285/) · [Email](https://mail.google.com/mail/?view=cm&fs=1&to=raba.fieldlab@gmail.com)

`raba.fieldlab@gmail.com`

No employment, partnership, validation, or adoption is implied by contact or exchange.

---

## Transparency Note

This public research interface reflects research directed and reviewed by the Human Owner.

ChatGPT is used as a research, comparison, structuring, language, and editing assistant.

AI-assisted analysis does not constitute independent authority, approval, validation, or canonicalization.

Final responsibility for public content remains with the Human Owner.
