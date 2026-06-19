# Kalshi: 49ers vs. Chargers market listed San Francisco Unified School District as source

## Bottom line

**Finding: This was a real but minor frontend/source-display error, not a demonstrated final resolution error. Confidence: high.**

Kalshi displayed the San Francisco Unified School District as the source for verifying a 49ers vs. Chargers football market. Event Horizon captured the issue and quoted Kalshi saying it was a frontend copy error, not an error in the CFTC-filed contract.[^eventhorizon]

This belongs in the tracker as **Failure (minor)**: a live market displayed a nonsensical source, but available reporting does not show user losses, a wrong final payout, or any practical repercussion beyond the frontend correction.

## Market details

- **Venue:** Kalshi
- **Market type:** NFL point-total market.
- **Game:** San Francisco 49ers vs. Los Angeles Chargers.
- **Issue:** frontend displayed "San Francisco Unified School District" as the outcome source.
- **Filed contract source:** the league governing the game, according to the `NFLTOTAL` contract terms.[^terms]
- **Kalshi response:** the source display was a simple copy/frontend error and the actual contract was never incorrect.[^eventhorizon]

## What happened

Event Horizon reported that a Kalshi point-total market for the 49ers vs. Chargers game listed the San Francisco Unified School District as the source for verifying the outcome.[^eventhorizon]

Kalshi updated the displayed source to the NFL after the issue was flagged. A Kalshi spokesperson told Event Horizon that the problem was a frontend display issue, distinct from the actual contract filed with the CFTC, and called it a simple copy error.[^eventhorizon]

The linked `NFLTOTAL` terms support Kalshi's defense on the binding-rule side. They state that the Source Agency is the league governing the game.[^terms]

## The allegation against Kalshi

The allegation is not that the final settlement was wrong. It is that Kalshi displayed a nonsensical verification source on a live market.

That is still important. Prediction-market users rely on displayed rules and source text when pricing contracts. A source field is not decorative; it tells users whose data controls the payout.

## Kalshi's defense

Kalshi's defense is strong but limited.

The defense is that the CFTC-filed contract was correct, the actual source was always the relevant league, and the school-district text appeared only in the frontend display.[^eventhorizon][^terms]

That means the error likely did not change the legally controlling settlement rule. It also means the episode is better classified as quality-control/source-display risk than as a final misresolution.

## Assessment

### Did Kalshi display the wrong source?

**Yes.** Event Horizon captured and described the school-district source display.[^eventhorizon]

### Was the filed contract itself wrong?

**Not on the available evidence.** Kalshi denied that, and the linked terms say the source agency is the league governing the game.[^eventhorizon][^terms]

### Was there a demonstrated wrong payout?

**No.** No source reviewed shows an incorrect final settlement.

### Was this a real failure for the tracker?

**Yes, but only as a minor presentation/source-control failure.** The market-facing source field was wrong, which matters for users reading the live market, but the available evidence points to a frontend copy error rather than a broken filed rule or final misresolution.

### Overall classification

- **Frontend/source-display error:** Yes
- **Filed-rule error:** Not established
- **Final misresolution:** Not established
- **Reported user harm:** Not established
- **Best public verdict:** Failure (minor); no proven settlement error

## Precise blocker to a stronger finding

The missing evidence is a final settlement record showing that the erroneous displayed source affected payout or caused user losses. Without that, the case should stay framed as a minor live-market source-display failure.

## Sources

[^eventhorizon]: Dustin Gouker, Event Horizon, ["Why Is Kalshi Saying A School District Is The Source For Who Wins A Football Game?"][eventhorizon], August 21, 2025. Documents the erroneous frontend source, Kalshi's correction, and Kalshi's statement that the filed contract was correct.

[^terms]: Kalshi, [`NFLTOTAL` contract terms][terms]. States that the source agency is the league governing the game.

[eventhorizon]: https://nexteventhorizon.substack.com/p/why-is-kalshi-saying-a-school-district-is-source-for-nfl-markets
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/NFLTOTAL.pdf
