# Kalshi: 49ers vs. Chargers point-total market displayed a school district as the source

## Bottom line

**Finding: Failure (minor). A live Kalshi 49ers vs. Chargers point-total market displayed "San Francisco Unified School District" as the verification source, while the governing CFTC-resolution contract — verified from a dated copy of the terms captured two days before the game — named the league governing the game. Kalshi called it a frontend copy error and corrected the displayed text before the market settled. The source-display field was wrong on a live, tradeable market, which is a real presentation/source-control failure; but the binding rule was never wrong, no payout was affected, and no user harm is demonstrated. Confidence: high.**

Event Horizon reported that the live point-total market for the 49ers vs. Chargers preseason game displayed the San Francisco Unified School District as the source for verifying the outcome.[^eventhorizon] A Kalshi spokesperson called it "a simple copy error" and a "frontend display" issue distinct from the CFTC-filed contract, "which serves as the resolution source with the CFTC and was never incorrect."[^eventhorizon] The governing contract, captured two days before the game, names the league governing the game as the Source Agency — with no "school," "district," "Unified," or "SFUSD" text anywhere.[^terms-dated][^api]

This belongs in the tracker as **Failure (minor)**: the market-facing source field was wrong on a live market, which matters for users reading the live rules, but the available evidence points to a frontend copy error rather than a broken filed rule or final misresolution, and the error was caught and fixed before settlement.

## Market details

- **Venue:** Kalshi
- **Market:** NFL point-total market, series `KXNFLTOTAL` ("Pro Football Total Points," scope "Point Total"), governed by the `NFLTOTAL` contract (document titled "FOOTBALLTOTALS").[^api][^terms-dated]
- **Game:** San Francisco 49ers vs. Los Angeles Chargers, NFL preseason Week 3, **August 23, 2025**, at Levi's Stadium (49ers won 30–23).[^game]
- **Issue:** the live market frontend displayed "San Francisco Unified School District" as the source for verifying the outcome.[^eventhorizon]
- **Filed contract source (dated, governing):** "The Source Agency is the league governing `<game>`," per the `NFLTOTAL` terms captured August 21, 2025 — two days before the game.[^terms-dated]
- **Live settlement source (Kalshi API):** "the Governing League," linked to `https://www.nfl.com/`.[^api]
- **Kalshi response:** a "simple copy error" / "frontend display" issue, "distinct from having an error with the actual contract itself."[^eventhorizon]

## What happened

Event Horizon reported on August 21, 2025 that a Kalshi point-total market for the 49ers vs. Chargers game listed the San Francisco Unified School District as the source for verifying the outcome.[^eventhorizon]

A Kalshi spokesperson told Event Horizon: "When we see frontend display issues like this (importantly, this is distinct from having an error with the actual contract itself, which serves as the resolution source with the CFTC and was never incorrect), we work immediately to update them with the proper text, as we did in this situation," and described it as "a simple copy error."[^eventhorizon] Kalshi updated the displayed source after the issue was flagged.

The game itself was played on August 23, 2025 — two days after the report.[^game] Because the error was observed and corrected before the contract settled, the display problem never reached the settlement stage.

The governing `NFLTOTAL` terms support Kalshi's defense on the binding-rule side. A copy of the terms captured by the Wayback Machine on August 21, 2025 — two days before the game — states: "The Source Agency is the league governing `<game>`." The words "school," "district," "Unified," and "SFUSD" do not appear anywhere in the document.[^terms-dated] The live Kalshi API for the series independently lists the settlement source as "the Governing League," linked to the NFL's official site.[^api]

## The allegation against Kalshi

The allegation is not that the final settlement was wrong. It is that Kalshi displayed a nonsensical verification source on a live market.

That is still important. Prediction-market users rely on displayed rules and source text when pricing contracts. A source field is not decorative; it tells users whose data controls the payout.

## Kalshi's defense

Kalshi's defense is strong but limited.

The defense is that the CFTC-filed contract was correct, the actual source was always the league governing the game, and the school-district text appeared only in the frontend display.[^eventhorizon][^terms-dated][^api]

That means the error did not change the legally controlling settlement rule. It also means the episode is better classified as quality-control/source-display risk than as a final misresolution. The dated terms snapshot is the decisive piece: the governing version in force around the event date named the league, not a school district.

