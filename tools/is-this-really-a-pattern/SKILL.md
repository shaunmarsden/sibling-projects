---
name: is-this-really-a-pattern
description: Review a log of similar-sounding instances, complaints, feedback, incidents, and separate genuine repeated drivers from similar wording that hides different causes. Use when deciding whether a recurring issue deserves a real fix or process change, or checking whether a supposed pattern is actually supported by the log. Do not use this for judging a single instance on its own; this is for spotting what actually recurs across several.
---

# Is This Really a Pattern?

You do not need to install anything to try this once. The lines between the dashes at the very top are just this file's label; leave them in. On GitHub, copy this using the **Raw** button near the top of the page rather than selecting the rendered text, so the tables and links below paste in cleanly. Send the whole file as your first message in any AI chat tool, then paste in your log.

Find what genuinely recurs across a log without turning a repeated phrase into a made-up root cause. The same words can hide different causes, and different words can describe the same cause.

## Gather the Inputs

A log containing, for each entry: an identifier for which instance it came from, the exact wording used, the diagnosed cause and the evidence for it if known, and the period the log covers.

Keep repeated entries from the same underlying instance as separate occurrences but only one distinct instance. If instance identity is unclear, say so before counting.

## Check the Log Before Finding Patterns

State what is missing, inconsistent, or too vague. A diagnosed cause is evidence only when the log explains how it was established. If the log records wording but not the cause, label the cause unknown rather than inferring it confidently.

## Build Candidate Groups

Group the log twice:

1. By similar wording or topic
2. By the underlying cause recorded in the evidence

Compare the two views. Similar words with different causes are a misleading surface pattern. Different words with the same cause may be a genuine pattern.

Count both occurrences and distinct instances. Do not let two entries from one instance look like two independent examples.

## Judge Each Pattern

For every candidate, show:

- The entries supporting it
- Evidence the cause is the same or different across them
- Evidence against the pattern
- A confidence level specific to that finding: low, medium, or high, explained rather than reduced to a fixed number

Sample size, distinct instances, and consistency of the cause all matter.

## Apply the Guardrails

- Never report a percentage or rate from a small or mixed sample
- Never merge different causes because the wording shares a term
- Never split the same cause merely because people described it differently
- If fewer than two distinct instances support a candidate, call it an isolated signal, not a pattern
- Do not present a fix or process change as already decided

## Stop When the Evidence Is Too Thin

If the cause is unknown across most entries, report the missing diagnosis work instead of inventing patterns. If instance identity cannot be resolved, show a range rather than a false exact count.

## Require Human Review

A person checks the diagnoses, decides whether a finding actually matters, and approves any resulting fix or process change.

For a fictional worked example, read [the worked example](example/). For the harder case, repeat complaints miscounted as separate instances, a log with no diagnosed causes at all, and a percentage request the sample cannot support, read [the second worked example](example-two/). Use [the blank template](templates/pattern-review-template.md) for your own log, and [the review checklist](checks/checklist.md) before acting on any finding.
