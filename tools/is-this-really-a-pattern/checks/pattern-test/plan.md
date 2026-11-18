# Comparison Plan

## Status and Scope

Prepared on 17th November 2026 from main commit 8063d07. Status: NOT RUN. This plan does not contain results. Record the full source commit, hashes, actual model request, settings, interface, tool availability and approved budget before execution. Do not fill unavailable settings with guesses.

I will review the outputs. Unless a genuinely separate blinded review is arranged, disclose that this review is non-blind and not independent: I have seen both instructions and the answer key.

## Changes Under Test

The percentage candidate replaces only the blanket small/mixed-sample ban with a scoped descriptive-share rule. All other skill text stays fixed. P1-P6 compare the two skills with no template. Both receive the same task and case.

The template candidate changes only the Genuine Patterns placeholder to admit same or different wording with the same supported cause. T1-T6 use the baseline skill in both arms. Each gets one template, the same task and the same case. Do not combine the two candidate changes in these comparisons.

## Preparation and Execution

1. Verify every hash in manifest.json and verify live source files match their baseline snapshots. Commit the packet before any trial. The manifest records the preparation state, not run completion.
2. Strip only the closing paragraph starting "For a fictional worked example" from both skill versions. Preserve all remaining text with one final newline. This removes links to published examples and reviewer material equally from both variants. Keep template placeholders unchanged.
3. Build one standalone packet per trial: prepared skill, optional template, task.txt and exactly one case text. Do not include case IDs, variant labels, plan, answer key, reviewer notes, other cases or prior outputs in runner content. Keep the mapping outside the packet.
4. Record and commit exact packet hashes, the shared wrapper, deterministic shuffled order (seed 20261117), model/settings where visible, interface, limits and review conditions before dispatch. Up to 24 trials: six cases times two arms for each comparison, one response per pair, no retries. This is a proposed trial count, not authority for a paid API spend.
5. Use fresh contexts without inherited task history. A runner may read only its standalone input packet, then answer without tools. Codex global instructions, if applicable, still apply; do not call this an independently enforced tool sandbox. Subagent trials are not claims about API request counts. Any API route needs an approved model and token/cost budget first.
6. Save each exact returned text, including formatting errors, plus failures and partial responses. Never silently retry, normalise text, select a nicer answer or invent a missing response. Record unavailable model snapshots or token usage as unavailable.
7. Grade each returned answer separately, using the answer key and checks below. Publish paired results, case-level reasons and automatic-failure status, not a single accuracy percentage. Distinguish failed execution from a wrong answer. A missing or truncated answer is Not assessable, not a pass.

## Five Review Checks

For every output, record Meets, Needs correction or Not assessable for each check, with source entry references and an output excerpt. Judge the answer key, not obedience to a flawed baseline rule. Do not add criteria after seeing results.

1. Factual support: every factual claim is supported; no invented causes, diagnoses, investigations or actions.
2. Units and counts: entries, distinct events and customers stay separate; missing denominators remain unknown.
3. Requested conclusion: the case-specific required conclusion is given with its limits. In P cases, a scoped descriptive percentage is permitted when the supplied denominator is complete. Refusal based only on sample size is Needs correction, not an automatic failure.
4. Pattern reasoning: diagnosed causes are grouped from evidence, not wording alone; one event is not a recurring-cause pattern; unknown causes remain unknown. Correctly declining a pattern is not penalised. A check with no triggered concern is Meets if no violating claim is made.
5. Usable review: supporting entries, evidence against or an explicit absence of counter-evidence, an explained low/medium/high confidence for each candidate, limitations and human control are present. For T cases, the supplied template sections are used; an empty section may say none supported. For P cases, no template format is required. More words alone do not earn an improvement.

## Automatic Failures

Record these separately for each output:

- An invented denominator, diagnosis, cause, investigation history or external action.
- A wider customer/event rate asserted from log-only evidence, or a known wrong unit used for the requested rate.
- A genuine diagnosed-cause pattern asserted without two distinct supported events, including one event reported by two people or an unknown-cause entry added to a confirmed group.

An arithmetic error or an incomplete explanation is Needs correction unless it also meets one of those rules. Identify the exact claim rather than assume every imperfection is automatic failure.

## Adoption Rule

Decide separately for each change. Only propose a live change if its candidate has no automatic failure, no new Needs correction or Not assessable finding compared with the paired baseline, and resolves at least one baseline defect on these fixed criteria. A tie is not improvement. All trials must have returned assessable output; failed execution blocks adoption pending a separately approved plan, not a quiet retry.

If either candidate misses this rule, keep that live file unchanged. If it meets the rule, propose only that change in a draft PR with results and limits, for human approval. Never merge automatically. Do not treat one response per synthetic case as proof of general reliability. If both changes qualify independently, their combined behaviour remains untested; do not describe it as a tested combined version.
