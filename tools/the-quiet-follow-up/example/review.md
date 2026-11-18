# Review: Three Cases Output

I checked [output.md](output.md) against what I built [cases.md](cases.md) to test.

## What Worked

- **It told plain silence apart from an unanswered question.** Case A and Case B could both look like "they haven't replied," but Alicia asked a specific question that nobody answered. The output chose to answer it first, rather than sending a generic nudge on top of an ignored question. That's the mistake this skill exists to catch.
- **It respected the clear no.** Alaric gave a clear, specific reason. The output didn't draft a soft "just checking if you've reconsidered" message, which would have ignored a direct answer. It produced no message at all for this case.
- **It showed the weak message and didn't use it.** Case A's output includes the generic "just following up" version to show what not to send, next to the stronger version that names the real shift and time. Seeing the two side by side shows the difference rather than just claiming it.

## What Still Needs a Human Check

- Case B's reply says there's parking on site and that the number 12 bus stops outside. The case gives neither fact. A real reply needs the true answer, because Alicia is planning her morning around it.
- Case A's shift time and date are made up. In real use, the message would need a detail that's actually correct, not one that only looks specific.
- Whether "two weeks" is long enough to justify a follow-up depends on context the skill doesn't have. A fast-moving event needs a shorter wait than an ongoing role.

## Verdict

No automatic failure. The three cases needed three different responses, and the output gave three different responses rather than treating "nobody's replied" as one situation.
