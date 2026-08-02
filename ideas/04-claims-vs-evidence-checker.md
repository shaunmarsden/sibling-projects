# Claims vs. Evidence Checker

**One line:** Checks whether a tracked status (a project's "on track," a task's "done," a candidate's "strong fit") is actually supported by evidence, or just written down.

**Generalises from:** [pipeline-evidence-review](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/pipeline-evidence-review/SKILL.md), the CRM-specific version of "the recorded field is a claim, not a fact," generalised to any tracked list with a status column.

**Who it is for:** project managers checking status reports, recruiters checking a pipeline of candidates, anyone maintaining a tracker where the field can quietly drift ahead of what actually happened.

**Status:** Built, 2 August 2026. Live at [github.com/shaunmarsden/claims-vs-evidence-checker](https://github.com/shaunmarsden/claims-vs-evidence-checker), with a fictional home renovation punch list catching a false "done" and a stale "in progress", while correctly leaving two genuinely healthy items alone.

## Rough Shape

- **Gather the inputs:** the tracked list with its recorded statuses; whatever notes or evidence exist per item; confirmation the reviewer actually owns or can see evidence for each item, not just that it appears on a shared list
- **Method:** for each item, state the recorded status next to what the evidence actually supports; name the gap if any; suggest what to confirm before trusting the recorded field, never change it directly
- **Guardrails:** never treat the recorded status as evidence of anything; call genuinely healthy, well-supported items healthy rather than manufacturing a problem everywhere
- **Stop when unsafe:** the list has no evidence attached at all, only statuses, in which case there is nothing to check the status against

## Open Questions

- Does the working-states list (the pipeline-evidence-review equivalent of "exploring, qualification incomplete, paused") need to be domain-specific per use case, or can a smaller generic set (on track, blocked, no recent evidence, complete) cover most trackers?
- Worth scoping this to one concrete first use case (project status reports specifically) rather than "any tracker," the same way book-to-skill stayed concrete rather than "any document"
