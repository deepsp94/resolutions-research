# Kalshi: 2025 NFL win-total misgrading

## Bottom line

**Finding: This was a real operational settlement error that Kalshi later corrected. Confidence: high that at least some markets were misgraded; medium on the full scope.**

Kalshi reportedly misgraded multiple 2025 NFL regular-season win-total markets. The clearest public example was a San Francisco 49ers over 10.5 wins position: the 49ers finished the regular season **12-5**, so over 10.5 should have paid Yes.[^event-horizon][^sfchronicle]

Instead, affected users were initially reimbursed only their original position cost rather than receiving the full $1 settlement value for winning contracts. After public criticism, Kalshi reversed course and paid correct Yes holders the difference up to the full contract settlement value.[^event-horizon][^ingame]

This is not a semantic ambiguity or a rules-versus-spirit dispute. It is a straightforward operational failure: the market outcome was mechanically knowable, the initial treatment was wrong, and Kalshi later fixed it.

## Market details

- **Venue:** Kalshi
- **Market type:** 2025 NFL regular-season team win totals
- **Clearest reported example:** San Francisco 49ers over 10.5 wins
- **Real-world result:** 49ers finished the 2025 regular season 12-5.[^sfchronicle]
- **Initial issue:** some winning positions were reportedly reimbursed at cost rather than paid at $1.
- **Final correction:** Kalshi paid affected correct positions the full $1 contract settlement value, net of prior reimbursement.[^event-horizon][^ingame]

I could not recover the specific Kalshi market page or ticker for the 49ers over 10.5 contract from Kalshi's public site. The case is therefore based on contemporaneous industry reporting that reproduced or described Kalshi communications and on external reporting of the 49ers' final record.

## What happened

Event Horizon reported that Kalshi Discord users complained on January 6-7, 2026 about NFL win-total markets being graded incorrectly. The clearest example described was a user who held 49ers over 10.5 wins and did not receive winnings even though San Francisco had won 12 regular-season games.[^event-horizon]

Event Horizon further reported that Kalshi's initial fix was to reimburse the original trade amount but not pay out winnings. The report says Kalshi later emailed affected users explaining that an NFL win-total market had been determined in error and that correct Yes holders at expiration would be credited up to the full $1 settlement value.[^event-horizon]

InGame separately reported that many or most NFL totals markets appeared to have been settled on December 22, before the regular season ended on January 4, and that many markets were therefore settled incorrectly. It reported that by January 7 the issue appeared resolved and quoted a Kalshi spokesperson saying people were paid in full, including winnings.[^ingame]

Event Horizon also reported that Kalshi confirmed on X that people who held winning positions in markets that resolved incorrectly were paid their winnings.[^event-horizon]

## The allegation against Kalshi

### 1. The markets resolved before the relevant season was over

InGame reported that the win-total markets appeared to have been mostly settled on December 22, even though the NFL regular season did not end until January 4 and teams still had games remaining.[^ingame]

If that account is correct, the initial grading process failed before even reaching the final arithmetic.

### 2. Winning users were initially not paid winnings

Event Horizon reported that Kalshi's initial remedy was cost reimbursement rather than full winning settlement. That matters because a correct contract holder is not made whole by receiving only the purchase cost if the contract should have paid $1.[^event-horizon]

### 3. The example was not close

The 49ers over 10.5 example was not a statistical correction or judgment call. San Francisco finished 12-5, which is over 10.5.[^sfchronicle]

This makes the case much cleaner than source-timing or natural-language disputes. Once the regular season ended, the correct settlement direction was obvious.

## Kalshi's defense

Kalshi's own defense is mostly implicit in the correction.

The email reproduced by Event Horizon, and the spokesperson statement reported by InGame, indicate that Kalshi treated the issue as an erroneous determination and credited affected correct positions to the full settlement value.[^event-horizon][^ingame]

That is an important distinction. Kalshi did not defend the initial grading as a valid interpretation of the rule. It corrected the outcome.

The strongest defense is therefore limited but real:

- operational errors can occur on exchanges and sportsbooks;
- Kalshi eventually identified the erroneous determinations;
- affected correct holders were reportedly paid the full $1 contract value; and
- the public record does not show that Kalshi intentionally refused payment after the correction.

The defense does not erase the failure. The failure includes both the initial misgrading and the apparent initial decision to treat cost reimbursement as final.

## Assessment

### Did Kalshi initially resolve at least some NFL win-total markets incorrectly?

**Yes, on the available reporting.**

Event Horizon and InGame both report incorrect NFL win-total grading. Event Horizon cites Kalshi's later email to affected users saying a market had been determined in error, and InGame quotes a Kalshi spokesperson confirming full payment after the issue.[^event-horizon][^ingame]

### Was the 49ers over 10.5 example objectively a winning Yes?

**Yes.**

The 49ers finished 12-5, which is over 10.5 wins.[^sfchronicle]

### Did Kalshi eventually correct the mistake?

**Yes, according to the available reporting.**

Affected correct holders were reportedly credited the difference between their initial reimbursement and the full $1 payout.[^event-horizon][^ingame]

### Was this a real failure for the tracker?

**Yes.**

This is one of the clearest operational failures in the seed list. It does not depend on fuzzy words, legal interpretation, or oracle governance. It was a settlement execution problem in markets whose facts were easy to verify.

### Overall classification

- **Operational settlement error:** Yes
- **Rule ambiguity:** No
- **Corrected by venue:** Yes
- **Scope fully known:** No
- **Best public verdict:** Real misgrading, later remediated

## Precise blocker to a stronger finding

The unresolved issue is scope. The public record identifies the 49ers over 10.5 market as the clearest example and says more than one NFL win-total market was affected, but it does not establish the full list of misgraded markets, the number of affected users, total dollars initially withheld, or total remediation cost.

## Sources

[^event-horizon]: Dustin Gouker, Event Horizon, ["Why Wasn't Kalshi Paying Traders That Won NFL Futures Bets?"][event-horizon], January 8, 2026. Reports Discord complaints, the 49ers over 10.5 example, initial cost reimbursement, Kalshi's corrective email, and Kalshi's later confirmation that winners were paid.

[^ingame]: Jeff Edelstein, InGame, ["The Prediction Market That Couldn't Count Straight"][ingame], January 7, 2026. Reports premature NFL win-total settlement, user complaints, later full payment, and a Kalshi spokesperson's confirmation.

[^sfchronicle]: San Francisco Chronicle, ["49ers net favorable 2026 schedule with third-place finish in NFC West"][sfchronicle], January 4, 2026. Reports that the 49ers finished the 2025 regular season 12-5.

[event-horizon]: https://nexteventhorizon.substack.com/p/why-wasnt-kalshi-paying-traders-that-won-nfl-futures
[ingame]: https://www.ingame.com/the-prediction-market-that-couldnt-count-straight/
[sfchronicle]: https://www.sfchronicle.com/sports/49ers/article/49ers-net-favorable-2026-schedule-third-place-21276434.php
