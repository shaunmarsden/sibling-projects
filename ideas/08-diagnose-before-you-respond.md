# Diagnose Before You Respond

Works out what's really behind an objection or complaint before answering it, rather than arguing with the words on the surface.

It comes from [objection-response](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/.agents/skills/objection-response/SKILL.md) and applies it to negotiations or customer complaints rather than sales objections.

It's for anyone facing pushback where answering the literal words could miss the real concern: a customer complaint, a colleague pushing back on a plan, a negotiation where the stated sticking point may not be the real one.

I built it on 2 August 2026 and kept it light: five files, with one combined worked example rather than separate case, output and review files. To answer the worry below that it was too speculative, I limited it to customer complaints, not pushback in general. [The repo](https://github.com/shaunmarsden/diagnose-before-you-respond) has a made-up bakery example. It tests a simple fault that shouldn't be over-diagnosed, and a complaint whose real cause isn't the one stated.

## Rough Shape

It needs the pushback exactly as said or written, what's known about the person's authority or stake in the outcome, and whether you need a quick live answer or a considered written one.

The method works out the likely real reason before drafting anything. The response deals with that reason, not just the surface words. It ends with an honest next step, including walking away when that's the right call.

It must never invent a reason the evidence doesn't support. Once it has found a deeper reason, it must never argue with the surface words, because that just argues the wrong problem again.

It stops if the evidence is too thin to diagnose anything with confidence, and says so plainly rather than guessing.

## Open Questions

- This is the idea on the list most likely to feel like "generic conflict advice" unless it's aimed at one sharp use. It's worth deciding that use (customer complaints? pushback from colleagues?) before building anything, rather than trying to cover all pushback everywhere.
- Might this work better as a second worked example inside a broader tool rather than its own repo, given how close it sits to ordinary negotiation advice, with no strong general method underneath?
