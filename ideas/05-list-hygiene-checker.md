# List Hygiene Checker

**One line:** Audits any spreadsheet or list for duplicates, missing fields, stale entries and rows that are not real records at all, the same way a CRM export gets checked.

**Generalises from:** [crm-hygiene-review](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/crm-hygiene-review/SKILL.md), stripped of anything CRM-specific.

**Who it is for:** anyone maintaining a mailing list, a contact database, an inventory sheet, or any list that has been added to by more than one person over time and has probably accumulated duplicates and test rows nobody has cleaned up.

**Status:** Concept only, not built.

## Rough Shape

- **Gather the inputs:** the list or export to check, with whatever fields exist; what counts as a required field for this specific list, since that varies by use case
- **Method:** scan for missing required fields; flag likely duplicates separately from merely possible ones, never merge on name similarity alone; flag rows that look like test entries or placeholders rather than real records; flag entries that look complete but have not been touched in a long time
- **Guardrails:** every finding is a suggestion, nothing is merged, deleted or changed automatically; keep confident and uncertain duplicate findings visibly separate; call clean rows clean rather than finding a problem everywhere
- **Stop when unsafe:** the list is missing enough structure (no way to tell what a duplicate would even look like) that a check cannot be done with any confidence

## Open Questions

- Same generic-vs-concrete question as the claims checker: pick one first use case (mailing lists? contact databases?) rather than trying to cover every possible spreadsheet from the start
- Is there a genuinely different failure pattern per list type worth its own guidance (a mailing list's duplicates look different from an inventory sheet's), or does one generic method actually travel well?
