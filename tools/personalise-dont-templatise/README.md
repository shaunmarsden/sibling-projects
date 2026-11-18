# Personalise, Don't Templatise

<p>
  <img alt="Status: Working tool" src="https://img.shields.io/badge/status-working%20tool-2563eb">
  <a href="LICENSE"><img alt="Licence: MIT" src="https://img.shields.io/badge/licence-MIT-lightgrey"></a>
</p>

Fill in a fixed message template with real detail. It handles one recipient, several recipients on the same message, or a recipient who needs to forward part of it to someone who wasn't there.

## Why

A template you send again and again goes wrong in three predictable ways. The opening line is generic and would read the same for anyone. With two recipients, one gets addressed directly and the other is quietly pushed into the third person. Or a section meant for forwarding is written as if the person it's for were reading the email. This handles all three and leaves the template itself untouched.

[![Three routes for personalising a fixed template based on recipients.](assets/diagrams/14-personalise-dont-templatise.svg)](SKILL.md)

**Not what you need?** This personalises a template you already have, for recipients you know. If this is a cold first message to someone you don't know yet, try [First Contact That Isn't Generic](../first-contact-that-isnt-generic/).

## Use It

Copy [SKILL.md](SKILL.md) and paste it into your AI tool (ChatGPT, Claude, Gemini or similar), then paste in the real detail and say how many people it's going to. It produces a message that:

- Personalises the opening line and resource reference with something specific, never generic
- Keeps the template structure exactly as it is, with no reordering or rewriting
- Addresses every recipient directly when there's more than one, never pushing a second person into the third person
- Keeps any block meant for forwarding clearly separate, written in the third person about the recipient and the resource

<details>
<summary><strong>See what it produces</strong></summary>

1. A personalised opening line and resource reference, specific to this recipient
2. The fixed template structure, untouched
3. Every recipient addressed directly, or a clearly separate third-person block for someone it's being forwarded to
4. A stop and a question, instead of a guess, whenever it's unclear who the recipients are or a resource isn't ready

</details>

[The worked example](example/) is a fictional photography workshop's follow-up template. It goes to one recipient, to two recipients together, and to one recipient who needs to forward part of it to someone who wasn't at the session. [The second worked example](example-two/) covers harder cases: a recipient situation that's unclear, and a request to send a placeholder link before the resource exists.

Use [the blank template](templates/message-template.md) for your own case, and [the review checklist](checks/checklist.md) before you send.

You don't need to install anything, set up a project or write code to try it.

## Before You Use It

This drafts the message. It only gets sent if a person approves it.

## Feedback

Used it for a real template? [Start a discussion](https://github.com/shaunmarsden/sibling-projects/discussions) if something didn't fit.

## Part of a Family

This is one of a family of free tools that take patterns from [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows) beyond sales. [sibling-projects](../../README.md) lists the rest. Not sure which one fits? Try [the interactive picker](https://shaunmarsden.github.io/sibling-projects/), which shows clickable cards, or paste a description into an AI chat with [the router](../../ROUTER.md).
