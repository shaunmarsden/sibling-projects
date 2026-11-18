# Post-Mortem Builder

<p>
  <img alt="Status: Working tool" src="https://img.shields.io/badge/status-working%20tool-2563eb">
  <a href="LICENSE"><img alt="Licence: MIT" src="https://img.shields.io/badge/licence-MIT-lightgrey"></a>
</p>

Work out whether a failed attempt (a rejected application, a cancelled project, a pitch that went nowhere) is really over or just blocked, and what would justify trying again.

## Why

The reason you're given for a failure isn't always the whole story. "It didn't work out" can mean several different things. It might be a real dealbreaker that won't change, a pause with its own timeline, a thread that just needs a normal follow-up, or a clear no that should stay closed. Treat all four the same and you'll get at least one wrong: you'll chase something that has clearly ended, or write off something that hasn't.

[![A simple tree of possible classifications after an outcome.](assets/diagrams/03-post-mortem-builder.svg)](SKILL.md)

**Not what you need?** This is for something that has already closed, been rejected or gone quiet for good. If the decision is still open and just taking a while, try [What's Actually Causing This Delay?](../whats-causing-this-delay/).

## Use It

Copy [SKILL.md](SKILL.md) and paste it into your AI tool (ChatGPT, Claude, Gemini or similar), then paste in the final message or record and whatever you know about what changed. It classifies the outcome as one of:

- A hard blocker, where a real requirement wasn't met and is unlikely to change
- Timing, where the fit is real but the moment isn't, usually with a stated future trigger
- A contact change, where the person has gone but the case may still work through someone else
- An unresolved concern, where something specific was raised and answered, and still rejected
- A no-decision, where an answer was sent and then contact stopped. That isn't a rejection at all.

[The worked example](example/) has four fictional cases: a rejected job application, a paused grant, a quiet partnership pitch and an unconditional decline. It tests whether the classifications stay distinct. [The second worked example](example-two/) is harder: a stated reason that blends three factors with no clear main one.

<details>
<summary><strong>See what it produces</strong></summary>

1. What was said or shown, kept apart from a tidier story
2. Whether the case itself still stands, checked separately from who was involved
3. A classification (hard blocker, timing, contact change, unresolved concern or no-decision), or a plain "blended, none confirmed as primary" where that's the truth
4. What would justify trying again, or a plain statement that nothing would

</details>

Use [the blank template](templates/post-mortem-template.md) for your own case, and [the review checklist](checks/checklist.md) before you decide whether to try again.

You don't need to install anything, set up a project or write code to try it.

## Before You Use It

This gives you an analysis and a recommendation. You decide whether to try again and whether to send anything. It will never suggest a reason to go back to someone who has given a clear, unconditional no.

## Feedback

Used it on a real case? [Start a discussion](https://github.com/shaunmarsden/sibling-projects/discussions) if a classification didn't fit or a category was missing.

## Part of a Family

This is one of a family of free tools that take patterns from [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows) beyond sales. [sibling-projects](../../README.md) lists the rest. Not sure which one fits? Try [the interactive picker](https://shaunmarsden.github.io/sibling-projects/), which shows clickable cards, or paste a description into an AI chat with [the router](../../ROUTER.md).
