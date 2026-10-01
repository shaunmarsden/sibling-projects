# Skill Author

A tool that takes a task you repeat and turns it into a proper `SKILL.md`, with real guardrails, stop conditions and a section on what a person must review, instead of the one-off prompt most people write.

It takes the method behind every skill in [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows) and makes it work for any field, not just sales. See [what-is-a-sales-ai-skill.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/what-is-a-sales-ai-skill.md) and [progressive-disclosure.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/progressive-disclosure.md).

It's for anyone with a prompt they keep reusing and retyping, who'd do better turning it into a proper, reusable set of instructions with clear limits. It probably has the widest audience on the list, since it's a step up from prompting itself, not from any one field.

I built it on 2 August 2026. In [the repo](https://github.com/shaunmarsden/skill-author), the worked example builds a complete skill (support-ticket triage) from a plain description of the task. It then tests that skill on made-up tickets with deliberate traps where tone and urgency point different ways, in both directions.

## Rough Shape

It needs the repeated task in your own words, what a good result looks like, and what the AI must never do or decide alone for this task.

The method turns the task description into the standard shape: inputs, method steps, guardrails, when to stop, and what still needs a person. Once the core file works, it moves any worked example into a separate file, following the progressive disclosure pattern.

It must never produce a skill with no stop conditions or no human-review section. A skill that can't say when to refuse to run isn't finished.

It stops if the task should never go to an AI unsupervised at all (an action you can't undo, a legal or medical decision). It says so rather than dressing the task up as a skill with limits.

## Open Questions

- Should the output be plain markdown that works pasted into anything, or should it also build the files each platform needs (a Claude skill folder, a Custom GPT's instructions field and so on)?
- Is a self-test step worth building in, like the audit in [progressive-disclosure.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/progressive-disclosure.md) that checks a skill's line count and structure, run on a new skill before calling it done?
