# Diagnose Before You Respond

**One line:** Works out what is actually driving a stated objection or complaint before answering it, rather than arguing with the surface wording.

**Generalises from:** [objection-response](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/objection-response/SKILL.md), applied to negotiation or customer complaints rather than a sales objection specifically.

**Who it is for:** anyone facing pushback where answering the literal words risks missing the real concern underneath them, a customer complaint, an internal stakeholder pushing back on a plan, a negotiation where the stated sticking point may not be the real one.

**Status:** Built, 2 August 2026, kept lightweight (5 files, one combined worked example rather than separate case/output/review files). Scoped tightly to resolve the speculative-ness flagged below: customer complaints specifically, not pushback in general. Live at [github.com/shaunmarsden/diagnose-before-you-respond](https://github.com/shaunmarsden/diagnose-before-you-respond), with a fictional bakery worked example testing both a genuine simple fault (should not be over-diagnosed) and a complaint whose real driver is not the stated issue.

## Rough Shape

- **Gather the inputs:** the pushback exactly as it was said or written; what is known about the person's actual authority or stake in the outcome; whether a fast, live answer or a considered written one is needed
- **Method:** diagnose the likely real driver before drafting anything; produce a response that addresses the diagnosed driver, not just the surface wording; end with an honest next step, including walking away where that is genuinely the right call
- **Guardrails:** never invent a driver the evidence does not actually support; never argue with the surface wording once a deeper driver has been diagnosed, that just relitigates the wrong problem
- **Stop when unsafe:** the evidence is too thin to diagnose anything with real confidence, in which case say that plainly rather than guessing at a driver

## Open Questions

- This is the one idea on the list most likely to feel like "generic conflict advice" unless it is scoped to one sharp use case. Worth deciding that use case (customer complaints specifically? internal stakeholder pushback specifically?) before building anything, rather than trying to cover all pushback everywhere
- Might this actually be better as a second worked example inside a broader tool rather than its own repo, given how close it sits to ordinary negotiation advice without a strong generalisable method underneath it?
