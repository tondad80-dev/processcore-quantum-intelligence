# ProcessCore

**Evidence before interpretation.**

ProcessCore is an independent engineering project developing checks for AI-generated Python modules on Raspberry Pi. It pairs explicit specifications with predefined tests and recorded results. Deployment remains a separate human decision.

[Website](https://tondad80-dev.github.io/processcore-quantum-intelligence/) · [Dated verification](public-status-2026-10-14.md)

## Reviewed public state — 14 October 2026

Observation runtime **v0.4** remains the accepted public reference baseline. The separately versioned Factory module **0.1.3-rc.1** is installed on Raspberry Pi. All **29 manifest files** matched their declared size and SHA-256 during this review.

Two distinct original Factory **0.1.0** jobs have stored test and acceptance evidence:

| Original job | Prescribed tests | Recorded decision | Product adoption |
| --- | --- | --- | --- |
| NORMALIZE | 7 passed | Accepted candidate | Not deployed into a product |
| SUMMARY | 8 passed | Accepted candidate | Not deployed into a product |

The original job files and the acceptance records' references to their results matched their stored hashes. Each job recorded one model invocation. These are bounded module results, not evidence that arbitrary generated code is correct.

## Actual Pi terminal verification

The website includes an anonymized replay of a terminal session recorded on **14 October 2026**, using Factory **0.1.3-rc.1**:

- A deliberately constructed fixture printed a forged success report claiming **999 tests**, then exited before completing verification.
- The independent runner rejected the incomplete run: **0 completed tests**, **0 candidate calls**, and `worker_exited_before_completion`.
- A legitimate control using the original NORMALIZE candidate completed **7 tests** with **14 candidate calls** and return code **0**. The forged case returned **1**.

The test did not call or evaluate the forged candidate's incorrect answer. It verifies rejection of an incomplete run, not detection of all incorrect programs or false reports. The fixture was deliberately constructed; it was not spontaneous model behavior.

[Terminal replay (MP4)](media/processcore-false-pass-demo.mp4) · [Masked transcript](media/processcore-pi-terminal.txt) · [Timestamped capture](media/processcore-pi-terminal.cast)

The replay is slowed for readability. Identity and paths are masked. The recorded verification made no model calls or production changes, and preserved the original job.

## Architecture and scope

**EVIDENCE → PROVENANCE → AUTHORITY → INTERPRETATION**

A task specification, generated artifact, passing test, candidate acceptance and permission to deploy are separate records and decisions.

The current Factory runner separates test-runner and candidate execution environments. The isolated control above is a new verification; it does not rewrite the historical generation or acceptance of the original jobs.

Advisory reuse may inform a new task under an explicit contract. It does not authorize execution or dispense with fresh tests and acceptance. End-to-end reuse with fresh acceptance and product integration remains to be demonstrated. General production readiness, universal portability, token savings and hallucination elimination are not established by the public evidence.

The post-v0.4 control research also separates observed state, expected state, policy decision, authorization and effect. A no-effect invocation does not authorize continuing activation or remediation. Validation logic itself remains auditable; a validator result does not automatically redefine project authority.

## Separate project snapshots

AgriCore is a development demonstrator with its own runtime and project authority. The reviewed **0.1.38** shadow candidate has a stored result of **579 passing regression tests**. Production adoption and Factory job closure are not established by that result. A supplier-search match does not confirm price, stock, delivery or a purchasing outcome.

The **14 October** QCore review found three running services, 25 internal trial profiles and no commercially released profiles. Service activity and queue size do not establish customer-ready data.

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
