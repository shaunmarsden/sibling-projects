---
name: sibling-projects-router
description: Work out which of the sibling-projects tools actually fits a described situation, and hand off to it cleanly. Use when someone describes a problem in their own words and is not sure which of the eighteen tools applies, or when two tools sound similar and it matters which one is actually right. Do not use this to solve the underlying task yourself; it recommends a route, it does not do the work of the tool it recommends.
---

# Sibling Projects Router

You do not need to install anything to try this once: copy this whole file, paste it as your first message in any AI chat tool, then follow it with your actual situation.

Someone describing a real situation rarely names the tool they need; they describe the problem. This reads that description and hands off to the right existing tool, without trying to solve the task itself and without inventing a new method one of the eighteen already covers.

## Gather the Inputs

- The actual goal, in your own words, not a guess at which tool you mean
- Whether this is still open and undecided, or has already closed one way or another
- Whether this is about one thing, or several similar-sounding things you are trying to compare
- The main blocker or open question, if one is apparent

## Route to the Right Tool

| Situation described | Route to |
| --- | --- |
| Writing up a meeting and want confirmed facts kept separate from estimates and assumptions | [Evidence-Labelled Meeting Notes](https://github.com/shaunmarsden/evidence-labelled-meeting-notes) |
| Want a scoring rubric for judging AI output in a specific domain, not a fixed one that does not fit | [Build Your Own AI Output Rubric](https://github.com/shaunmarsden/build-your-own-rubric) |
| Have a repeated task and want a proper, bounded skill file instead of a one-off prompt | [Skill Author](https://github.com/shaunmarsden/skill-author) |
| Have a book, course, or policy document and want it structured as a skill instead of loaded whole | [Book to Skill](https://github.com/shaunmarsden/book-to-skill) |
| A tracked status, on track, done, in progress, might not actually match the evidence behind it | [Claims vs. Evidence Checker](https://github.com/shaunmarsden/claims-vs-evidence-checker) |
| A list or spreadsheet might have duplicates, missing fields, or stale rows | [List Hygiene Checker](https://github.com/shaunmarsden/list-hygiene-checker) |
| Something has already failed or closed, and you want to know if it is genuinely over | [Post-Mortem Builder](https://github.com/shaunmarsden/post-mortem-builder) |
| Someone has gone quiet and you are deciding whether, and what, to send next | [The Quiet Follow-Up](https://github.com/shaunmarsden/the-quiet-follow-up) |
| A customer complaint has come in and you want to diagnose the real driver before replying | [Diagnose Before You Respond](https://github.com/shaunmarsden/diagnose-before-you-respond) |
| Weighing a decision (a job offer, a vendor, a project idea) with more than one aspect to judge | [Is This Actually a Good Fit?](https://github.com/shaunmarsden/is-this-a-good-fit) |
| Someone else has agreed to present your case to a third party you cannot be in the room for | [Brief Your Advocate](https://github.com/shaunmarsden/brief-your-advocate) |
| Need a written case for a decision-maker who was not part of the original conversations | [Make the Case](https://github.com/shaunmarsden/make-the-case) |
| Want a weekly view of your own work composed from what you already have, no dashboard | [Weekly Roundup Builder](https://github.com/shaunmarsden/weekly-roundup-builder) |
| A decision is still open and stalled, "let me think about it" has gone on longer than it should | [What's Actually Causing This Delay?](https://github.com/shaunmarsden/whats-causing-this-delay) |
| You keep seeing what sounds like the same complaint or issue across several instances and want to know if it is one real pattern | [Is This Really a Pattern?](https://github.com/shaunmarsden/is-this-really-a-pattern) |
| Sending the same template message to more than one recipient, or one recipient who needs to forward part of it | [Personalise, Don't Templatise](https://github.com/shaunmarsden/personalise-dont-templatise) |
| Have an important conversation coming up and the useful information is scattered | [Prep Card Builder](https://github.com/shaunmarsden/prep-card-builder) |
| Reaching out cold to someone you do not know, and want an opener anchored to something real rather than a generic observation | [First Contact That Isn't Generic](https://github.com/shaunmarsden/first-contact-that-isnt-generic) |

### Common Confusions Worth Checking Explicitly

- **Post-Mortem Builder versus What's Actually Causing This Delay:** Post-Mortem Builder is for something that has already closed, failed, or gone quiet long enough to be treated as over. What's Actually Causing This Delay is for a decision still open and undecided, not yet closed either way. If nobody has said no and nothing has actually ended, route to the delay diagnosis, not the post-mortem.
- **Diagnose Before You Respond versus What's Actually Causing This Delay:** a complaint names a specific stated issue that needs a reply. A stalled decision usually has no specific stated concern at all, just delay. If something specific was actually said, route to diagnosing the complaint; if the person has gone quiet or vague with nothing specific stated, route to the delay diagnosis instead.
- **Claims vs. Evidence Checker versus List Hygiene Checker:** the claims checker is about whether one tracked status is actually supported by evidence, one item at a time. List Hygiene is about structural problems across a whole list, duplicates, missing fields, staleness, regardless of what any single status field claims. A single suspicious status routes to the claims checker; a whole list that has not been cleaned up routes to list hygiene.
- **Is This Really a Pattern versus Is This Actually a Good Fit:** the pattern checker looks across several different instances over time to find a shared cause. The fit checker looks at several different aspects of one single decision. If you are comparing several complaints, incidents, or pieces of feedback, route to the pattern checker; if you are weighing one decision's pros and cons, route to the fit checker.
- **Brief Your Advocate versus Make the Case:** Brief Your Advocate prepares someone else to present your case on your behalf, live or by forwarding it themselves. Make the Case builds the actual written document, which might be read directly by the decision-maker with nobody presenting it for you. If a specific person has agreed to carry this for you, route to briefing them; if the document itself is what gets sent or read, route to making the case.
- **First Contact That Isn't Generic versus Prep Card Builder:** First Contact drafts the actual first message to someone you have not yet reached, before any conversation exists. Prep Card Builder is for a conversation that is already arranged, or already happening, and needs organising beforehand. If nothing has been sent or scheduled yet, route to first contact; if a conversation is already on the calendar, route to the prep card.
- **None of these fit:** say so plainly rather than forcing the closest match. Suggest raising it as a new idea in a [sibling-projects discussion](https://github.com/shaunmarsden/sibling-projects/discussions) instead of inventing a method on the spot.

## Produce a Clean Handoff

Once a route is chosen, state:

- **The objective**: what the user is actually trying to achieve, in one sentence
- **The recommended tool**: named directly, with a link
- **Why this route fits**: the specific detail that pointed here rather than to a similar-sounding alternative
- **What it will need from you**: what the recommended tool's own gathered inputs require
- **What still requires a person**: carried forward from the recommended tool's own guardrails, not reset to a blank slate

## Apply the Guardrails

- Never solve the underlying task in place of the tool being recommended
- Never force a fit when the described situation does not actually match anything in the table; say so
- Do not assume which tool fits from a single keyword; check the actual situation against the confusions above when two tools sound similar

## Require Human Review

This recommends a route and prepares a handoff. Actually running the recommended tool, and everything it in turn requires a person to check, stays exactly as documented in that tool.

For a fictional worked example, including one that deliberately tests the Post-Mortem Builder versus What's Actually Causing This Delay confusion above, read [the worked example](router-example/).
