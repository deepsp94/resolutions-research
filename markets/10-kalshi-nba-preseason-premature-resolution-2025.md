# Kalshi: NBA preseason premature resolutions

## Bottom line

**Finding: No failure. Two NBA preseason game-winner markets — `KXNBAGAME-25OCT10BOSTOR` (Boston vs Toronto) and `KXNBAGAME-25OCT10ORLPHI` (Orlando vs Philadelphia) — were reportedly graded early and for the wrong team, then reverted to "to be determined" before settlement, with a Kalshi staffer saying there would be "no losses." No final mispayment or lasting loss is documented; a glitch corrected before settlement is not a practical resolution failure. Confidence: medium, because the entire early-grade → revert → no-loss chain rests on a single contemporaneous report.**

The markets and the real game outcomes are now verified from primary data. Kalshi ran two preseason game-winner markets in series `KXNBAGAME` ("Professional Basketball Game"), settled off NBA.com, with the tickers `KXNBAGAME-25OCT10BOSTOR` and `KXNBAGAME-25OCT10ORLPHI`.[^api][^wayback] The games tipped the night of October 10, 2025 ET, and the actual results were **Toronto 107, Boston 105** and **Orlando 128, Philadelphia 98**, both preseason.[^espn][^nba]

Event Horizon reported that Kalshi resolved both markets before the games ended and initially for the wrong team, that users complained on Discord and the site that bets were graded as losses, that the pages then showed "to be determined" despite final scores being listed, and that a Kalshi staffer said the issue was being reviewed and there would be "no losses."[^event-horizon] No archived market page, API record, second outlet, or user-forum thread independently captures that erroneous-then-reverted state. On the available record this is a **temporary operational glitch corrected before settlement**, not a practical resolution failure.

## Market details

- **Venue:** Kalshi
- **Series:** `KXNBAGAME`, "Professional Basketball Game"; settlement source: the Governing League (NBA.com).[^api][^wayback]
- **Markets:** `KXNBAGAME-25OCT10BOSTOR` ("Boston vs Toronto Winner?") and `KXNBAGAME-25OCT10ORLPHI` ("Orlando vs Philadelphia Winner?").[^wayback]
- **Close condition (from the market page):** "This market will close and expire after a winner is declared"; markets carried `can_close_early: true` and `close_unconfirmed: true`.[^wayback]
- **Games tipped:** night of October 10, 2025 ET (`expected_determination_time` 2025-10-10 22:00 ET).[^wayback]
- **Actual results:** Toronto 107, Boston 105; Orlando 128, Philadelphia 98 — both preseason.[^espn][^nba]
- **Reported issue:** markets graded before game end and for the wrong team.[^event-horizon]
- **Reported correction:** markets moved back to "to be determined"; a Kalshi staffer said users would have no losses.[^event-horizon]

## What happened

Both markets were standard game-winner contracts settled off the NBA. The pre-game state is confirmed by a Wayback snapshot taken October 10, 2025 at 15:35 UTC — before tipoff — which shows both markets `active`, trading live (e.g. Toronto bid/ask 52/53; Boston 46/49), with empty `result` fields and an `expected_determination_time` of 2025-10-10 22:00 ET.[^wayback] That snapshot confirms the tickers, titles, NBA source, and close mechanics, but predates the alleged misgrade.

The actual results were Toronto 107–105 over Boston and Orlando 128–98 over Philadelphia, both preseason.[^espn][^nba]

Event Horizon reported on October 11, 2025 that Kalshi had graded both markets before the games ended and for the wrong team, that users complained on Discord and the site that their bets were incorrectly graded as losses, and that by publication the pages showed "to be determined" despite final scores being listed.[^event-horizon] The same report says a Kalshi staffer on Discord stated the issue was being investigated and there would be "no losses" on the outcomes, and that Kalshi had not returned a request for comment by publication.[^event-horizon]

## The allegation against Kalshi

### 1. The markets resolved before the event was complete

If a game-winner market grades before the game ends, the settlement system has failed the most basic event-completion check. The market's own `close_unconfirmed: true` / `can_close_early: true` flags describe a mechanism by which an early or unconfirmed close could occur.[^wayback] This is materially different from a disputed definition or a source-hierarchy issue.

### 2. The initially displayed winners were wrong

Event Horizon's account says the markets were not only early but graded for the wrong team.[^event-horizon] The real winners were Toronto and Orlando.[^espn][^nba] The report does not specify, in text, which side each market was wrongly graded toward, so the "wrong winner" claim is attributed to the report rather than independently reconstructed.

### 3. Users temporarily saw losses on markets that should not have been final

The alleged harm is temporary but real: users saw bets graded as losses while the markets should still have been unresolved.[^event-horizon] Even with no final loss, premature loss displays can affect trust, displayed balances, and user decisions.

