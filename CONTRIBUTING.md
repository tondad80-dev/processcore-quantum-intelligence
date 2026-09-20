# Contributing to ProcessCore

Thank you for your interest in ProcessCore.

ProcessCore is an experimental systems-engineering project focused on deterministic evidence, provenance, authority and auditability around probabilistic AI interpretation.

Contributions are welcome when they preserve those boundaries and keep public claims narrower than the evidence.

## Core contribution principles

Please keep these distinctions explicit:

- evidence is not interpretation;
- validation is not authority;
- observed state is not expected state;
- policy decision is not authorization;
- authorization is not effect;
- persistence is not activation;
- an execution path is not execution authority.

A contribution should not collapse these boundaries for convenience.

## Scope

Good contributions are typically:

- small and reviewable;
- deterministic where practical;
- explicit about assumptions and inputs;
- reproducible from documented steps;
- fail-closed when authority is unresolved;
- careful not to rewrite historical evidence;
- compatible with the current public claim boundaries.

Large architectural changes should be split into smaller independently reviewable steps where possible.

## Evidence and claims

When proposing a change, distinguish clearly between:

1. what was observed;
2. what was validated;
3. what remains unresolved;
4. what authority, if any, permits execution or mutation;
5. what effect actually occurred.

Do not present a passing validator result as proof of authority.

Do not rewrite a historical FAIL or UNKNOWN result into PASS. A corrected follow-up test should be recorded as a new result.

## Runtime and effect boundaries

A code path, service definition, wrapper, deployment artifact or persistent integration point may exist without being active or authorized to execute.

Contributions must not imply that:

- persistence means activation;
- activation means authority;
- authority means an effect occurred;
- a successful test means production readiness;
- a research result means autonomous remediation is enabled.

Any state-changing action should remain separately authorized and independently auditable.

## Project boundaries

ProcessCore, QCore and AgriCore are separate project authorities.

Evidence or implementation progress in one project does not automatically establish authority in another.

Cross-project integration should make provenance and authority transfer explicit rather than implicit.

## Pull requests

A useful pull request should include:

- a concise description of the change;
- the problem or uncertainty it addresses;
- the evidence used to justify the change;
- how the change was tested;
- any remaining limitations or unresolved points;
- confirmation that no broader runtime, production or authority claim is being made unless separately established.

Prefer one logical change per pull request.

## Public documentation

Documentation and website changes should reflect the verified project state, not anticipated capability.

Avoid language such as:

- production-ready;
- autonomous remediation;
- fully deployed;
- active control plane;
- guaranteed correctness;
- hallucination-free;

unless those claims are independently established by evidence appropriate to that claim.

## Security and sensitive implementation details

Do not publish credentials, secrets, private infrastructure identifiers, private network details or sensitive runtime internals.

Public documentation should explain architectural boundaries without requiring disclosure of private operational details.

## License

By contributing to this repository, you agree that your contributions will be licensed under the Apache License, Version 2.0, consistent with the repository's [LICENSE](LICENSE) file.
