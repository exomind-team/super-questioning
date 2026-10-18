# Pending decisions and next experiments

## Highest priority

1. **Cross-skill activation:** repeat the two ENTP-mode cases with an isolated skill registry and the same Luna xhigh setup. Determine whether the host activates a second Skill, the model merely uses its language, or the `super-questioning` instructions need an explicit boundary. The occurrence in both v5.7.0 and 0.6.1 argues against immediately adding a version-specific rule.
2. **Action reporting:** repeat the bounded write cases and check that the reported link/path matches the actual target and that the target was read back before claiming completion. One 0.6.1 run created the correct file but had a shell check error and a mismatched final link; another completed correctly without a post-write read-back. Independent verification confirmed all requested edits in the pilot.
3. **Real creative artifact:** repeat R5 with an actual poster image or visual artifact. The current test used a text brief, so it did not test visual inspection or the quality of aesthetic comparison.

## Method improvements

- Increase repetitions beyond n=3 per case/version and randomize trial order, while retaining fresh-context Luna xhigh runs.
- Save full anonymized transcripts for scoring instead of reconstructed summaries. Keep the scorer blind to the mapping and hypotheses.
- Add a human-participant round to see whether the problem redefinition is useful to the person, not just coherent to a scorer reading a transcript.
- Keep route-number accuracy secondary. The primary outcome remains a concrete, evidence-grounded change in the user’s problem understanding after several turns.

## Repository work deferred

The public repository audit identified limited structural validation, a self-contained Skill ZIP versus repository-validator distinction, no README/LICENSE, and no behavior-test infrastructure. Those items were not changed in this pilot. The validator is not a behavior-quality gate; decide separately whether to accept a Skill-only package path or retain source-repository checks.

No 0.6.2 Skill patch is included in this handoff. The current evidence does not justify an additional rule before the cross-skill and write-reporting issues are replicated.
