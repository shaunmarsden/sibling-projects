# Weekly Roundup Builder

<p>
  <img alt="Status: Working tool" src="https://img.shields.io/badge/status-working%20tool-2563eb">
  <a href="LICENSE"><img alt="Licence: MIT" src="https://img.shields.io/badge/licence-MIT-lightgrey"></a>
</p>

Pull this week's data and findings into one accurate report, without inventing a trend when there's no earlier report to compare against.

## Why

A weekly report is easy to get quietly wrong in two ways. It can claim movement from a single snapshot with nothing to compare it to. Or it can treat a section with no data as a confirmed zero. This builds the report from what exists, marks what's missing as missing, and only claims a trend once there's a real earlier report to compare with.

[![Checks that prevent a weekly report confusing missing data with zero or a snapshot with a trend.](assets/diagrams/15-weekly-roundup-builder.svg)](SKILL.md)

## Use It

Copy [SKILL.md](SKILL.md) and paste it into your AI tool (ChatGPT, Claude, Gemini or similar). Then paste in whatever you have for this period. It produces a report that:

- **Uses existing findings** rather than redoing analysis already done elsewhere
- **Never claims a trend** without a real earlier report to compare against
- **Separates missing from zero**, both ways round
- **Names specific priorities** from this period's data, not generic advice

<details>
<summary><strong>See exactly what it produces</strong></summary>

1. Each section built from what exists, with missing sections marked missing, not zero
2. A trend claim only where a real earlier report supports one
3. Specific priorities from this period's data, not generic advice
4. A refusal of any request to estimate a missing figure, rather than quietly filling it in

</details>

See [the worked example](example/): a made-up freelance designer's first weekly roundup. [The second worked example](example-two/) is harder: the same designer's next week.

Use [the blank template](templates/roundup-template.md) for your own roundup, and [the review checklist](checks/checklist.md) before you act on anything it suggests.

No installation, project or coding needed to try it once.

## Before You Use It

This writes a report. It doesn't act on anything in it. Approving and acting on any suggested priority is your decision.

## Feedback

Used it for a real weekly roundup? [Start a discussion](https://github.com/shaunmarsden/sibling-projects/discussions) if something didn't fit.

## Part of a Family

This is one of a family of free tools that take patterns from [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows) beyond sales. See [sibling-projects](../../README.md) for the rest. Not sure which one fits? Try [the interactive picker](https://shaunmarsden.github.io/sibling-projects/) to click through the cards, or [the router](../../ROUTER.md) if you'd rather paste a description into an AI chat.
