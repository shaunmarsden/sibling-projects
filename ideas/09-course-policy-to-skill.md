# Course/Policy to Skill

Book-to-skill's method, aimed at training material or a staff handbook instead of a book.

It comes from [book-to-skill](https://github.com/shaunmarsden/book-to-skill) itself: the same index and chapter files, with different source material.

It's for anyone with a long course, a training manual or a policy document they want an AI to consult section by section, without loading the whole thing into every conversation. Its audience overlaps so much with book-to-skill's that it may end up as a worked example there rather than a separate repo.

I built it on 2 August 2026 as a second worked example inside [book-to-skill](https://github.com/shaunmarsden/book-to-skill), not its own repo, which answered this file's own open question. `SKILL.md` now covers training material and policies as well as books, with one real addition: a step that checks for contradictions, since a policy can overrule itself between sections in a way a book's chapters rarely do. The second worked example is lighter on purpose than the first. It's a made-up remote work policy in two sections, where the later section overrules the earlier one for certain roles.

## Rough Shape

It has the same shape as [book-to-skill's SKILL.md](https://github.com/shaunmarsden/book-to-skill/blob/main/SKILL.md): an index file, one file per section or module, a glossary of the organisation's own terms, and a document listing every named process or rule.

The main difference to build for is that policies and training material often have rules that overrule each other (a newer policy replacing an older one), which a book rarely does. It needs a step that checks for contradictions between sections, which book-to-skill's method doesn't.

## Open Questions

- A separate repo, or a second worked example folder inside book-to-skill, given how much of the method is the same?
- If it stays separate, what's the real difference worth building (the contradiction check above is the strongest candidate), rather than just renaming book-to-skill?
