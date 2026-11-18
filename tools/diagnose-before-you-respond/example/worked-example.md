# Worked Example: Two Complaints, Millbrook Bakery

A made-up small bakery. I tested whether the tool over-diagnoses a simple, real fault, and whether it catches a hidden cause when there is one.

## Case 1: Wrong Cake Flavour

**Complaint:** "I ordered a lemon cake for my daughter's birthday and you sent chocolate. She's allergic to chocolate, we couldn't even use it."

**Diagnosis:** `genuine-fault`. The stated issue is the actual problem, an order mix-up with a real consequence. There is nothing to dig beneath here.

**Reply:** "I'm so sorry, this was our mistake, the wrong cake should never have gone out, especially with an allergy involved. I'd like to send a replacement lemon cake today at no charge, and refund the original order, both need a quick manager sign-off given the amount, which I'm requesting now. Thank you for flagging this straight away."

**Why this is right:** the fault is real and specific. A longer "we hear you" reply, or digging for a deeper cause, would solve a problem that isn't there.

**What a person still needs to check:** the reply says approval is needed "given the amount", but the complaint gives no amount, so that detail is invented. The complaint also describes an allergen mix-up. Someone should find out how the wrong cake went out, as that is a safety issue as well as a service one.

## Case 2: Late Collection Order

**Complaint:** "My order wasn't ready when I arrived, I ended up waiting twenty minutes. Would've been nice to get a heads up instead of just standing there."

**Diagnosis:** `feeling-unheard`. The lateness itself is a real but fairly small issue; the actual driver, based on the wording, is that nobody told them it would be late until they were already standing there waiting. A reply that only addresses "sorry it was late" misses that.

**Reply:** "Sorry about that, and you're right, we should have let you know as soon as we realised it was running behind rather than leaving you to find out by waiting. I'll flag this with the team so orders running late get a heads-up call going forward. Would a small credit toward your next order help make up for the wait? I'd like to apply that, pending a quick check with my manager."

**Why this is right:** a reply of only "sorry it was late" would miss the real complaint. It's about the missing warning, not the twenty minutes.

**What a person still needs to check:** the reply says late orders will get a heads-up call from now on, and implies staff knew the order was running late. The complaint supports neither. Check both with the team before sending.

## What This Tests

Case 1 checks that the tool doesn't over-diagnose a simple, real fault and give a longer reply than it needs. Case 2 checks that it catches a hidden cause that differs from the stated problem, rather than answering only the surface.

The repository doesn't record which model wrote the diagnoses and replies, or whether it knew what the test was checking. Read them as an illustration of what a good run looks like, not as a logged run.
