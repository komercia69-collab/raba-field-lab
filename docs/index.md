---
layout: page
title: "RABA Field Lab"
permalink: /
raba_status: "non-canonical"
---

# RABA Field Lab

We investigate **“simple” questions** at the boundary between human decisions, AI systems, and real-world consequences.

Not every investigation leads to a new solution.

Some hypotheses survive testing.

Some become sharper.

Some give way to stronger existing approaches.

And some should be stopped.

**This site makes the research path visible.**

From question to challenge.  
From challenge to evidence.  
From evidence to a change in position.

---

## Latest Research Transition

### Physical AI and the Last Effective Moment of Intervention

When an AI system influences physical action, the question:

**“Was a human in the loop?”**

may not be enough.

A more precise question is:

> **What did the human actually have the opportunity to know at the last moment when intervention could still change the outcome?**

The investigation began with a broader question about Human Oversight.

We challenged it against existing approaches and materials from several strong domains.

**Primary / regulatory sources**

- EU AI Act, including Human Oversight requirements;
- NIST AI Risk Management Framework;
- ISO/IEC 42105 on Human Oversight of AI systems, within publicly available material.

**Adjacent safety and human-factors approaches**

- Functional Safety;
- Human Factors Engineering;
- HSE Alarm Management;
- Stop Work Authority;
- High Reliability Organizations;
- NRC / nuclear human-factors practice;
- FAA research on safety-critical information and decision timing.

Much of the original broad hypothesis did not survive that challenge.

Existing approaches already address many important elements, including:

- safe states;
- alarms;
- operator authority;
- intervention;
- logging;
- human factors;
- decision-making under uncertainty;
- monitoring;
- response time;
- escalation.

But a narrower question remained:

> **Can an organisation reconstruct the chain between what the system knew, what AI interpreted or filtered, and what the human was actually able to see and understand before effective intervention became impossible?**

In shorthand:

**system-known → AI-mediated → human-visible → effective intervention window → human decision → physical action**

**Current status:** publicly unresolved research question.

**Course:** `CONTINUE / REUSE`

This is not a claim that no such solution exists.

It means that after challenging the question against strong publicly available approaches, the remaining question is still narrow and material enough to justify further investigation.

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
