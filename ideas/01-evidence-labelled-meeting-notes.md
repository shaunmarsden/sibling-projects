# Evidence-Labelled Meeting Notes

**One line:** Turn any meeting transcript into notes that keep confirmed facts, estimates and pure assumptions visibly separate, so nothing invented gets treated as agreed.

**Generalises from:** the fact/estimate/assumption discipline in [extract-post-call-evidence](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/extract-post-call-evidence/SKILL.md), stripped of anything sales-specific (no CRM suggestions, no next-step framing tied to a deal).

**Who it is for:** anyone who leaves a meeting and has to write it up, project managers, consultants, recruiters, anyone whose job involves "what did we actually agree" being different from "what does everyone remember agreeing."

**Status:** Built, 2 August 2026. Live at [github.com/shaunmarsden/evidence-labelled-meeting-notes](https://github.com/shaunmarsden/evidence-labelled-meeting-notes), with a fictional worked example (Fernbridge Digital) built with deliberate traps, the same pattern as [book-to-skill](https://github.com/shaunmarsden/book-to-skill)'s Art of War demo.

## Rough Shape

- **Gather the inputs:** a transcript or clear notes from a meeting; who was in it; what the write-up needs to support (a summary for absent stakeholders, an action list, a decision record)
- **Method:** separate what was explicitly said from what is being inferred; label every action with who owns it and by when, only if that was actually stated; flag anything that sounds like a decision but was never confirmed as one
- **Guardrails:** never invent an owner or a date for an action that was left open; never upgrade "someone mentioned" to "it was agreed"
- **Stop when unsafe:** the transcript is too thin or garbled to support any confident labelling

## Open Questions

- Does this need a single fixed output format, or should the shape flex by meeting type (status update vs. negotiation vs. brainstorm)?
- Worth a fictional worked example the same way Hartwell works for the sales repo, a generic business meeting rather than a sales call
