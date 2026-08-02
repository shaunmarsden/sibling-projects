# Skill Author

**One line:** A tool that takes someone's repeated task and produces a proper `SKILL.md`, with real guardrails, stop conditions and a human-review section, instead of the one-off prompt most people write.

**Generalises from:** the actual authoring discipline behind every skill in [practical-ai-sales-workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows), see [what-is-a-sales-ai-skill.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/what-is-a-sales-ai-skill.md) and [progressive-disclosure.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/progressive-disclosure.md), pulled out as a domain-agnostic method rather than sales-specific content.

**Who it is for:** anyone who has a prompt they reuse and retype variations of constantly, and would benefit from turning it into a proper reusable, bounded instruction set instead. Probably the widest possible audience of the whole list, since this is a step up from prompting itself, not from any one domain.

**Status:** Built, 2 August 2026. Live at [github.com/shaunmarsden/skill-author](https://github.com/shaunmarsden/skill-author). The worked example produces an actual, complete generated skill (support-ticket triage) from a plain-English task description, then self-tests it against fictional tickets with deliberate tone-versus-urgency traps in both directions.

## Rough Shape

- **Gather the inputs:** the repeated task in the person's own words; what a good result looks like; what the AI must never do or decide on its own for this task
- **Method:** turn the task description into the standard shape: gather inputs, method steps, guardrails, stop-when-unsafe conditions, what still needs a human. Push a worked example into a separate file rather than inline, per the progressive disclosure pattern, once the core file is doing its job
- **Guardrails:** never produce a skill with no stop conditions or no human-review section; a skill that cannot say when it should refuse to run is not finished
- **Stop when unsafe:** the task described is something that should never be handed to an AI unsupervised at all (an irreversible action, a legal or medical decision), in which case say so rather than dressing it up as a bounded skill

## Open Questions

- Should the output be platform-agnostic markdown (works pasted into anything) or should it also generate the platform-specific wrapper files (Claude skill folder structure, a Custom GPT's instructions field, and so on)?
- Is there a self-test step worth building in, the way [progressive-disclosure.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/progressive-disclosure.md)'s audit checks a skill's line count and structure, applied to a freshly generated skill before calling it done?
