# Build Your Own AI Output Rubric

**One line:** A tool that walks someone through building a fixed scoring rubric for judging AI output in their own domain, instead of judging it by gut feel every time.

**Generalises from:** [the sales AI output rubric](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/evaluations/sales-ai-output-rubric.md), one level up: not a fixed rubric itself, a method for building one.

**Who it is for:** anyone using AI for repeated output in a domain with its own real stakes, legal drafting, code review, marketing copy, hiring screens, research summaries. Almost nobody defines "good" before they start trusting an AI's answer.

**Status:** Concept only, not built.

## Rough Shape

- **Gather the inputs:** the task the AI is doing repeatedly; two or three examples of a genuinely good output and a genuinely bad one, if the person has them; what a failure would actually cost if it went unnoticed
- **Method:** identify the areas that would each independently make an output good or bad (not just one overall gut score); separate scoring areas from automatic-failure conditions, things that fail the output regardless of how good everything else is; keep the rubric to ten areas or fewer so it stays usable
- **Guardrails:** never let the rubric become so detailed nobody actually fills it in; the automatic-failure list is for genuinely unacceptable outcomes, not just weak ones
- **Stop when unsafe:** the person cannot actually describe what a bad output looks like in their domain, meaning the rubric would just be guessed

## Open Questions

- Should this produce a rubric as a static document, or actually walk someone through scoring a real first output as part of building it, the way the sales rubric's worked example does?
- Is there a generic "automatic failure" starter list worth including (invented facts, invented commitments, missing a stated constraint), or does that have to be fully domain-specific every time?
