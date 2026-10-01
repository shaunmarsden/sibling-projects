# Build Your Own AI Output Rubric

A tool that walks you through building a fixed rubric for scoring AI output in your own field, so you stop judging it by gut feel each time.

It goes one level up from [the sales AI output rubric](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/evaluations/sales-ai-output-rubric.md). It isn't a rubric itself; it's a way to build one.

It's for anyone using AI for repeated work in a field with real stakes: legal drafting, code review, marketing copy, hiring screens, research summaries. Almost nobody decides what "good" means before they start trusting an AI's answer.

I built it on 2 August 2026. [The repo](https://github.com/shaunmarsden/build-your-own-rubric) has a made-up worked example on customer support replies for Thornbury Outfitters. It builds a rubric, then applies it to a new output that fails in a subtler way than the bad example the rubric came from, to check the rubric still holds.

## Rough Shape

It needs the task the AI does over and over, two or three examples of a good output and a bad one if you have them, and what a failure would cost if nobody noticed it.

The method finds the areas that could each make an output good or bad on their own, rather than one overall gut score. It keeps scoring areas apart from automatic failures, which fail the output however good the rest is. It keeps the rubric to ten areas or fewer so people will use it.

It must never let the rubric get so detailed that nobody fills it in. The automatic-failure list is for outcomes that are unacceptable, not just weak.

It stops if you can't describe what a bad output looks like in your field, because then the rubric would be a guess.

## Open Questions

- Should this produce a rubric as a fixed document, or walk you through scoring a real first output while you build it, as the sales rubric's worked example does?
- Is there a general "automatic failure" starter list worth including (made-up facts, made-up commitments, a missed constraint), or does it have to be specific to each field every time?
