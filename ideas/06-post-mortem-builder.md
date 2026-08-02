# Post-Mortem Builder

**One line:** Works out whether a failed initiative is genuinely over or just blocked, and what would actually justify revisiting it, applied to any failed effort, not just a lost sale.

**Generalises from:** [review-lost-opportunity](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/review-lost-opportunity/SKILL.md), the loss-classification logic (a genuine disqualification vs. a pause vs. something that could still be revived) applied beyond a sales deal.

**Who it is for:** anyone doing a post-mortem on a failed pitch, a rejected job application, a cancelled project, a grant application that did not land, where "why did this actually fail" tends to get answered emotionally rather than by checking what was actually said.

**Status:** Concept only, not built.

## Rough Shape

- **Gather the inputs:** whatever record exists of the failure, the actual stated reason if one was given, anything known about what changed on the other side; a clear separation between what was said and what is being assumed about why
- **Method:** classify what actually happened (a stated reason, an inferred reason, no reason given at all); check whether the underlying problem is likely to still exist; state plainly what, if anything, would justify trying again, versus treating it as genuinely closed
- **Guardrails:** never invent a reason where the evidence only supports an unknown; do not let this become a tool for justifying re-approaching someone who has clearly and explicitly said no
- **Stop when unsafe:** there is no actual record of what was said or why, only a feeling that it did not work out, in which case there is nothing to classify

## Open Questions

- Does the classification set from the sales version (disqualification, timing, budget, wrong contact, and so on) travel to other domains, or does each domain (hiring, funding, project cancellation) need its own failure taxonomy?
- Worth a worked example per domain, or one generic example plus a note on adapting the categories?
