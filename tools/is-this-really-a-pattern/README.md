# Is This Really a Pattern?

<p>
  <img alt="Status: Illustrative examples" src="https://img.shields.io/badge/status-illustrative%20examples-2563eb">
  <a href="LICENSE"><img alt="Licence: MIT" src="https://img.shields.io/badge/licence-MIT-lightgrey"></a>
</p>

Compare similar-sounding complaints, feedback or incidents with the causes recorded in your log. See where the evidence supports a repeated cause and where it does not.

## Why

The same word can hide two different problems, and two different descriptions can hide the same one. Issue logs often get this wrong both ways. They merge things that only sound alike, and they miss a real pattern because people described it differently each time.

[![A two by two grid showing when repeated wording is a genuine pattern and when it is misleading.](assets/diagrams/02-is-this-really-a-pattern.svg)](SKILL.md)

**Not what you need?** This looks for evidence of a repeated cause across entries in one log. If you have two records, kept separately, that should each show the same thing, try [Do These Actually Match?](https://github.com/shaunmarsden/sibling-projects/tree/main/tools/do-these-actually-match/).

## Use It

Copy [SKILL.md](SKILL.md) and paste it into any AI chat, then paste in a log you are allowed to share. The instructions ask for:

- Genuine patterns, where different wording hides the same diagnosed cause across at least two distinct instances
- Misleading surface patterns, where similar wording hides different causes, named so a fix doesn't go to the wrong place
- Isolated signals, which are real but have only one instance so far
- A confidence level for each finding, never a percentage from a sample too small to support one

<details>
<summary><strong>See what it produces</strong></summary>

1. Genuine patterns, with the same diagnosed cause across at least two distinct instances
2. Misleading surface patterns, named so a fix isn't aimed at the wrong cause
3. Isolated signals kept apart from confirmed patterns, with the cause marked unknown where the log doesn't establish one
4. A confidence level for each finding, never a percentage from a sample too small to support one

</details>

[The worked example](example/) is a fictional team's feedback over four sprints. The shared word "communication" hides two different issues, and two differently worded complaints have the same recorded cause. [The second worked example](example-two/) has repeat complaints from one customer, no recorded diagnoses and a request for a percentage.

Both are illustrations, not logged model tests. The model, run instructions and settings are not recorded. The [first review](example/review.md) and [second review](example-two/review.md) explain the outputs' limits, including unsupported claims and the difference between a count within a log and a wider rate. There is no measured accuracy or tool-by-tool compatibility evidence here.

Use [the blank template](templates/pattern-review-template.md) for your own log, and [the review checklist](checks/checklist.md) before you act on any finding.

You don't need to install anything, set up a project or write code to try it.

## Before You Use It

This reviews the log; it doesn't decide anything. Whether a finding is worth acting on, and any fix or process change that follows, is your call.

The AI cannot verify the causes outside the material you supply. Check its groupings and counts against the original entries. Remove private details the review does not need, and use only material approved for your chosen AI tool.

## Repository Checks

Pull requests and changes to main run offline checks for relative links, heading anchors, Markdown punctuation and SVG XML. These do not test AI behaviour or external websites. With Python 3.11 or newer, run these from this folder (`tools/is-this-really-a-pattern`):

```sh
python3 -m unittest discover -s checks -p 'test_*.py' -v
python3 checks/check_repository.py
```

The checker reads Git-tracked files, so stage new documentation first. It supports the inline Markdown and HTML link forms used here, not every possible Markdown syntax. Frozen test packet hashes are checked too; that checks file integrity, not model quality.

The [rule comparisons](evaluations/pattern-comparison-2026-11-17/README.md) tested the percentage rule and pattern template separately in 24 isolated Codex trials. Neither candidate met the frozen adoption rule, so the live skill, template and historical examples are unchanged. The review is non-blind and does not establish general reliability.

## Feedback

Used it on a real log? [Start a discussion](https://github.com/shaunmarsden/sibling-projects/discussions) if a grouping didn't fit.

## Part of a Family

This is one of a family of free tools that take patterns from [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows) beyond sales. [sibling-projects](https://github.com/shaunmarsden/sibling-projects) lists the rest. Not sure which one fits? Try [the interactive picker](https://shaunmarsden.github.io/sibling-projects/), which shows clickable cards, or paste a description into an AI chat with [the router](https://github.com/shaunmarsden/sibling-projects/blob/main/ROUTER.md).
