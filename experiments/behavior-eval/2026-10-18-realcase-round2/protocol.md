# Protocol

## Question

Does 0.6.2 improve authorized demo-first execution, delegated routine choices, feedback uptake, and verification/reporting compared with 0.6.1 on tasks drawn from prior Skill use?

This comparison tests only 0.6.1 vs 0.6.2. It does not compare either version with 5.7.0.

## Cases

Three reusable task patterns were derived from historical conversations found through session-extract and rewritten as synthetic fixtures:

1. Dashboard critique: produce a bounded mock demo, then reduce copy and make a status trend visible.
2. Decision alignment: continue from settled decisions, keep credential policy unresolved, make a plan and mock demo only, then report assumptions and unknowns.
3. Routing graph: build a single-file editable one-way graph with optional routing and specific model endpoints, then incorporate feedback.

Prompts and fixtures were normalized for the test. Raw conversations, session IDs, account/project names, local paths, screenshots, and credentials are not part of this branch.

## Runs and blinding

- 12 valid runs: 3 cases × 2 versions × 2 fresh contexts per case/version cell.
- Each trial used Luna with xhigh reasoning and one assigned Skill copy, treated as already activated.
- Trial participants were not told whether their copy was A or B, nor the version mapping.
- A separate no-context Luna xhigh assessor received only the A/B packet, task materials, outputs, and a scoring rubric. The assessor returned its score before the mapping was unsealed.
- Mapping after unsealing: A = 0.6.2-pre_alpha; B = 0.6.1-pre_alpha.
- The coordinator did not inspect the mapping until the assessor returned its report.

## Scoring

The blind assessor scored five criteria from 0 to 2 (maximum 10 per trial): intent/constraint fidelity; action choice and momentum; feedback adaptation; assumption/unknown handling; and verification/reporting. The rubric instructed the assessor not to penalize the text-only constraint that prevented browser rendering.

## Deviations and limits

- One initial routing trial used the shared scratch path because its isolated fixture lacked routing.html. That attempt was excluded. The isolated baseline was restored from the other three routing fixtures after their SHA-256 hashes matched, then the same masked trial was rerun with a fresh Luna xhigh context at the exact path. Only the corrected run is counted.
- The model scored supplied source and participant reports; no browser rendering or interaction playback was provided.
- Only two repetitions were run per version × case cell. A single assessor and a broad rubric produced a 10/10 ceiling.
- Fresh conversation context was used, but the host Skill registry may not have been fully isolated. Participants were instructed to use only the assigned Skill file.
- The tasks are anonymized reconstructions, not live user sessions. No direct measure of whether a human's understanding or judgment changed was collected.
