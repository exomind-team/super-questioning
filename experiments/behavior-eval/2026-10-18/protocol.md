# Protocol and blind procedure

## Arms and scope

The pilot compared three pinned Skill commits: formal baseline v5.7.0 (`53312ab`), experimental v0.6.0 (`49d43dc`), and experimental v0.6.1 (`dba6e7e`). Each version received each of six scenario classes once: one run per version × scenario, 18 total fresh-context sessions (three runs per scenario across all versions). Every session used Luna xhigh. All test agents were started without prior conversation context and were directed to use one masked Skill package for one scenario. The host-wide Skill registry remained available and was not isolated. The metadata version string was normalized to `masked`; the v5.7.0 package included its referenced runtime files, while the two experimental packages were self-contained.

The six scenarios were: same-message activation plus write authorization; evidence dispute overlapping with counterargument; creative dissatisfaction without a visual reference; vague goal and problem redefinition; mature decision with a bounded edit; and skip, limited delegation, and stop. Write requests used unique temporary fixtures. Other fixtures were synthetic and read-only.

## Scoring

The test runs were assigned randomized labels A/B/C. After all runs, a fresh no-context Luna xhigh scorer received a redacted, anonymized summary packet with the version mapping withheld. It scored next-action fit, substantive progress, evidence discipline, user agency/authorization, and efficiency. A first scoring packet omitted one observed ENTP-mode declaration; we corrected the packet and used a second fresh blind scoring pass as the reported result. The mapping was revealed only after the corrected scoring pass completed.

## Blindness and reproducibility limits

This was a masked randomized comparison, not perfect double-blind testing: the acting model necessarily read the Skill text it was following and could infer stylistic differences. The system-level Skill registry was not isolated; despite the trial wrapper, two sessions emitted an unrequested ENTP-mode preamble. That may reflect cross-skill routing or model behavior and needs a test in an isolated registry.

Trials were grouped by scenario, and labels were randomized to version identities; there was no model seed control. The scorer evaluated summarized reconstructed transcripts rather than a complete raw turn log. The visual scenario used a written poster brief rather than an image. Interactive question UI tools were disabled so each trial remained a text conversation. These constraints make the totals directional only.

All scenario names and assets in this report are synthetic. Product names, absolute local paths, and private design notes have been removed.
