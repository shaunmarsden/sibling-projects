# Do These Actually Match?

Compare two separately kept records of the same thing and show only where they really disagree, instead of a full side-by-side or picking whichever source is handier.

It comes from the Conflicting evidence label in the [METHODOLOGY.md](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/METHODOLOGY.md) of [Practical AI Sales Workflows](https://github.com/shaunmarsden/practical-ai-sales-workflows), which the [approval-gated sales copilot guide](https://github.com/shaunmarsden/practical-ai-sales-workflows/blob/main/guides/build-an-approval-gated-sales-copilot.md#label-the-evidence) works through in detail. I took out everything sales-specific and made it a tool of its own for a much more common case: two whole records that should match.

It's for anyone matching up two separately kept records of the same thing, such as a manual count against a system export, one team's spreadsheet against another's, or a membership list against who has paid. They don't want a wall of near-identical rows, or a confident mismatch that turns out to be a unit conversion.

I built it on 22 August 2026. [The repo](https://github.com/shaunmarsden/do-these-actually-match) has a made-up hardware shop's stock count checked against its till export. It tests a unit conversion, a formatting difference, a new delivery and an unfinished count. A second, harder made-up case tests an ID mismatch that can't be confirmed, a duplicated payment row, and a real conflict in status.