## Kalshi's defense

Kalshi's defense is implicit rather than fully public. The strongest available point is that the erroneous grades were not left in place: Event Horizon reported the outcomes were moved back to "to be determined" and that a staffer said users would have no losses.[^event-horizon]

That supports a limited defense:

- the error was detected quickly;
- the markets were moved out of the wrong final state before settlement;
- users were reportedly told they would not be harmed; and
- no final wrong payout is documented in any source.

The defense does not erase the initial erroneous state. It does change the practical classification: a temporary market-state problem reportedly corrected before final harm.

## Assessment

### Did Kalshi grade the markets early and wrong at first?

**Reportedly yes, on a single source.** Event Horizon directly reports early and wrong grading, with embedded Discord screenshots inside the article.[^event-horizon] No primary artifact independent of that article confirms it: the only archived market snapshot is pre-game, and the markets have since aged out of the live API.[^wayback][^api]

### Did Kalshi later revert the state?

**Reportedly yes — but only per the same single source.** The article says the markets showed "to be determined" after the issue and that a staffer said users would have no losses.[^event-horizon] There is no independent confirmation of the revert or the "no losses" assurance.

### Is a final wrong payout established?

**No.** No source shows users ultimately lost money after Kalshi reviewed the issue.

### Was this a practical resolution failure?

**No, not on the available record.** The account supports a temporary early/wrong market state, but the same account says Kalshi reverted the outcomes and that users would have no losses. Without evidence of final mispayment or lasting loss, this is not a practical resolution failure.

### Overall classification

- **Temporary market-state error:** Reportedly yes (single source)
- **Final mispayment:** Not established
- **Rule ambiguity:** No
- **Corrected by venue before settlement:** Reportedly yes (single source)
- **Best public verdict:** No failure; temporary premature/wrong market state apparently remediated before final harm

## Precise blocker to a stronger finding

The blocker is source depth, and it is precise: the markets, the NBA settlement source, and the real game results (Toronto 107–105, Orlando 128–98) are verified from primary data, but the **entire exonerating chain — early/wrong grade → revert to "to be determined" → staffer "no losses" — rests on one report (Event Horizon, October 11, 2025) with no independent corroboration.** The only archived market page is a pre-game snapshot, the markets have aged out of the live Kalshi API, no second outlet or user-forum thread covers the incident, and the staffer statement survives only inside that article's screenshots. A stronger finding would need a post-game archived/API record showing the erroneous grade and the revert, the final settlement values for both markets, and a direct Kalshi support statement confirming no user losses. (Minor: Event Horizon's "Saturday night" framing is slightly off — the tickers and game logs date the games October 10, 2025, a Friday.)

## Sources

[^event-horizon]: Dustin Gouker, Event Horizon, "Kalshi Resolved Two NBA Preseason Games Early And With The Wrong Winner," October 11, 2025. Sole contemporaneous report; states the two affected markets, premature/wrong grading, the move back to "to be determined," user complaints on Discord and the site, and a Kalshi staffer saying there would be "no losses." Embedded Discord screenshots are the only contemporaneous artifacts and exist only within this article. [Article][event-horizon]

[^api]: Kalshi API, series `KXNBAGAME` ("Professional Basketball Game"), settlement source "the Governing League" (NBA.com). The two October 2025 markets have aged out of the live markets API. [API][api]

[^wayback]: Wayback Machine snapshot of the Kalshi market pages `kxnbagame-25oct10bostor` and `kxnbagame-25oct10orlphi`, captured October 10, 2025 15:35 UTC (before tipoff). Confirms the tickers, titles ("Boston vs Toronto Winner?", "Orlando vs Philadelphia Winner?"), NBA settlement source, close condition ("This market will close and expire after a winner is declared"), and the `can_close_early: true` / `close_unconfirmed: true` flags; shows both markets `active` with live prices and empty `result` fields. Does not capture the post-game erroneous-grade or revert state. [Snapshot][wayback]

[^espn]: ESPN, Celtics vs Raptors game summary, October 10, 2025 (preseason): Toronto 107, Boston 105. [ESPN][espn]

[^nba]: NBA.com / Yahoo Sports box score, Magic vs 76ers, October 10, 2025 (preseason): Orlando 128, Philadelphia 98. [NBA][nba]

[event-horizon]: https://nexteventhorizon.substack.com/p/kalshi-resolved-two-nba-preseason-games-wrong
[api]: https://api.elections.kalshi.com/trade-api/v2/series/KXNBAGAME
[wayback]: https://web.archive.org/web/20251010153517/https://kalshi.com/markets/kxnbagame/professional-basketball-game/kxnbagame-25oct10bostor
[espn]: https://www.espn.com/nba/game/_/gameId/401812697/celtics-raptors
[nba]: https://www.nba.com/game/bos-vs-tor-0012500044
