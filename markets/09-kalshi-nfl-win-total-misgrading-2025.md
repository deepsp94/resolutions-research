# Kalshi: 2025 NFL win-total misgrading

## Bottom line

**Finding: Failure, resolved. Kalshi settled NFL regular-season win-total markets on December 22, 2025 — before the regular season ended on January 4, 2026, with games still to be played — and graded them incorrectly, paying objective winners as losers. The governing `WINTOTAL` contract sets expiration "one week after the end of the regular season" and permits earlier expiration only when the outcome can no longer change, so the premature settlement was a direct contract violation. Kalshi initially reimbursed only original trade cost rather than the full $1, then corrected the error and paid correct Yes holders in full, including winnings. Confidence: high on the failure-and-remediation sequence; medium on full scope.**

The clearest public example is a San Francisco 49ers over 10.5 wins position. The 49ers finished the 2025 regular season **12-5**, so over 10.5 was an objective Yes, but the holder was initially not paid winnings.[^event-horizon][^pfr] This is not a semantic ambiguity or a rules-versus-spirit dispute: the markets were settled before the season ended, the outcome was mechanically knowable once it did, the initial treatment was wrong, and Kalshi later fixed it.

The decisive contract fact is timing. The binding terms set the latest expiration at "one week after the end of the regular season" and allow early expiration **only** when "an event described in the Payout Criterion occurs (or can no longer occur)" — i.e., when the result is already mathematically locked.[^terms] On December 22, 2025, with Week 18 still to play (the 49ers' regular-season finale against Seattle fell on January 4, 2026), most win totals were not locked.[^ingame][^nfl-week18] Settling them then violated the written rule.

## Market details

- **Venue:** Kalshi
- **Series / ticker:** `KXNFLWINS`, "Pro Football Wins" (Win Totals), rulebook `WINTOTAL`.[^api]
- **Market type:** 2025 NFL regular-season team win totals.
- **Governing contract:** the `WINTOTAL` terms, CFTC-certified **May 14, 2025** and initially listed May 15, 2025 — the version in force for the 2025 season.[^cert]
- **Underlying:** "the number of regular season game wins by `<team>` in the `<year>` season"; postseason and exhibition games excluded.[^terms]
- **Expiration timing (governing rule):** "The latest Expiration Date of the Contract shall be one week after the end of the regular season for `<team>`," with earlier expiration only when an outcome "occurs (or can no longer occur)" under Rule 7.2.[^terms]
- **Settlement sources:** the Governing League (NFL) and ESPN.[^api]
- **Settlement Value:** $1.00.[^terms]
- **Clearest reported example:** San Francisco 49ers over 10.5 wins; the 49ers finished 12-5.[^pfr]

## What happened

InGame reported that NFL win-total markets appeared to have been settled on **December 22, 2025**, even though the regular season did not end until **January 4, 2026** and teams still had games remaining, with "many — if not most NFL totals markets" settled incorrectly.[^ingame] The independent record confirms the timing: the 2025 NFL regular season concluded with Week 18 on January 4, 2026, and the 49ers played their regular-season finale against Seattle that day.[^nfl-week18]

Event Horizon reported that Kalshi Discord users complained on January 6-7, 2026 about NFL win-total markets being graded incorrectly. The clearest example was a holder of 49ers over 10.5 wins who did not receive winnings even though San Francisco won 12 regular-season games. Event Horizon also reported that the grade was inverted — "the people who technically lost these bets/trades were paid out as winners."[^event-horizon] The 49ers' 12-5 finish is independently verified.[^pfr]

Event Horizon reported that Kalshi's initial fix was to refund the original trade amount without paying winnings. Kalshi later emailed affected users, in language reproduced by Event Horizon: "You are receiving this email because you have traded on a NFL Win total market that was determined in error. Upon review, we have decided that users who held correct 'Yes' positions at the time of Expiration shall be paid out their full contract settlement value of $1."[^event-horizon]

After the issue went viral on X (more than one million views), Kalshi reversed course in the early hours of January 7 and paid winners in full. Kalshi confirmed on X that "all people who had winning positions that resolved incorrectly got paid their winnings."[^event-horizon] A Kalshi spokesperson told InGame: "It was quickly resolved, people were paid out in full, including winnings."[^ingame]

## The allegation against Kalshi

### 1. The markets resolved before the season was over

The win-total markets appeared to have been settled December 22, 2025, even though the NFL regular season did not end until January 4, 2026 and teams still had games remaining.[^ingame][^nfl-week18] The governing contract sets the latest expiration at "one week after the end of the regular season" and permits early expiration only when the outcome can no longer change.[^terms] On December 22 most totals — including the 49ers' — were not yet locked, so the early settlement broke the written rule before any arithmetic was even at issue.

### 2. The grade was wrong, and winners were initially not paid winnings

Event Horizon reported that the grade was inverted (losers paid as winners) and that Kalshi's initial remedy was cost reimbursement rather than full winning settlement.[^event-horizon] A correct contract holder is not made whole by receiving only the purchase cost when the contract should have paid $1.

### 3. The example was not close

The 49ers over 10.5 example was not a statistical correction or judgment call. San Francisco finished 12-5, which is over 10.5.[^pfr] Once the regular season ended, the correct settlement direction was obvious.

## Kalshi's defense

Kalshi's defense is mostly implicit in the correction. The email reproduced by Event Horizon and the spokesperson statement reported by InGame both treat the issue as an erroneous determination and credit affected correct positions to the full $1 settlement value.[^event-horizon][^ingame] Kalshi did not defend the initial grading as a valid interpretation of the rule; it corrected the outcome.

The strongest defense is therefore limited but real:

- operational errors can occur on exchanges and sportsbooks;
- Kalshi identified the erroneous determinations within roughly one to two days;
- affected correct holders were paid the full $1 contract value, net of prior reimbursement; and
- the public record does not show that Kalshi intentionally refused payment after the correction.

The defense does not erase the failure. The failure includes the premature settlement, the inverted grading, and the initial decision to treat cost reimbursement as final.

## Assessment

### Did the markets settle before the governing contract allowed?

**Yes.** The contract sets the latest expiration at "one week after the end of the regular season" and allows earlier expiration only when the outcome "occurs (or can no longer occur)" under Rule 7.2.[^terms] The December 22, 2025 settlement preceded the January 4, 2026 season end with games still to play, and the 49ers' total was not mathematically locked, so the early settlement was a contract violation.[^ingame][^nfl-week18]

### Was the 49ers over 10.5 example objectively a winning Yes?

**Yes.** The 49ers finished 12-5, which is over 10.5 wins.[^pfr]

### Did Kalshi eventually correct the mistake?

**Yes.** Affected correct holders were credited the difference between their initial reimbursement and the full $1 payout; Kalshi confirmed on X and to InGame that winners were paid in full, including winnings.[^event-horizon][^ingame]

### Was this a real failure for the tracker?

**Yes.** This is one of the clearest operational failures in the seed list. It does not depend on fuzzy words, legal interpretation, or oracle governance. It was a premature settlement and grading-execution problem in markets whose facts were easy to verify.

### Overall classification

- **Premature settlement against the written rule:** Yes
- **Operational settlement / grading error:** Yes
- **Rule ambiguity:** No
- **Corrected by venue:** Yes
- **Winners ultimately made whole:** Yes (resolved)
- **Scope fully known:** No
- **Best public verdict:** Real misgrading, later remediated

## Precise blocker to a stronger finding

The unresolved issue is scope. The public record identifies the 49ers over 10.5 market as the clearest example and indicates that many or most NFL win-total markets were affected, but Kalshi never published the full list of misgraded markets, the number of affected users, the total dollars initially withheld, or the total remediation cost. The governing contract, the premature-settlement timing, the inverted grade, the initial cost-only reimbursement, and the final full payment are all verified; only the precise scope numbers remain unpublished.

## Sources

[^api]: Kalshi public API, series endpoint for `KXNFLWINS`. Confirms series ticker `KXNFLWINS`, rulebook `WINTOTAL`, scope "Win Totals," settlement sources the Governing League (NFL) and ESPN, and links to the contract terms and product certification. [API][api]

[^terms]: Kalshi, `WINTOTAL` contract terms (binding rules). Underlying is "the number of regular season game wins by `<team>` in the `<year>` season"; "The latest Expiration Date of the Contract shall be one week after the end of the regular season for `<team>`," with earlier expiration only when an outcome "occurs (or can no longer occur)" under Rule 7.2; Settlement Value $1.00; "Revisions to the Underlying made after Expiration will not be accounted for." [PDF][terms]

[^cert]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification, "Will `<team>` have `<above/below/between/exactly/at least>` `<count>` wins in the `<year>` season?" Contract, dated May 14, 2025, initially listed May 15, 2025 — the governing version for the 2025 season. [Cert][cert]

[^event-horizon]: Dustin Gouker, Event Horizon, "Why Wasn't Kalshi Paying Traders That Won NFL Futures Bets?", January 8, 2026. Reports Discord complaints, the 49ers over 10.5 example, the inverted grade (losers paid as winners), initial cost-only reimbursement, Kalshi's corrective email ("determined in error… full contract settlement value of $1"), and Kalshi's X confirmation that winners were paid. [Event Horizon][event-horizon]

[^ingame]: Jeff Edelstein, InGame, "The Prediction Market That Couldn't Count Straight," January 7, 2026. Reports settlement on December 22, 2025 before the January 4, 2026 season end, that many or most NFL totals markets were settled incorrectly, that winners were initially reimbursed cost without winnings, and a Kalshi spokesperson's confirmation: "It was quickly resolved, people were paid out in full, including winnings." [InGame][ingame]

[^pfr]: Pro-Football-Reference, 2025 San Francisco 49ers season. Reports that the 49ers finished the 2025 regular season 12-5, second in the NFC West. [PFR][pfr]

[^nfl-week18]: 2025 NFL season, Week 18 schedule. The regular season concluded with Week 18 on January 4, 2026; the San Francisco 49ers played their regular-season finale against the Seattle Seahawks that day. [Wikipedia][nfl-week18]

[api]: https://api.elections.kalshi.com/trade-api/v2/series/KXNFLWINS
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/NFLWINS.pdf
[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/NFLWINS.pdf
[event-horizon]: https://nexteventhorizon.substack.com/p/why-wasnt-kalshi-paying-traders-that-won-nfl-futures
[ingame]: https://www.ingame.com/the-prediction-market-that-couldnt-count-straight/
[pfr]: https://www.pro-football-reference.com/teams/sfo/2025.htm
[nfl-week18]: https://en.wikipedia.org/wiki/2025_NFL_season
