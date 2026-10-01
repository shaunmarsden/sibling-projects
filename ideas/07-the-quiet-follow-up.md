# The Quiet Follow-Up

Decides what, if anything, to send next when someone has gone quiet, instead of sending a fixed run of ever more pushy messages on a timer.

It comes from [plan-chase-sequence](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/plan-chase-sequence/SKILL.md) and applies it beyond a quiet sales prospect.

It's for recruiters chasing candidates who have gone silent, event organisers chasing no-shows or unconfirmed RSVPs, and anyone waiting on an unanswered support ticket or a stalled internal request.

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/the-quiet-follow-up) has a made-up worked example about a food bank's volunteer coordinator. It tests three outcomes: follow up now, answer something first, and stop.

## Rough Shape

It needs the original message or request, what has been sent since and when, anything that has happened since (an out-of-office reply, a change of role, or silence with no signal at all), and how many follow-ups have gone out.

The method first decides whether to follow up at all, change the channel or contact, add missing information, or stop. Only then does it draft a message, built on something real.

The message must rest on something real, never invented pressure or a fake deadline. It never reminds the person you've already followed up unless this really is the last message. It knows when pushing further stops helping.

It stops if there's a clear sign this shouldn't be chased any more (an outright decline, someone who has left, a clear no) and the request is to chase anyway.

## Open Questions

- Does the decision tree (chase now, wait, change contact, add evidence, stop) hold up outside sales, or does each field (recruiting, events, support) need its own version of "when to stop"?
- Is it worth a made-up worked example for each field, given how different a recruiting chase and a support-ticket chase feel in practice?
