# Public website verification — 14 October 2026

This note records the scope and limits of the ProcessCore website review. It updates public documentation; it does not authorize a runtime or product change.

## Source verification

The installed Factory module identifies itself as **0.1.3-rc.1**. All **29** declared files matched their recorded sizes and SHA-256 hashes during the 14 October review.

The original **NORMALIZE** and **SUMMARY** job results identify Factory **0.1.0** as their generation version. Their stored results contain **7** and **8** successful prescribed tests, respectively. The original job files matched their recorded hashes, and the acceptance records matched the referenced result hashes. Both decisions are **ACCEPTED_CANDIDATE**; product adoption is false.

These historical results remain separate from the newer runner verification.

## Recorded current-runner check

[The masked transcript](media/processcore-pi-terminal.txt) and [timestamped capture](media/processcore-pi-terminal.cast) accompany the [actual Pi terminal replay](media/processcore-false-pass-demo.mp4).

The deliberately forged fixture claimed 999 successful tests, then exited before completing verification. The independent runner recorded success false, zero completed tests, zero candidate calls and `worker_exited_before_completion`. The command returned 1.

The legitimate NORMALIZE control completed seven successful tests, with 14 candidate calls and command return code 0. This is a new control run; it does not rewrite the original job.

No model calls or production changes occurred in this recorded verification. The incorrect answer defined by the forged fixture was never evaluated. This check covers rejection of one incomplete-run failure mode, not correctness of arbitrary code or detection of every false report.

## Website checks and corrections

- Before the documentation corrections, all 20 repository-backed public files returned HTTP 200 and matched the repository content.
- The MP4 supported a byte-range request with HTTP 206 and the expected total length of 619,778 bytes.
- Eleven main-page interaction scenarios passed a JavaScript DOM harness, including job and fixture selection, keyboard navigation, playback, pause and reduced-motion behavior.
- Three archive-filter scenarios passed: case-insensitive match, no match and clearing the query. The original four displayed metric values remain available without JavaScript.
- HTML IDs, local link targets and ARIA references were checked.
- The current README was reconciled with the two original jobs and installed runner. The 29 September explanation and 10 October review remain available as historical documents.
- Small-text contrast and anchor offsets under the sticky navigation were improved.
- The August archive has a current presentation notice, its own canonical/share URL and the current contact profile. Its historical metrics and research statements remain unchanged. Content and recorded values remain visible without JavaScript; its filter responds to input changes.

These are source, functional and HTTP checks. This review did not include rendered-page testing in a mobile browser or testing with assistive technology. It is not an accessibility certification or a performance benchmark.

## Historical data and research limits

The August archive's HTML scores differ from its JSON excerpt. The JSON has a 31 July generation date, ten published top actors and no per-record validation evidence. The public download does not contain the complete dataset described in the archived report.

Historical empirical and sensitivity claims in that archive were not independently reproduced in this review. The original mathematical source notation remains visible as text.

The two published Python calculation blocks in the separate TDK notes were reproduced successfully. This establishes reproducibility of those calculations, not empirical confirmation of TDK or independent validation of the cited papers.

GitHub and the linked Golden project page returned HTTP 200. LinkedIn rejected a HEAD request with HTTP 405; that check did not establish whether the profile is available to a signed-in visitor.

No external forums were included.

## Current references

- [Current README](README.md)
- [Current project website](https://tondad80-dev.github.io/processcore-quantum-intelligence/)
- [29 September explanation](public-status-2026-09-29.md)
- [10 October historical review](public-status-2026-10-10.md)
