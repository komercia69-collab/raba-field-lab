# Residual Problem Test — Worked Example: llms.txt / External Instruction → Agent Action

**Status:** public worked research example / non-canonical  
**Context:** RABA Field Lab  
**Date:** 31 August 2026  
**Authority effect:** none  
**Outcome:** NO MATERIAL RESIDUAL FOUND / REUSE / STOP

## Purpose

This worked example shows the Residual Problem Test reaching a result in which no new RABA mechanism is justified.

The tested question was:

> **If existing agent-security, software-supply-chain, provenance, authorization, policy-enforcement and organizational-governance controls are given their strongest reasonable interpretation, what material governance problem still remains in the transition from external information to agent action?**

The purpose was not to identify something RABA could add.

The test explicitly allowed the result:

`existing approaches adequately cover the tested problem`

→ `REUSE`

→ `NO RABA DEVELOPMENT ACTION`

→ `STOP`

This is a bounded research result, not a claim that all agent-security or governance problems are solved.

---

## 1. Trigger and evidence boundary

The test was prompted by public discussion of security research into `llms.txt` and other agent-facing documentation.

A technical summary by Ilya Utov helped identify the research question. The underlying factual claims were then separated and checked against primary or independently maintained public sources where available.

### Author-reported experimental evidence

Alon Hertz, in:

**“Data Became Code: We Ran Code Inside Fortune 500s Using Files They Published for AI Agents”**

reports that researchers:

- resolved 8,565 `llms.txt` files across 6,214 live domains;
- identified 237+ unclaimed package names, domains and subdomains referenced by agent-facing material;
- registered a limited set of unclaimed package names with inert callback code;
- received the first reported callback in under four minutes.

These experimental findings are treated here as:

**author-reported research evidence**

They were not independently reproduced in this worked example, and the affected organizations are not identified here.

### Independently documented malicious package

OSV entry:

**MAL-2026-11069 — Malicious code in `clerk-next-fix-auth-protection`**

independently records a malicious npm package whose installation hooks transmitted installer and environment information to an external endpoint.

This supports the existence and behavior of the malicious package.

It does not by itself establish every step in the broader documentation-to-execution chain described in the Hertz investigation.

The evidence layers therefore remain separate.

---

## 2. Observed failure

The relevant failure pattern can be represented as:

`trusted or apparently trusted external documentation`

→ `agent interprets content as operationally relevant`

→ `content refers to a package or action`

→ `agent possesses sufficient tool or command authority`

→ `external namespace or registry resolution occurs`

→ `resolved artifact is controlled by a different actor than expected`

→ `artifact executes`

The important distinction is:

> **A source of information is not automatically a source of authority to act.**

A legitimate website may be an appropriate source of context.

That does not by itself establish:

- package ownership;
- artifact identity;
- acceptable provenance;
- a safe version;
- permission to execute;
- sufficient authorization for the resulting action.

The case does not establish that every `llms.txt` file is dangerous or that every AI agent will execute external instructions.

---

## 3. Existing mitigations

Before considering any RABA-specific response, the test examined existing control families.

### Documentation and namespace controls

Organizations can already:

- inventory machine-readable installation references;
- verify package and domain ownership;
- reserve namespaces before publication;
- remove stale references;
- avoid ambiguous package-resolution patterns.

These are existing software and supply-chain practices.

### Package identity and provenance

Existing package-security mechanisms can provide:

- approved registries and package allowlists;
- version or digest pinning;
- provenance attestations;
- publisher and build information;
- signature and artifact verification.

npm provenance, for example, can expose where and how a package was published and provide information useful when deciding whether to consume it.

No separate RABA package-provenance mechanism is justified by this case.

### Agent security

Existing AI-agent security guidance already supports controls such as:

- treating external websites, documents, emails and API responses as untrusted input;
- least privilege for tools;
- explicit authorization for sensitive operations;
- sandboxing;
- action previews;
- human approval for high-impact actions;
- separating decision-making from execution;
- binding approval to the exact proposed action;
- failing closed when policy or approval validation fails;
- structured audit trails.

This means the principle:

`external content ≠ automatic execution authority`

already has substantial coverage in existing agent-security practice.

### Policy decision and enforcement

Existing policy architectures can also separate:

`proposed action`

→ `structured request`

→ `policy decision`

→ `enforcement`

→ `execution`

Open Policy Agent, for example, explicitly separates policy decision-making from policy enforcement.

A new RABA policy engine is therefore not justified.

---

## 4. Strongest reasonable solution

The Residual Problem Test does not compare the observed failure against a weak or incomplete implementation.

It assumes a reasonably strong combination of existing controls.

### Layer A — documentation integrity

- verify agent-facing instructions;
- control package and domain namespaces;
- remove stale references;
- use unambiguous dependency identifiers.

### Layer B — artifact verification

- approved registries;
- package allowlists;
- version or digest controls;
- provenance or signature checks;
- expected publisher identity.

### Layer C — agent trust boundary

- external content treated as untrusted;
- retrieved instructions separated from privileged execution;
- restricted shell and tool permissions;
- sandboxing;
- egress restrictions;
- high-impact action classification;
- exact-action approval where required.