## Assessment

### Did Kalshi display the wrong source?

**Yes.** Event Horizon captured and described the school-district source display, and Kalshi acknowledged and corrected it.[^eventhorizon] This claim rests on a single outlet (Event Horizon); no independent contemporaneous capture was found, which is consistent with a transient frontend bug that was fixed quickly.

### Was the filed contract itself wrong?

**No.** The `NFLTOTAL` terms captured August 21, 2025 — two days before the game — name "the league governing `<game>`" as the Source Agency, with no school-district text anywhere, and the live Kalshi API lists the settlement source as "the Governing League" → nfl.com.[^terms-dated][^api] Kalshi also denied any contract error.[^eventhorizon]

### Was there a demonstrated wrong payout?

**No.** The error was reported on August 21 and corrected before the August 23 game; the market had not settled when the bug was observed.[^eventhorizon][^game] No source reviewed shows an incorrect final settlement or user harm.

### Was this a real failure for the tracker?

**Yes, but only as a minor presentation/source-control failure.** The market-facing source field was wrong on a live, tradeable market, which matters for users reading the live rules, but the evidence points to a frontend copy error rather than a broken filed rule or final misresolution.

### Overall classification

- **Frontend/source-display error:** Yes
- **Filed-rule error:** Not established (governing terms named the league)
- **Final misresolution:** Not established
- **Reported user harm:** Not established
- **Best public verdict:** Failure (minor); no proven settlement error

## Precise blocker to a stronger finding

Two residual limitations, both immaterial to the verdict. First, the display-error claim is single-sourced to Event Horizon; no independent contemporaneous screenshot or report was located. Second, the CFTC product-certification PDF for `NFLTOTAL` returns a 404 (NoSuchKey) at both the standard regulatory URL and the URL the Kalshi API itself advertises, so the certification document could not be retrieved directly. Neither gap changes the finding: the dated August 21, 2025 terms snapshot establishes the governing Source Agency as the league, and the live API corroborates it. The case stays framed as a minor live-market source-display failure, with no settlement record showing the erroneous display affected any payout.

## Sources

[^eventhorizon]: Dustin Gouker, Event Horizon, ["Why Is Kalshi Saying A School District Is The Source For Who Wins A Football Game?"][eventhorizon], August 21, 2025. Documents the erroneous frontend source ("San Francisco Unified School District"), Kalshi's correction, and the spokesperson's statement that it was "a simple copy error" and a "frontend display" issue "distinct from having an error with the actual contract itself, which serves as the resolution source with the CFTC and was never incorrect." Single-source for the display-error claim.

[^terms-dated]: Kalshi, [`NFLTOTAL` contract terms][terms-dated] (document titled "FOOTBALLTOTALS"), as captured by the Wayback Machine on August 21, 2025 — two days before the August 23 game. States: "Source Agency: The Source Agency is the league governing `<game>`." The strings "school," "district," "Unified," and "SFUSD" do not appear anywhere in the document. This is the governing version as of the event date. (Current live copy: [PDF][terms-live].)

[^api]: Kalshi public API, series `KXNFLTOTAL` ("Pro Football Total Points," scope "Point Total"). The `settlement_sources` field lists a single source: `{"name": "the Governing League", "url": "https://www.nfl.com/"}`, corroborating the filed terms. [API][api]

[^game]: San Francisco 49ers vs. Los Angeles Chargers, NFL preseason Week 3, played August 23, 2025 at Levi's Stadium; 49ers won 30–23. Establishes that the August 21 report and Kalshi's correction preceded settlement. [ESPN recap][game]

[eventhorizon]: https://nexteventhorizon.substack.com/p/why-is-kalshi-saying-a-school-district-is-source-for-nfl-markets
[terms-dated]: https://web.archive.org/web/20250821181310/https://kalshi-public-docs.s3.amazonaws.com/contract_terms/NFLTOTAL.pdf
[terms-live]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/NFLTOTAL.pdf
[api]: https://api.elections.kalshi.com/trade-api/v2/series/KXNFLTOTAL
[game]: https://www.espn.com/nfl/recap/_/gameId/401776567
