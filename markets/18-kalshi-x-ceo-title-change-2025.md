# Kalshi: Linda Yaccarino leaves or is replaced as X CEO in 2025

## Bottom line

**Finding: This was a real market-title/rules mismatch and live-title-change problem. Confidence: high.**

Kalshi initially displayed a market title saying "Linda Yaccarino leaves X this year?" After Yaccarino announced she was leaving X, Yes traded up near 99% and Kalshi itself posted about the market. But the detailed rules did not simply ask whether she left; they required that X have, or announce it would have, a new CEO by the specified date.[^eventhorizon][^terms]

Kalshi later changed the displayed title to "Linda Yaccarino replaced as X CEO in 2025?" or substantially similar replacement language.[^kalshi][^eventhorizon]

This belongs in the tracker even if no final wrong payout is shown. The problem was that the visible market title communicated one trigger, the binding rule used a different trigger, and the venue changed the live title only after substantial trading.

## Market details

- **Venue:** Kalshi
- **Original title reported by Event Horizon:** `Linda Yaccarino leaves X this year?`
- **Later/current title:** `Linda Yaccarino replaced as X CEO in 2025?`
- **Contract series:** `XCEOCHANGE`
- **Underlying/source agency:** releases from X and reporting from Bloomberg.
- **Payout criterion in contract terms:** X has, or will have, a new CEO by the specified date.
- **Key allegation:** title said "leaves"; rules required "new CEO"/replacement.[^eventhorizon][^terms][^kalshi]

## What happened

Event Horizon reported that Yaccarino announced she was leaving X on a Wednesday morning and that the news was widely reported. It also reported that Kalshi posted about her leaving while showing the market graph near 99% Yes.[^eventhorizon]

But Event Horizon pointed out that the displayed market title did not match the detailed rule. The title asked whether Yaccarino would leave, while the rule required an announcement that X would have a new CEO by December 31, 2025.[^eventhorizon]

The public contract terms support the rule-side reading. The `XCEOCHANGE` terms state that the payout criterion is whether X has, or will have, a new CEO by the relevant date, and that it is enough for an announcement to say the move will occur even if the change officially happens later.[^terms]

Event Horizon then reported that Kalshi changed the market title to replacement language and that Yes fell from near 99% to much lower levels after users read the rules or saw the clarification.[^eventhorizon]

## The allegation against Kalshi

### 1. The original title communicated the wrong trigger

"Linda Yaccarino leaves X this year?" is naturally satisfied by Yaccarino announcing her departure. It does not require a successor to be named.

The contract terms, however, required a new CEO condition.[^terms] That is a materially different event.

### 2. Kalshi's own social post amplified the title-level reading

Event Horizon reported that Kalshi tweeted in a way that made it seem like Yaccarino had left and showed the market at 99%.[^eventhorizon]

That matters because many users price the visible title and platform presentation, not only the contract PDF.

### 3. The live title change came after trading

Event Horizon reported that Kalshi changed the market name on Wednesday night, after the departure announcement and after the market had traded heavily around the title-level interpretation.[^eventhorizon]

Changing a live title to match the rule may reduce future confusion, but it also confirms that the prior title was materially misleading.

## Kalshi's defense

The strongest defense is that the filed/binding contract terms controlled from the beginning.

Those terms say the underlying is X releases and Bloomberg reporting, and the payout criterion is whether X has or will have a new CEO by the date.[^terms] Event Horizon also acknowledged that the new title better captured the intent of the market based on the rules.[^eventhorizon]

Under that defense, Kalshi did not change the contract. It corrected a front-end/title problem so users would better understand the already-existing rule.

## Assessment

### Did Yaccarino leaving satisfy the original visible title?

**Yes, in ordinary language.**

Event Horizon reported that she tweeted she was leaving and that the fact was widely reported.[^eventhorizon]

### Did Yaccarino leaving necessarily satisfy the detailed rule?

**No.**

The detailed terms required X to have, or announce it would have, a new CEO by the specified date.[^terms]

### Did Kalshi change the live title?

**Yes, according to Event Horizon, and the current Kalshi page uses replacement language.**[^eventhorizon][^kalshi]

### Was there a demonstrated final wrong payout?

**Not established.**

The documented failure is presentation and rule clarity, not an already-proven final settlement error.

### Was this a real failure for the tracker?

**Yes.**

A prediction market's visible title is economically important. Here, the title and rules diverged on the central trigger, and the title was changed only after market-moving news.

### Overall classification

- **Operational settlement error:** Not established
- **Title/rules mismatch:** Yes
- **Live clarification/title change:** Yes
- **Binding-rule defense:** Strong
- **Best public verdict:** Real presentation/rules failure; no proven final misresolution

## Precise blocker to a stronger finding

The missing evidence is the final settlement outcome and a complete archived record of every title/rule version as displayed to users at each moment. The available evidence is enough to establish a title/rules mismatch and live-title correction, but not enough to prove final settlement harm.

## Sources

[^eventhorizon]: Dustin Gouker, Event Horizon, ["Kalshi Changed The Title Of A Market About X's CEO, And It Seems Like A Problem"][eventhorizon], July 10, 2025. Documents the original title, Yaccarino announcement, title change, rule mismatch, price movement, and reported Kalshi employee response.

[^terms]: Kalshi, [`XCEOCHANGE` contract terms][terms]. States the source agency and payout criterion requiring that X has, or will have, a new CEO by the specified date.

[^kalshi]: Kalshi, ["Linda Yaccarino replaced as X CEO in 2025?"][kalshi]. Current market page title using replacement language.

[eventhorizon]: https://nexteventhorizon.substack.com/p/kalshi-changed-the-title-of-a-market
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/XCEOCHANGE.pdf
[kalshi]: https://kalshi.com/markets/kxxceochange/linda-yaccarino-leaves-x
