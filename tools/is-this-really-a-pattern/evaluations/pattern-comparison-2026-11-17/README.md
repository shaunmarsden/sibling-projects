# Pattern Rule Comparison Results

Neither candidate meets the frozen adoption rule. The percentage change resolves three baseline refusals, but adds a confidence-reporting omission in one paired case. The template baseline already handles same-wording patterns, and its candidate adds an unsupported investigation claim. I have left both live files unchanged.

Start with the paired results below. These are small synthetic comparisons, not general reliability or cross-tool compatibility evidence.

## What Ran

I ran 24 isolated Codex subagent trials on 17th November 2026: six cases, two versions and one response per pair for each of two separate comparisons. There were no retries or direct API calls.

The [plan](../../checks/pattern-test/plan.md), [answer key](../../checks/pattern-test/answer-key.json), exact input packets and [registration](registration.json) were committed in `1f3c6d9` before the first trial. The [manifest](../../checks/pattern-test/manifest.json) preserves the original NOT RUN preparation status and hashes. It is not the completion record.

The percentage comparison changed one guardrail in the skill and supplied no template. The template comparison changed one placeholder, using the baseline skill in both arms. No combined candidate was tested.

Each runner had a fresh context without this conversation. It received only the shared wrapper and one anonymous packet: skill, optional template, task and one case. It was told to read that packet once and not use other tools or files. These were instruction-level restrictions, not an independently audited sandbox. Shared Codex/global instructions still applied.

No model or reasoning override was set. The interface inherited the parent configuration, but did not expose an exact model identity, snapshot, sampling settings, token usage or internal inference-call count in the returned result. These are Codex subagent trials, not claims of one API request each.

I graded the returned text after seeing both variants and the answer key. This is non-blind, non-independent review. All returned texts are preserved in the linked JSON `text` fields, including non-ASCII punctuation. No output was rewritten to fix an error.

## Percentage Rule

The [source cases](../../checks/pattern-test/cases.json) define the counting units and requests. The six required conclusions are fixed in the answer key.

| Case | Baseline output | Candidate output | Required conclusion and other findings |
| --- | --- | --- | --- |
| P1: five-entry share | [R23](outputs/R23.json) | [R03](outputs/R03.json) | Baseline gives 3/5 but refuses the percentage. Candidate gives 60% of entries, not customers. Both omit some per-finding confidence explanations. |
| P2: all-product customers | [R01](outputs/R01.json) | [R04](outputs/R04.json) | Both correctly refuse the wider rate with no population denominator. Candidate's optional 60% is explicitly log entries only. |
| P3: filtered extract | [R24](outputs/R24.json) | [R11](outputs/R11.json) | Both correctly leave the all-feedback share unknown. |
| P4: incidents versus rows | [R21](outputs/R21.json) | [R22](outputs/R22.json) | Baseline counts 1/2 but refuses the percentage. Candidate gives 50% of incidents, not 3/5 rows. Its confidence level covers arithmetic, not the two isolated findings. |
| P5: zero numerator | [R05](outputs/R05.json) | [R18](outputs/R18.json) | Both correctly give 0/4 = 0% of this log. Baseline omits confidence levels for some findings. |
| P6: represented customers | [R19](outputs/R19.json) | [R16](outputs/R16.json) | Baseline gives 2/4 but refuses the percentage. Candidate gives 50% of represented customers and separates the coincidentally equal entry share. Baseline omits per-finding confidence levels. |

Both versions have no automatic failures in this comparison. The baseline meets the requested conclusion in three cases; the candidate does so in all six. That is a count of these fixed conclusions, not a measured general accuracy rate. The baseline already handled zero, unknown denominators and wider-rate refusal, so the candidate gets no improvement credit for those.

The candidate resolves check 3 in P1, P4 and P6. However, check 5 in P4 is a new Needs correction finding: R22 says "Confidence is high in the incident count and percentage", but does not explain a low/medium/high level for the two isolated-signal findings. R21 explicitly attaches high confidence to its isolated-signal conclusion using incident identities. The frozen plan asks for finding-level confidence, not just confidence in arithmetic.

Under the rule requiring no new correction on any case, the percentage candidate does not qualify for adoption. This does not prove the rule change caused the omission; with one response per pair, variation is a plausible explanation. It does mean this run does not clear the pre-agreed gate.

## Pattern Template

| Case | Baseline output | Candidate output | Required conclusion and other findings |
| --- | --- | --- | --- |
| T1: identical words, same cause | [R06](outputs/R06.json) | [R13](outputs/R13.json) | Both find the supported two-event cable pattern. The baseline already handles the target case. |
| T2: different words, same cause | [R08](outputs/R08.json) | [R12](outputs/R12.json) | Both find the supported two-event cable pattern. |
| T3: identical words, different causes | [R02](outputs/R02.json) | [R09](outputs/R09.json) | Both keep cable and timer diagnoses apart. Candidate also says two events are too small to establish a recurring cause; that is the wrong reason here. The causes differ, whereas two supported same-cause events meet the skill's threshold. |
| T4: unknown causes | [R07](outputs/R07.json) | [R17](outputs/R17.json) | Both distinguish recurring symptoms from unestablished causes without asserting that no investigation happened. |
| T5: two people, one event | [R20](outputs/R20.json) | [R15](outputs/R15.json) | Both count two reports as one event, not a recurring-cause pattern. |
| T6: supported pair plus unknown | [R14](outputs/R14.json) | [R10](outputs/R10.json) | Both keep E3 out of the confirmed cable count. Both omit a confidence level for its separate isolated finding. Candidate invents investigation history. |

All six main grouping conclusions meet the answer key for both versions. The baseline has no automatic failures. The candidate has one: R10 says "E3 has no investigation or diagnosis", but the case says only that no diagnosis or investigation record was supplied. Missing records do not prove that no investigation happened. That triggers the frozen invented-investigation-history rule, even though the cable grouping itself is right.

R09's sample-size explanation is Needs correction, not an automatic failure: it does not invent a diagnosis or reverse the main grouping. The candidate resolves no baseline defect and adds factual problems, so it does not qualify for adoption.

## Full Review and Preservation

The [review record](review.json) gives each of the five judgements for all 24 outputs, with source case IDs and output excerpts. It records automatic failures separately. No output is Not assessable; all returned in full. Check 5 was applied to the findings' confidence, supporting entries, counter-evidence or its stated absence, limits and human control. A clearly scoped confidence statement can cover multiple findings, but an arithmetic-only confidence statement does not cover separate pattern findings.

The [completion record](completion.json) records counts and hashes of the archived returned-text files. Input hashes still match the pre-run manifest. The live SKILL.md, live template, source logs, original outputs and illustration reviews are unchanged.

The offline checker and its unit tests check documentation and packet integrity, not model behaviour. The raw-output JSON is deliberately not normalised by the Markdown punctuation check.

## Limits

These twelve short synthetic cases and single responses cannot establish stable regression rates, broad quality, real-user usefulness or compatibility with other tools. The same reviewer designed the cases and scored them. There was no independent human or blinded review. The environment and exact model identity limits above matter.

I have not rerun failures, edited the candidate after seeing results or weakened the adoption rule. Any revised candidate or further comparison needs a new frozen packet and separate approval. Preparing and running a comparison is useful evidence even when neither change is adopted.
