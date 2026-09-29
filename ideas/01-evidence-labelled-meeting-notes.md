# Evidence-Labelled Meeting Notes

Turn any meeting transcript into notes that keep confirmed facts, estimates and plain assumptions apart, so nothing made up gets treated as agreed.

It comes from the fact, estimate and assumption rules in [extract-post-call-evidence](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/extract-post-call-evidence/SKILL.md), with everything sales-specific taken out: no CRM suggestions, and no next steps tied to a deal.

It's for anyone who has to write up a meeting: project managers, consultants, recruiters, anyone whose job turns on the gap between "what did we actually agree" and "what does everyone remember agreeing."

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/evidence-labelled-meeting-notes) has a made-up worked example (Fernbridge Digital) full of deliberate traps, the same pattern as [book-to-skill](https://github.com/shaunmarsden/book-to-skill)'s Art of War demo.

## Rough Shape

It needs a transcript or clear notes from the meeting, who was there, and what the write-up is for: a summary for people who missed it, an action list or a record of decisions.

The method separates what people said from what it infers. It gives each action an owner and a date only if someone stated them. It flags anything that sounds like a decision but nobody confirmed.

It must never make up an owner or a date for an action left open. It must never turn "someone mentioned" into "it was agreed".

It stops if the transcript is too thin or garbled to label with any confidence.

## Open Questions

- Does this need one fixed output format, or should the shape change by meeting type (status update, negotiation, brainstorm)?
- Is it worth a made-up worked example, the way Hartwell works for the sales repo, using a general business meeting rather than a sales call?
