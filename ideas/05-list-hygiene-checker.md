# List Hygiene Checker

Checks any spreadsheet or list for duplicates, missing fields, stale entries and rows that aren't real records, the same way you'd check a CRM export.

It comes from [crm-hygiene-review](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/crm-hygiene-review/SKILL.md), with everything CRM-specific taken out.

It's for anyone keeping a mailing list, a contact database, a stock sheet, or any list that several people have added to over time. Those lists have usually built up duplicates and test rows that nobody has cleared out.

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/list-hygiene-checker) has a made-up running club membership list with five deliberate traps: a clear duplicate, a possible one, a fake test row, two real records with gaps, and one that looks complete but is stale.

## Rough Shape

It needs the list or export, with whatever fields it has, and which fields this list must have filled in, since that varies from list to list.

The method looks for missing required fields. It flags likely duplicates apart from merely possible ones, and never merges on a similar name alone. It flags rows that look like tests or placeholders rather than real records. It flags entries that look complete but nobody has touched in a long time.

Every finding is a suggestion. It never merges, deletes or changes anything itself. It keeps sure and unsure duplicates apart, and calls clean rows clean rather than finding a problem everywhere.

It stops if the list has too little structure to check with any confidence, for example no way to tell what a duplicate would look like.

## Open Questions

- The same question as for the claims checker: pick one first use (mailing lists? contact databases?) rather than trying to cover every spreadsheet from the start.
- Does each type of list fail in its own way, enough to need its own guidance (a mailing list's duplicates look different from a stock sheet's), or does one general method work for all of them?
