# Public status review — 10 October 2026

> **Historical review:** this document records evidence available on 10 October 2026. Its current-state statements refer to that date. For the reviewed 14 October Factory status, see the [current README](README.md) and [dated verification](public-status-2026-10-14.md). The original results below are preserved.

This review updates the website's explanation, not the accepted runtime baseline.

## Evidence levels

| Item | Source and scope | Status |
| --- | --- | --- |
| ProcessCore observation runtime | Accepted public baseline described in [README](README.md) | v0.4 remains the reference. |
| Bounded Factory run | Reconciled 29 September public state in [29 September explanation](public-status-2026-09-29.md#ai-factory--reusable-software-factory-target) | One model invocation, one isolated candidate, static AST/compile checks passed. |
| Factory reuse | Public baseline available on 10 October | A second distinct job has not been demonstrated in the reconciled public evidence. |
| AgriCore development | Owner-provided project status on 10 October | Version 0.1.32; 20 archived candidates; supplier emails prepared, none sent in the reported step. Live search and supplier delivery were not independently verified in this review. |
| QCore audit | Latest project audit report and inspected snapshot discussed on 10 October | 42,122 SCOUTED records; none FOR_WORKER. End-to-end event-log-to-registry transfer and cost causality remain unresolved. |

AgriCore's latest development version is separate from the reconciled ProcessCore Factory result. This review does not establish that all AgriCore changes were generated, adopted or deployed through that Factory path.

The candidate summary is documentation of the public baseline, not a new independently reproduced runtime experiment. Private runtime artifacts, internal network addresses and credentials are not published.

## Website changes

- Separate the date of this page review from the 29 September reconciled public reference.
- Put the concrete Factory result before the architecture discussion.
- Describe the practical AgriCore workflow and label its latest snapshot as owner-reported.
- Keep the open QCore handoff and cost questions explicit.
- Add a direct link to the separate [Golden product page](https://tondad80-dev.github.io/commercial-golden-api-deploy/).
- Retain the stable baseline, project boundaries and historical lineage.

The canonical project website remains:
https://tondad80-dev.github.io/processcore-quantum-intelligence/

The bare user-site address returned 404 in this review. Repairing that address requires its own user-site repository/configuration and is not accomplished by this project-page update.
