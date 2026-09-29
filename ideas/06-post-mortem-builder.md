# Post-Mortem Builder

Works out whether a failed effort is really over or just blocked, and what would justify trying again. It works for any failed effort, not just a lost sale.

It takes the way [review-lost-opportunity](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/review-lost-opportunity/SKILL.md) sorts a loss (a real disqualification, a pause, or something that could still be revived) and applies it beyond a sales deal.

It's for anyone looking back on a failed pitch, a rejected job application, a cancelled project or a grant bid that didn't succeed. The question "why did this actually fail" tends to get an emotional answer, not one based on what people said.

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/post-mortem-builder) has four made-up cases: a rejected job application, a paused grant, a partnership pitch that went quiet, and a flat decline. They test whether it can tell a hard blocker, a timing problem, no decision and a case closed for good apart.

## Rough Shape

It needs whatever record exists of the failure, the reason given if there was one, and anything known about what changed on the other side. It keeps what was said apart from what's being assumed about why.

The method sorts what happened: a stated reason, an inferred reason, or no reason at all. It checks whether the underlying problem probably still exists. It says plainly what, if anything, would justify trying again, or whether to treat it as closed.

It must never invent a reason where the evidence only supports an unknown. It must not become a way to justify going back to someone who has clearly said no.

It stops if there's no record of what was said or why, only a feeling it didn't work out, because then there's nothing to sort.

## Open Questions

- Do the sales version's categories (disqualification, timing, budget, wrong contact and so on) work in other fields, or does each field (hiring, funding, cancelled projects) need its own list of reasons for failure?
- Is it worth a worked example for each field, or one general example plus a note on adapting the categories?
