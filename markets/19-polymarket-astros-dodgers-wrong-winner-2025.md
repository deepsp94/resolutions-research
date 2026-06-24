# Polymarket: Astros vs. Dodgers resolved to the losing team

## Bottom line

**Finding: Failure (resolved). Polymarket's market on the July 4, 2025 Astros–Dodgers game resolved to the Dodgers even though the Astros won 18-1. The misresolution is now confirmed from primary data: the Polymarket gamma API reports outcomePrices `["0", "1"]` for `["Astros", "Dodgers"]` on slug `mlb-hou-lad-2025-07-04`, with `automaticallyResolved: true` and $217,946 in volume.[^gamma] The cause was the UMA optimistic-oracle path: a proposer submitted "Dodgers" and the proposal went undisputed through the challenge window, auto-resolving the market wrong.[^tylerd] Polymarket reportedly made affected holders whole through an off-oracle refund (affected shares redeemable for $1), but the verbatim official statement was not retrieved. Confidence: high on the misresolution; medium-high on the remediation.**

The Astros beat the Dodgers 18-1 at Dodger Stadium on July 4, 2025 — confirmed independently of any prediction-market commentary by the ESPN box score.[^espn] This is not a semantic edge case: the market was supposed to pay the team that won the game, and on the binding oracle record it paid the team that lost by 17 runs.

The remediation record is corroborated but remains secondary. Contemporaneous observers reported a refund was announced "immediately," and the PolymarketGuide archive describes Astros vs. Dodgers as a rare wrong-resolution case where affected shares were made redeemable for $1, with notice via an on-site banner and a statement on X/Discord.[^tylerd][^refunds] The official Polymarket statement itself could not be retrieved, and gamma still reflects the Dodgers outcome — so the fix was an off-oracle economic refund, not an on-chain re-resolution.

## Market details

- **Venue:** Polymarket
- **Market:** "Astros vs. Dodgers," slug `mlb-hou-lad-2025-07-04` (gamma event 30680, market 559108, conditionId `0xa6a39b8770e8ded99a9c410e3054e96275f55b529d0be38278fde7ff2cdf42d3`).[^gamma]
- **Real-world game:** Houston Astros at Los Angeles Dodgers, July 4, 2025, 9:10 PM ET.[^gamma]
- **Resolution source:** MLB.com; resolved via the UMA adapter (`resolvedBy 0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74`).[^gamma]
- **Outcomes / outcomePrices (gamma):** `["Astros", "Dodgers"]` → `["0", "1"]` — i.e. resolved to **Dodgers**.[^gamma]
- **State:** `closed: true`, `closedTime: 2025-07-05 05:56:24Z`, `automaticallyResolved: true`, `umaResolutionStatus: resolved`, `umaResolutionStatuses: ["proposed"]`, volume $217,946.22.[^gamma]
- **Actual result:** Astros 18, Dodgers 1.[^espn]
- **Reported remediation:** affected shares made redeemable for $1 (off-oracle refund).[^tylerd][^refunds]

## What happened

On July 4, 2025, the Astros routed the Dodgers 18-1 at Dodger Stadium; ESPN records the final and describes Jose Altuve homering twice and driving in five.[^espn] The Polymarket market for that game (`mlb-hou-lad-2025-07-04`) nevertheless resolved to the Dodgers: gamma reports outcomePrices `["0", "1"]` against outcomes `["Astros", "Dodgers"]`, closed at 2025-07-05 05:56:24Z, with `automaticallyResolved: true`.[^gamma]

The mechanism was the UMA optimistic oracle, not a hand-keyed Polymarket decision. A proposer submitted "Dodgers" as the outcome, and that proposal was not disputed during the challenge window, so it auto-finalized against the real-world result.[^tylerd] The market's $217,946 volume matches the loss figure cited by contemporaneous observers and by the PolymarketGuide archive.[^gamma][^refunds]

A neighboring market — `mlb-hou-lad-2025-07-05`, the *July 5* game — resolved correctly to the Astros (gamma outcomePrices `["1", "0"]`).[^gamma2] Only the July 4 market misresolved. (An earlier version of this case incorrectly attributed the misresolution to the `-07-05` slug.)

## The allegation against Polymarket

The allegation is straightforward: the market paid the wrong side in a completed baseball game. Unlike cases turning on "suit," "invasion," "approved," or "withdraw," there was no difficult language boundary. The market was supposed to pay the team that won. The Astros won by 17 runs, and the oracle resolved to the Dodgers.[^gamma][^espn]

## Cause, and a debunked framing

The initial public framing — "UMA whale manipulation" — was retracted by the same observer who first posted it. TylerD first attributed the result to whale manipulation, then corrected: "it appears this was not the result of UMA whales and occurred due to bots proposing that the Dodgers won and that result not being disputed."[^tylerd] A separate observation that a trader ("ElGigaWhale") bought ~65,000 Dodgers shares cheaply (0.1¢–4.2¢) describes opportunistic trading on a near-certain loser, not the cause of the resolution.[^tylerd] The verified cause is an undisputed UMA proposal — an oracle-path failure.

