# Pattern Rule Comparisons

**Status: Compared once on 17th November 2026.** Read the [results and limits](../../evaluations/pattern-comparison-2026-11-17/README.md). Neither candidate met the adoption rule; the live files are unchanged. The manifest's NOT RUN status is the preserved preparation record, not the completion status.

Start with the [comparison plan](plan.md). The [cases](cases.json) are synthetic. The [answer key](answer-key.json) and plan are reviewer-only material and must not be supplied to a runner.

Two comparisons isolate separate changes:

- Percentage rule: [baseline skill](baseline-skill.txt) against [candidate skill](candidate-skill.txt), without a template.
- Template: the same baseline skill in both arms, with either [baseline template](baseline-template.txt) or [candidate template](candidate-template.txt).

The [manifest](manifest.json) records file hashes. Plain-text snapshots preserve their original source bytes and relative links; those links belong to the live files' original locations, not this archive. The offline checker checks the live Markdown links, not links embedded in archived text. Runners must not follow them. Before execution, remove the final source-pointer paragraph from both skill versions as the plan specifies.

The [task](task.txt) and [runner wrapper](runner-wrapper.txt) are shared. Model, settings, interface and budget must be recorded and committed in a dated execution registration before the first trial. A prepared packet alone is not execution authorisation.

The live [skill](../../SKILL.md), [template](../../templates/pattern-review-template.md), source logs and historical outputs remain unchanged. No cross-tool compatibility or real-world reliability follows from a small synthetic comparison.
