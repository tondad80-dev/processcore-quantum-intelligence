# ProcessCore

**Evidence before interpretation.**

ProcessCore is an independent engineering project developing checks for AI-generated Python modules on Raspberry Pi. It pairs explicit specifications with predefined tests and recorded results. Deployment remains a separate human decision.

[Website](https://tondad80-dev.github.io/processcore-quantum-intelligence/) · [Earlier website review](public-status-2026-10-14.md) · [Latest claim check](media/processcore-claim-check-2026-10-14.json)

## Current public status — 28 October 2026

A **scoped ProcessCore 1.0.2 assembly** was accepted on Raspberry Pi / Node00 on **27 October 2026**, following the earlier scoped 1.0.0 acceptance on 14 October. It covers bounded observation, source retrieval, Python-module checking and structured-claim checks. The source-index refresh restored current source retrieval within the existing scope. This is a reconciliation of recorded evidence, not a new test run or general production-readiness claim.

One **two-file lifecycle-report utility** has now completed task-specific qualification, acceptance and source adoption, and was installed on Pi on **25 October**. Its frozen campaign recorded **114 matching captures** (57 vectors in two orders); native Pi checks passed **7/7**. It validates and summarizes a fixed lifecycle JSON report format, without proving the truth of that report. [Acceptance and limits](https://github.com/tondad80-dev/processcore-current/blob/a7576e747aeeb542f0696e4e46a4c728e46d5184/factory/evidence/lifecycle-summary-v1/decision.md) · [Pi installation](https://github.com/tondad80-dev/processcore-current/blob/bf64251a63ba9e5f957bdc55baf459890349abaa/factory/evidence/lifecycle-summary-v1/pi-native-20261025/installation.json).

General repository-task support remains experimental. The first measured-use pilot has **not started**: real use, total human effort, time savings and customer benefit have not yet been demonstrated. The terminal replay and module evidence below keep their **14 October** dates and original limitations.

### Preserved module evidence — 14 October 2026

Observation runtime **v0.4** and Factory module **0.1.3-rc.1** are separately versioned components. The scoped release does not renumber them. All **29 Factory manifest files** matched their declared size and SHA-256 in the **14 October review**; this documentation update did not rerun that check.

Two original Factory **0.1.0** jobs retain historical test and acceptance evidence. A new **CLAIM-SUMMARY-002** job adds an accepted candidate under the current **0.1.3-rc.1** runner:

| Job record | Prescribed tests | Recorded decision | Product adoption |
| --- | --- | --- | --- |
| NORMALIZE | 7 passed | Historical accepted candidate | Not deployed into a product |
| SUMMARY | 8 passed | Historical accepted candidate | Not deployed into a product |
| CLAIM-SUMMARY-002 | 21 passed; 73 candidate calls; return code 0 | Accepted and packaged under the current runner boundary | No product deployment established by this record |

The reviewed result, acceptance and delivery bindings matched their stored hashes. Each successful job recorded one model invocation. The new candidate summarizes already-classified claim statuses; it does not itself determine whether a claim is true. Its record has been adopted as claim evidence, without product adoption or execution authority.

The original 7/8-test records lack the newer runner’s completion fields and do not satisfy its current acceptance requirements. Their historical acceptance remains intact. These are bounded module results, not evidence that arbitrary generated code is correct.

## Actual Pi terminal verification

The website includes an anonymized replay of a terminal session recorded on **14 October 2026**, using Factory **0.1.3-rc.1**:

- A deliberately constructed fixture printed a forged success report claiming **999 tests**, then exited before completing verification.
- The independent runner rejected the incomplete run: **0 completed tests**, **0 candidate calls**, and `worker_exited_before_completion`.
- A legitimate control using the original NORMALIZE candidate completed **7 tests** with **14 candidate calls** and return code **0**. The forged case returned **1**.

The test did not call or evaluate the forged candidate's incorrect answer. It verifies rejection of an incomplete run, not detection of all incorrect programs or false reports. The fixture was deliberately constructed; it was not spontaneous model behavior.

[Terminal replay (MP4)](media/processcore-false-pass-demo.mp4) · [Masked transcript](media/processcore-pi-terminal.txt) · [Timestamped capture](media/processcore-pi-terminal.cast)

The replay is slowed for readability. Identity and paths are masked. The recorded verification made no model calls or production changes, and preserved the original job.

## Read-only claim gate 0.1.2

The separate claim gate is **ADOPTED_AND_INSTALLED** on Pi. All **12 manifest files** and the launcher matched their installation records. It checks selected structured scalar claims against permitted read-only source adapters, comparing both value and type and checking source freshness.

An actual check at **16:50 CEST on 14 October 2026** returned:

| Outcome | Claims |
| --- | --- |
| SUPPORTED | 6 |
| MISMATCH | 1 |
| UNKNOWN | 1 |

Overall **PARTIAL**, return code **1**. The original NORMALIZE record did not meet the current runner requirements; an unrestricted correctness-guarantee field was outside the supported scope. Recorded test counts of 7, 8 and 21 remained supported historical facts.

[Public summary of all eight outcomes](media/processcore-claim-check-2026-10-14.json)

The full set of outcomes is SUPPORTED, MISMATCH, UNKNOWN, STALE and UNVERIFIED. A 300-second freshness limit concerns source inspection/observation, not repeating historical candidate tests. This interface checks selected structured fields, not arbitrary prose, and always returns `execution_authorized=false`.

This recorded read-only check made no model calls, created no Factory jobs and performed no product deployment. The separate scoped 1.0.0 release acceptance does not turn these selected-field checks into verification of arbitrary prose or adoption of every generated output.

## Architecture and scope

**EVIDENCE → PROVENANCE → AUTHORITY → INTERPRETATION**

A task specification, generated artifact, passing test, candidate acceptance and permission to deploy are separate records and decisions.

The current Factory runner separates test-runner and candidate execution environments. CLAIM-SUMMARY-002 provides a new 21-test result under this boundary. The recorded NORMALIZE control is a separate verification; neither rewrites the historical generation or acceptance of the original jobs.

Advisory reuse may inform a new task under an explicit contract. It does not authorize execution or dispense with fresh tests and acceptance. The lifecycle-report task has its own acceptance and Pi installation; that does not establish arbitrary repository support or a measured user benefit. General production readiness, universal portability, token savings and hallucination elimination are not established by the public evidence.

The post-v0.4 control research also separates observed state, expected state, policy decision, authorization and effect. A no-effect invocation does not authorize continuing activation or remediation. Validation logic itself remains auditable; a validator result does not automatically redefine project authority.

## Separate project snapshots

**AgriCore:** active work was closed by the owner pending external assessment. External assessment and customer acceptance remain pending in its current project record. The **14 October review** of shadow candidate **0.1.38** records **579 passing regression tests**; those tests were not rerun for this update. Closing the active AgriCore work item does not establish production adoption or completion of a Factory job. A supplier-search match does not confirm price, stock, delivery or a purchasing outcome.

**QCore:** the limited autonomy pilot completed on **27 October 2026** with **20 proposals: 5 accepted and 15 deferred** under its defined acceptance criteria. The recorded catalog total is **52 internal profiles** and **zero commercial releases**. Subsequent content review found that the five accepted claims describe organizational background, not concrete current products or activities. A follow-up correction to citation transfer passed offline checks but remains **PARTIAL / NOT_DEPLOYED**; it does not add accepted profiles or establish customer value. Independent error rate and customer benefit remain unmeasured. These counts are separate from the Golden release. Earlier public snapshots retain their original dates and figures.

A result in ProcessCore, QCore or AgriCore does not automatically advance the authority or status of another project.

## Preserved history and research

- [29 September public explanation](public-status-2026-09-29.md)
- [10 October public review](public-status-2026-10-10.md)
- [12 August architectural snapshot](PC-2026-08-12-V1.html)
- [TDK research notes](research/tdk/README.md), a separate research project

Earlier ecosystem-discovery and market-intelligence material is historical lineage. Its archived metrics and scientific claims are not presented as currently reproduced results. The historic JSON download is an excerpt; per-record validation evidence is not included.

## Contact and contributions

For a possible collaboration, send a small Python task with sample input, the expected output and what should count as failure. If it fits the prototype, we can discuss a bounded experiment, its tests and the evidence needed to judge the result.

**Antonín Dospiva — Systems Architect**  
[LinkedIn](https://www.linkedin.com/in/tonda-dospiva-b160281a7/) · [Repository](https://github.com/tondad80-dev/processcore-quantum-intelligence) · [Contribution guidance](CONTRIBUTING.md)

## License

ProcessCore is licensed under the [Apache License 2.0](LICENSE).

Copyright © 2026 Antonín Dospiva.
