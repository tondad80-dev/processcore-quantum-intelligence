# ProcessCore

**Evidence before interpretation.**

ProcessCore is an independent experimental systems-engineering project exploring how deterministic evidence, provenance, authority and auditability can be established around probabilistic AI interpretation.

> The model may interpret evidence. It does not establish what evidence is authoritative.

## Current public state — 2026-09-20

**ProcessCore observation runtime v0.4 remains the accepted stable public reference baseline.**

The v0.4 observation baseline has demonstrated functional and semantic repeatability across accepted controlled runs. Legitimately volatile runtime state remains explicit volatility rather than being forced into false byte-for-byte identity.

Prototype v0.1 remains complete and frozen as an earlier implementation milestone. It is preserved as project lineage and is not rewritten as the current runtime baseline.

Post-v0.4 work has now crossed an additional implementation boundary: a persistent control-plane execution path has been created on Node00 under create-once control and verified after creation.

That path remains deliberately inert.

Its existence does not mean that it is active, runtime-tested, authorized for execution, scheduled, or permitted to produce effects.

The current public architectural framing remains:

**EVIDENCE → PROVENANCE → AUTHORITY → INTERPRETATION**

with the post-v0.4 control-path invariant:

**ACTUAL_STATE ≠ EXPECTED_STATE ≠ POLICY_DECISION ≠ AUTHORIZATION ≠ EFFECT**

with an additional implementation boundary:

**PERSISTENCE ≠ ACTIVATION ≠ EXECUTION AUTHORITY ≠ EFFECT**

ProcessCore does not make a language model deterministic. It makes the evidence and authority path explicit, bounded, inspectable and auditable.

### What is currently supported

- explicit evidence identity and provenance;
- source and project currentness checks;
- project-scoped context boundaries;
- deterministic evidence comparison;
- fail-closed handling of unresolved authority;
- version-scoped authority across controlled successor transitions;
- append-only audit mechanisms;
- separation of technical authority from downstream human or AI interpretation;
- stable v0.4 observation-runtime behavior with demonstrated functional repeatability;
- bounded post-v0.4 validation of explicit separation between actual state, expected state, policy decision, authorization and effect;
- create-once persistence of a control-plane execution path while keeping activation, execution authority and effect authority separate.

## Post-v0.4 control boundary

Current research extends ProcessCore beyond observation while preserving separate control boundaries.

**Detecting drift is not permission to fix it.**

Observed state is evidence. Expected state comes from valid project-scoped authority. Their difference may support classification or a deterministic policy decision, but a policy decision does **not** itself authorize a state-changing effect.

A further boundary is now explicit in the implementation:

**The existence of an execution path is not execution authority.**

A persistent control-plane path has been created and verified after creation, but remains intentionally inert. Persistence alone does not activate it, authorize runtime execution, create scheduling authority, or permit effects.

A state-changing effect requires separate explicit authorization. If an effect occurs, execution evidence and post-effect observation must remain separately inspectable and auditable; the resulting observation creates new evidence rather than silently rewriting the prior state.

LLM authority remains none.

This post-v0.4 work is bounded research and validation. It is **not** a declared ProcessCore v0.5 release, not a live autonomous-remediation claim, not proof of runtime readiness and not a production-readiness claim. The accepted v0.4 baseline remains preserved.

## Validation is not authority

A validator is a test layer, not an automatic source of truth.

Documented ProcessCore / AgriCore and ProcessCore-Lab cases have preserved validation failures for read-only reconciliation instead of automatically rewriting the underlying state. Reconciliation has shown cases where the authoritative contract remained coherent while the validator expected a different representation.

The architectural lesson is:

- evidence ≠ validation;
- validation ≠ authority;
- authority ≠ interpretation.

Validation logic must itself be auditable: its inputs, assumptions and expected representation need provenance too.

This is an architectural conclusion from documented ProcessCore cases. It is not presented as a quotation or rule from an external standard.

## AgriCore bound-project test context

AgriCore remains a separate runtime and project authority. Its current public-safe state is governed by a ledger-consistency hold, so unreconciled later experimental history is not represented here as current AgriCore truth.

Current public-safe boundaries:

- AgriCore remains a separate runtime and project authority;
- Raspberry Pi / project evidence remains runtime truth where applicable;
- similar evidence does not automatically cross a project boundary;
- ProcessCore evolution does not automatically advance AgriCore;
- the current authorized direction is read-only reconciliation of persistence-readiness and schema/runtime identity boundaries;
- candidate persistence, lifecycle mutation and runtime authorization are not claimed from the controlling reconciled state;
- failures and unresolved states remain unresolved rather than being converted into PASS;
- later unreconciled history stays outside the current public-state claim until reconciled.

AgriCore does **not** currently prove:

- universal portability;
- external interoperability;
- production readiness;
- autonomous remediation;
- hallucination elimination.

## Project boundaries

Responsibilities remain separated:

- **ProcessCore** — evidence, provenance, authority, deterministic processing and audit/control architecture;
- **QCore** — independent production data acquisition, processing and enrichment runtime;
- **AgriCore** — independent experimental domain project.

A result verified in one project does not automatically become authority in another.

## Failure semantics

ProcessCore prefers explicit uncertainty to invented certainty.

Examples:

- changed evidence does not silently inherit the authority of an earlier state;
- semantically similar evidence does not automatically cross a project boundary;
- unresolved authority remains unresolved;
- validation failure is not silently rewritten into success;
- historical audit state is preserved;
- a failed validator may itself become the object of audit when its assumptions conflict with authoritative evidence;
- observed drift does not create a policy decision;
- a policy decision does not itself authorize an effect;
- authorization does not remove the requirement for post-effect evidence.

## What ProcessCore is not

ProcessCore is not:

- an LLM;
- a production web crawler;
- a confidence engine;
- a claim that probabilistic models can be made fully deterministic;
- proof of universal portability or external interoperability;
- a production-ready autonomous system;
- live autonomous remediation;
- proof that a persisted execution path is active, runtime-ready or authorized to execute;
- a declared v0.5 release.

## Research lineage

ProcessCore evolved from an earlier technology-intelligence and ecosystem-discovery architecture.

That earlier state remains preserved as project history, including:

`PC-2026-08-12-V1.html`

Historical quantum-ecosystem, crawler, enrichment and market-intelligence material should be read as research lineage, not as the current ProcessCore runtime definition.

## Public references

Website:  
https://tondad80-dev.github.io/processcore-quantum-intelligence/

LinkedIn:  
https://www.linkedin.com/in/tonda-dospiva-b160281a7/

Repository:  
https://github.com/tondad80-dev/processcore-quantum-intelligence

---

**Antonín Dospiva**  
Systems Architect · AI Evidence · Provenance · Auditability
