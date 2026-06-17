# Kalshi: Government shutdown duration and alleged timezone cutoff issue

## Bottom line

**Finding: This is an unverified Reddit-only allegation. Confidence: low.**

The seed allegation says Kalshi changed or applied a UTC cutoff rather than an Eastern Time cutoff for a government-shutdown duration market, producing a different result from Polymarket. The only located evidence is a single Reddit comment inside an unrelated complaint thread.[^reddit]

That is not enough to establish that the market existed as described, that the rule changed, or that Kalshi resolved it incorrectly.

## Market details

- **Venue:** Kalshi
- **Market described by Reddit commenter:** "Will govt shut down be over before 43 days?"
- **Alleged issue:** UTC vs Eastern Time cutoff.
- **Evidence level:** one Reddit comment, no archived contract or market page.[^reddit]

## What happened

In a Reddit thread about a different Kalshi settlement delay, one commenter asserted that Kalshi had changed rules mid-market for a `43y` government-shutdown market by using UTC rather than ET. The commenter also claimed Polymarket treated the shutdown as ending before 43 days while Kalshi did not.[^reddit]

The comment does not link the market, reproduce the terms, identify the final determination, or show before/after rule text.

## The allegation against Kalshi

If true, the allegation would be serious: changing a time convention after trading can flip a duration market. Shutdown-duration contracts are especially sensitive to precise cutoff times.

## Kalshi's defense

No direct Kalshi defense was located.

The strongest implicit defense is evidentiary: without the original terms, the claim may reflect a misunderstanding of a UTC convention that was already in the contract.

## Assessment

### Is there a concrete market?

**Not sufficiently.** The comment gives a rough market description but no ticker or URL.[^reddit]

### Is there evidence Kalshi changed the rule?

**No.** The comment asserts it but provides no archived before/after record.

### Was there a demonstrated wrong payout?

**No.**

### Was this a real failure for the tracker?

**Only as a blocker note.** Timezone errors are a known failure mode, but this specific seed is not proven.

### Overall classification

- **Timezone/cutoff allegation:** Yes
- **Evidence quality:** Very weak
- **Rule change proved:** No
- **Final misresolution proved:** No
- **Best public verdict:** Blocker pending exact contract and archived rule text

## Precise blocker to a stronger finding

The missing evidence is the market URL/ticker, original and final contract terms, expiration convention, shutdown start/end timestamps, and final Kalshi determination. Without those, the allegation should not be used as evidence of a Kalshi mistake.

## Sources

[^reddit]: Reddit, r/Kalshi, ["Kalshi is scamming right now"][reddit], comment alleging a UTC/ET issue in a 43-day government-shutdown market.

[reddit]: https://www.reddit.com/r/Kalshi/comments/1pmvnnc/kalshi_is_scamming_right_now/
