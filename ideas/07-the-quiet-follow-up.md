# The Quiet Follow-Up

**One line:** Decides what, if anything, to send next when someone has gone quiet, instead of working through a fixed run of increasingly persistent messages on a timer.

**Generalises from:** [plan-chase-sequence](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/plan-chase-sequence/SKILL.md), applied beyond a quiet sales prospect.

**Who it is for:** recruiters following up on candidates who have gone silent, event organisers chasing no-shows or unconfirmed RSVPs, anyone waiting on an unanswered support ticket or a stalled internal request.

**Status:** Concept only, not built.

## Rough Shape

- **Gather the inputs:** the original exchange or request; what has already been sent and when; anything that has happened since (an out-of-office reply, a role change, genuine silence with no signal); how many follow-ups have already gone out
- **Method:** decide first whether to follow up at all, change the channel or contact, add missing information, or actually stop; only once that decision is made, draft a message anchored to something real, never manufactured urgency
- **Guardrails:** the anchor must be something real, never invented pressure or a fake deadline; never remind the person you have already followed up unless this is genuinely the last message; recognise when continuing to push stops being useful
- **Stop when unsafe:** there is a specific signal that this should not be chased further at all (an explicit decline, someone who has left, a clear no) and the request is to chase anyway

## Open Questions

- Does the decision tree (chase now, wait, change contact, add evidence, stop) hold up outside sales, or does each domain (recruiting vs. events vs. support) need its own version of "when to stop"?
- Worth a fictional worked example per domain, given how differently a recruiting chase and a support-ticket chase actually feel in practice
