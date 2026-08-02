# Course/Policy to Skill

**One line:** Book-to-skill's exact mechanic, aimed at training material or an employee handbook instead of a book.

**Generalises from:** [book-to-skill](https://github.com/shaunmarsden/book-to-skill) itself, same index-plus-chapter-files structure, different source material.

**Who it is for:** anyone who has a long course, a training manual, or a policy document they want an AI to consult section by section without loading the whole thing into every conversation. Overlaps closely enough with book-to-skill's actual audience that this may end up as a worked example there rather than a separate repo.

**Status:** Concept only, not built. Kept on the list because the source material genuinely differs in one important way books do not: policies and training material are usually the reader's own organisation's content, not a copyrighted book, which removes the one real constraint book-to-skill had to design carefully around.

## Rough Shape

- Same shape as [book-to-skill's SKILL.md](https://github.com/shaunmarsden/book-to-skill/blob/main/SKILL.md): an index file, one file per section or module, a glossary of the organisation's own specific terms, and a document of every named process or rule
- The main structural difference worth building for: policies and training material often have rules that supersede each other (a newer policy overriding an older one), which a book rarely does. Worth an explicit step checking for contradictions between sections, something book-to-skill's method does not need

## Open Questions

- Separate repo, or a second worked example folder inside book-to-skill itself, given how much of the actual method is identical?
- If it stays separate, what is the actual differentiator worth building (the contradiction-check step above is the strongest candidate) rather than just relabelling book-to-skill?