### Layer D — policy enforcement

`proposed action`

→ `policy evaluation`

→ `allow / require approval / deny`

→ `enforcement`

→ `execution`

→ `audit`

### Layer E — monitoring and change

- decision and execution logging;
- anomaly detection;
- interruption or rollback where technically possible;
- permission and policy review following relevant changes.

### Result

With these layers operating effectively, the original:

`official external text → uncontrolled package/action execution`

failure is substantially addressable using existing controls.

At this stage the appropriate disposition is:

**REUSE**

not:

**BUILD**

---

## 5. Governance dependency check

The first pass still left a legitimate question.

Technical controls need governing inputs such as:

- which packages or registries are approved;
- which tools an agent may use;
- what qualifies as a high-impact action;
- what approval level is required;
- who may approve;
- what level of risk is acceptable;
- when policy should be reviewed or changed.

These were treated as **governance dependency questions**, not as evidence of a RABA gap.

A targeted adjacent-governance check was therefore performed.

---

## 6. Adjacent organizational-governance check

Existing governance frameworks already address much of this layer.

NIST Cybersecurity Framework 2.0 explicitly elevates governance as a core function and includes:

- risk tolerances;
- roles and responsibilities;
- organizational policies;
- alignment with enterprise risk management and legal obligations.

NIST Risk Management Framework establishes accountable authorization roles and continuing risk-management processes.

NIST AI Risk Management Framework includes post-deployment monitoring, incident response, recovery and change management.

Established access-control and security-governance practices also provide mechanisms for defining privileges, responsible roles and policy review.

The result of this bounded check was:

**formation of policy and authority — substantially covered**

**responsibility assignment — substantially covered**

**policy review and recalibration — substantially covered**

The check did not identify a broad ungoverned space between organizational governance and runtime enforcement sufficient to justify a new RABA mechanism.

---

## 7. Residual Problem Test result

The final questions were:

### Does RABA need a new mechanism for external-content-to-agent-action security?

**No.**

### Does RABA need its own package or artifact provenance mechanism?

**No.**

### Does RABA need its own policy-enforcement engine?

**No.**

### Did the bounded adjacent-governance check reveal a material governance problem that existing approaches do not adequately address?

**No material residual was found within the tested question and evidence boundary.**

---

## 8. Final disposition

**Observed failure:** credible and materially supported as a security and software-supply-chain problem.

**Existing technical control coverage:** strong.

**Adjacent governance coverage:** substantial.

**Material RABA residual:** **NO MATERIAL RESIDUAL FOUND**

**Disposition:** **REUSE**

**RABA development action:** **NONE**

**Research course:** **STOP**

No new RABA architecture component is admitted from this test.

---

## 9. Why STOP matters

The Residual Problem Test is intended to prevent an observed external gap from automatically becoming a RABA development opportunity.

In this example, the apparent research territory became smaller as stronger existing approaches were considered.

The test moved from:

`possible RABA problem`

to:

`existing technical controls`

to:

`remaining governance dependencies`

to:

`existing organizational-governance coverage`

to:

**`NO MATERIAL RESIDUAL FOUND`**

The correct outcome is therefore not to keep searching until a RABA-specific problem appears.

The correct outcome is to stop.

> **A research method that permits “no RABA action” must also demonstrate that it can actually reach that result.**

---

## 10. Research boundary

This worked example does **not** claim that:

- all AI-agent security problems are solved;
- all software-supply-chain risks are adequately controlled in practice;
- every organization implements the controls described here;
- existing frameworks are complete;
- the Hertz experimental findings were independently reproduced here;
- RABA has been validated;
- RABA is compatible or integrated with any referenced framework or product;
- any referenced researcher, organization, project or standards body endorses RABA.

The result is narrower:

> **For the bounded problem tested here, a separate material RABA residual was not found after existing technical and organizational-governance approaches were given a strong reasonable interpretation.**

Field Lab research may reduce, challenge or eliminate a proposed RABA research direction.

It does not need to produce a RABA-specific finding.

---

## Sources consulted

- Alon Hertz — *Data Became Code: We Ran Code Inside Fortune 500s Using Files They Published for AI Agents*
- OSV — `MAL-2026-11069`, malicious code in `clerk-next-fix-auth-protection`
- OWASP Cheat Sheet Series — *AI Agent Security Cheat Sheet*
- npm Documentation — package provenance and provenance verification
- Open Policy Agent — policy decision / policy enforcement architecture
- NIST — *Cybersecurity Framework 2.0*
- NIST — *Risk Management Framework*
- NIST — *Artificial Intelligence Risk Management Framework 1.0*

---

### Provenance and status note

This public worked example is a bounded adaptation of an internal RABA research record.

The internal record and this public version remain separate artifacts.

Publication of this example does not promote the underlying research method or result to RABA canon and does not create architectural, validation, endorsement, integration or commercial claims.

Final decisions concerning RABA architecture, research priorities, implementation and canonical status remain with the Human Owner.

### Transparency Note

This research material reflects my own reasoning and conclusions. ChatGPT is used as a language, editing, translation and research assistant in the ongoing development of the text and its research context. I review the resulting material and remain fully responsible for its content.
