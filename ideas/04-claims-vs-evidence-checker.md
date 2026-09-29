# Claims vs. Evidence Checker

Checks whether evidence backs up a tracked status (a project's "on track," a task's "done," a candidate's "strong fit"), or whether someone just wrote it down.

It comes from [pipeline-evidence-review](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/pipeline-evidence-review/SKILL.md), the CRM version of "the recorded field is a claim, not a fact," and applies it to any list with a status column.

It's for project managers checking status reports, recruiters checking a list of candidates, and anyone keeping a tracker where the status can quietly run ahead of what happened.

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/claims-vs-evidence-checker) has a made-up punch list for a home renovation. It catches a false "done" and a stale "in progress", and leaves two healthy items alone.

## Rough Shape

It needs the list with its recorded statuses, whatever notes or evidence exist for each item, and confirmation that you own each item or can see its evidence, not just that it's on a shared list.

The method puts each item's recorded status next to what the evidence supports, and names any gap. It suggests what to confirm before you trust the recorded status. It never changes the status itself.

It must never treat the recorded status as evidence of anything. It calls well-supported items healthy rather than inventing a problem everywhere.

It stops if the list has only statuses and no evidence, because then there's nothing to check the statuses against.

## Open Questions

- Does the list of working states (pipeline-evidence-review's version of "exploring, qualification incomplete, paused") need to suit each use, or can a smaller general set (on track, blocked, no recent evidence, complete) cover most trackers?
- Is it worth starting with one concrete use (project status reports) rather than "any tracker," the same way book-to-skill stayed concrete rather than "any document"?