## Polymarket's response

The strongest mitigation is remediation. Contemporaneous observers reported "Refund was announced immediately," and the PolymarketGuide archive describes Astros vs. Dodgers as a rare wrong-resolution case handled by making affected shares redeemable for $1, with users notified via a banner and a statement on X/Discord.[^tylerd][^refunds] That does not erase the initial failure, but it reframes it as an operational/oracle-path mistake the venue corrected economically rather than a defended interpretation of ambiguous rules.

Two caveats keep this at medium-high confidence. First, the verbatim official Polymarket statement could not be retrieved; the refund is corroborated by third-party reporting and the PolymarketGuide archive, not by the primary statement text. Second, gamma still shows the Dodgers outcome, so the remedy was an off-oracle refund, not an on-chain re-resolution.

## Assessment

### Was the real-world outcome ambiguous?

**No.** The Astros won 18-1.[^espn]

### Was there a documented wrong resolution?

**Yes, from primary data.** The gamma API reports the market resolved to the Dodgers (outcomePrices `["0", "1"]`), `automaticallyResolved`, on the July 4 slug.[^gamma]

### What caused it?

**An undisputed UMA proposal.** A "Dodgers" outcome was proposed to the optimistic oracle and went unchallenged through the dispute window, auto-finalizing wrong. The "whale manipulation" framing was retracted by its own source.[^tylerd]

### Did Polymarket remedy the harm?

**Reportedly yes, off-oracle.** Affected shares were made redeemable for $1, per contemporaneous reports and the PolymarketGuide archive; gamma still reflects the Dodgers outcome, so this was a refund rather than a re-resolution.[^tylerd][^refunds]

### Was this a real failure for the tracker?

**Yes.** An objective sports market resolved to the team that lost by 17 runs.

### Overall classification

- **Operational settlement error:** Yes (undisputed UMA proposal)
- **Semantic ambiguity:** No
- **Reported remediation:** Yes — off-oracle $1 refund (secondary-sourced)
- **Best public verdict:** Failure (resolved): real misresolution, later economically remedied

## Precise blocker to a stronger finding

The misresolution and the game result are both verified from primary sources (gamma and the ESPN box score). The remaining gap is the verbatim official Polymarket refund statement and a per-wallet refund accounting; both are reported by secondary sources but were not retrieved directly. That is enough to classify the case as **Failure (resolved)** with high confidence on the failure and medium-high on the remediation, but not enough to reconstruct the refund independently.

## Sources

[^gamma]: Polymarket gamma API, `events?slug=mlb-hou-lad-2025-07-04`. Event 30680, market 559108, conditionId `0xa6a39b8770e8ded99a9c410e3054e96275f55b529d0be38278fde7ff2cdf42d3`. Outcomes `["Astros", "Dodgers"]`, outcomePrices `["0", "1"]` (resolved to Dodgers); `closed: true`, `closedTime 2025-07-05 05:56:24Z`, `automaticallyResolved: true`, `umaResolutionStatus: resolved`, `umaResolutionStatuses: ["proposed"]`, `resolvedBy 0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74`, volume 217,946.223426. [gamma][gamma]

[^gamma2]: Polymarket gamma API, `events?slug=mlb-hou-lad-2025-07-05` (the July 5 game). Outcomes `["Astros", "Dodgers"]`, outcomePrices `["1", "0"]` — resolved correctly to Astros. Confirms only the July 4 market misresolved. [gamma2][gamma2]

[^espn]: ESPN MLB scoreboard, July 4, 2025. Houston Astros defeated the Los Angeles Dodgers 18-1 at Dodger Stadium; Jose Altuve homered twice with five RBI. Primary game result, independent of prediction-market commentary. [ESPN][espn]

[^tylerd]: TylerD (@Tyler_Did_It), X thread, July 5, 2025. Original post: "$217k bet on the Astros vs Dodgers market / Astros win 18-1 / Market resolves to Dodgers." Self-correction in-thread: "it appears this was not the result of UMA whales and occurred due to bots proposing that the Dodgers won and that result not being disputed." Notes ElGigaWhale bought ~65,000 Dodgers shares at 0.1¢–4.2¢; a reply states "Refund was announced immediately." Contemporaneous primary account of the cause; remediation claim is observer-reported. [Thread][tylerd]

[^refunds]: PolymarketGuide Archive, "Refunds." Describes Astros vs. Dodgers as a rare wrong-resolution case (market resolved to Dodgers though the Astros won) handled by allowing affected shares to be redeemed for $1, with user notice via a banner and a statement on X/Discord. Secondary source. [Refunds][refunds]

[gamma]: https://gamma-api.polymarket.com/events?slug=mlb-hou-lad-2025-07-04
[gamma2]: https://gamma-api.polymarket.com/events?slug=mlb-hou-lad-2025-07-05
[espn]: https://www.espn.com/mlb/scoreboard/_/date/20250704
[tylerd]: https://x.com/Tyler_Did_It/status/1941581909835870389
[refunds]: https://polymarketguide.gitbook.io/polymarketguide-archive/precedents/polymarket/refunds
