# Kalshi: UFC 327 Padilla vs. Mederos corrected draw

## Bottom line

**Finding: No failure. Kalshi's binding contract resolves on "the first official final result," and at UFC 327 the first official result announced was a Christopher Padilla majority-decision win, so Kalshi paid Padilla contracts and nothing on Mederos. That gives the settlement genuine textual cover. But the honest case is narrower than Kalshi's stated defense: the result was corrected to a majority draw the same night, hours *before* the contract's own next-day 10:00 AM ET expiration — so this was not the "post-expiration revision" Kalshi's reporting invoked. The settlement is defensible under the first-official-result clause, while sitting in real tension with the contract's own Expiration Value, its 50/50 draw clause, and the permanent official result (a draw). Confidence: medium (on the normative call).**

Kalshi listed a market on the UFC 327 prelim between Christopher Padilla and MarQuel Mederos, governed by the `KXUFCFIGHT` / ACHIEVEMENTS contract.[^api][^terms] Padilla was initially announced the winner by majority decision, and Kalshi settled immediately on that first announcement, paying Padilla contracts.[^polypunter][^predictionnews] The scorecards were corrected the same night — within roughly an hour, after the next bout — to a majority draw, and the draw is now the permanent official result.[^mmaf-draw][^mmaf-denied]

The decisive question is *which clause governed*. The prior version of this file rested on a "revisions after Expiration will not be considered" defense.[^predictionnews] That defense is factually wrong on this timeline: the correction came the same night, before the contract's next-day 10:00 AM ET expiration, so the draw was not a post-expiration revision. The clause that actually carries the No-failure finding is the **Payout Criterion**, which keys settlement to "the **first** official final result" of the event — Padilla, as first announced.[^terms] Under that clause, settling on the initial Padilla win is a defensible application of the rule, even though the contract's other mechanics point the other way.

## Market details

- **Venue:** Kalshi
- **Market:** "UFC 327: Padilla vs Mederos" — event `KXUFCFIGHT-26APR11PADMED`, market `KXUFCFIGHT-26APR11PADMED-PAD` ("Padilla wins"), under series `KXUFCFIGHT` ("UFC Fight").[^api]
- **Question:** whether Christopher Padilla would win the Padilla vs. Mederos professional MMA fight at UFC 327, Kaseya Center, Miami, April 11, 2026.[^api][^mmaf-results]
- **Binding source:** Source Agencies are the governing association, the Associated Press, ESPN, The Wall Street Journal, and Fox Sports.[^terms]
- **Governing rule (Apr 2026):** Payout Criterion resolves on "the first official final result"; draws/no-contests resolve 50/50; Expiration Value is the value documented at the next-day 10:00 AM ET expiration; post-expiration revisions are excluded.[^terms][^api]
- **First official result announced:** Padilla, majority decision.[^mmaf-results][^polypunter]
- **Corrected and permanent official result:** majority draw (same-night correction; Florida commission denied Padilla's protest April 23, 2026).[^mmaf-draw][^mmaf-denied]
- **Kalshi settlement:** Padilla = Yes; Mederos = No.[^predictionnews][^polypunter]

## What happened

Padilla and Mederos fought three rounds on the early prelims. The referee deducted a point from Mederos in round three for an eye poke. The judges' scores were read and the announcer declared Padilla the winner by majority decision (29-27, 29-27, 28-28).[^mmaf-results][^polypunter]

| Time (ET, Apr 11–23, 2026) | Event |
|---|---|
| Fight ends | Padilla announced winner by majority decision; Kalshi settles on the first announcement[^polypunter] |
| ~An hour later, after the next bout | Officials find all three judges missed the round-3 point deduction; result corrected to **majority draw**, announced on the live broadcast[^mmaf-draw][^polypunter] |
| April 12 | Padilla files a formal protest with the Florida commission[^mmaf-protest] |
| April 23 | Florida commission **denies** the protest; majority draw stands as the permanent official result[^mmaf-denied] |

PolyPunter's account is explicit on the order of events: "UFC announced the update during the live broadcast, but Kalshi had already settled its market."[^polypunter] So Kalshi settled intraday on the first announcement, ahead of its own contractual expiration, and did not revisit the payout after the same-night correction.

## The allegation against Kalshi

The official final result is a draw, yet Kalshi paid a Padilla win.[^mmaf-draw][^predictionnews] The contract itself says a draw resolves 50/50.[^terms] The correction was announced the same night, hours before the contract's stated 10:00 AM ET next-day expiration, so it cannot fairly be called a post-expiration revision. Traders therefore argue the draw — not the retracted Padilla win — is what the contract's own Expiration Value and draw clause should have produced.[^predictionnews][^polypunter] Anyone checking the final result after the night of April 11 would see a draw, not a Padilla win.

## Kalshi's defense

Kalshi's reporting-era defense leaned on the revision-exclusion clause: "any revisions after Expiration will not be considered."[^predictionnews] On this timeline that defense does not hold — the correction preceded expiration.

The defense that does hold is narrower and rests on the **Payout Criterion** itself. The binding rule resolves on "the Expiration Values that it is reported that the **first** official final result of `<achievement>` event is `<participant>`."[^terms] The word "first" is load-bearing: it directs settlement to the result as first officially reported, which was the Padilla majority decision. Read that way, Kalshi settled on exactly the value the Payout Criterion names, and its consistency with the 2025 Oscars viewership market — where Kalshi settled on the initially reported figure and ignored later upward revisions — reflects a deliberate initial-result design choice rather than an ad hoc call.[^predictionnews]

## Assessment

### Was Padilla initially announced as the winner?

**Yes.** Padilla was announced the winner by majority decision before the correction.[^mmaf-results][^polypunter]

### Was the result corrected to a draw, and is the draw permanent?

**Yes.** The correction to a majority draw was announced the same night, and the Florida commission denied Padilla's protest on April 23, 2026, leaving the draw as the official record.[^mmaf-draw][^mmaf-denied]

### Did the correction occur before the contract's expiration?

**Yes — and this is the key factual correction to the prior file.** The correction was announced the same night, within roughly an hour.[^mmaf-draw][^polypunter] The contract's Expiration time is 10:00 AM ET, on the day after the official final result.[^terms] The draw therefore arrived hours before expiration, so the "revisions after Expiration will not be considered" clause does not apply to it. Kalshi's stated defense was built on the wrong clause.

### Does any clause still support the Padilla settlement?

**Yes — the Payout Criterion's "first official final result."** The binding rule keys resolution to the result as first officially reported, which was Padilla's majority decision.[^terms] That clause gives the settlement genuine textual cover independent of the (inapplicable) revision-exclusion clause.

### Is there a real internal inconsistency?

**Yes — and it is the genuine weakness here.** The same contract also provides that the Expiration Value is "the value of the Underlying as documented by the Source Agency on the Expiration Date at the Expiration time" (next-day 10:00 AM ET), and that draws resolve 50/50.[^terms] At the 10:00 AM ET expiration, the value documented by the Source Agencies (ESPN, WSJ, Fox Sports) was a draw, which the draw clause would settle 50/50. So the Payout Criterion ("first official final result" → Padilla) collides with the Expiration Value and draw clauses (→ draw, 50/50). The contract points in two directions on this fact pattern, and Kalshi chose the first-result direction.

### So was this a resolution failure?

**No — it was a defensible application of the operative clause, not a misresolution.** The "first official final result" language is express contract text that names the Padilla outcome, and Kalshi settled on it consistently with its initial-result design philosophy. A resolution failure would require Kalshi to have ignored or contradicted its binding rule; instead it applied one express clause over another in a contract that is internally inconsistent here. The failure, if any, is in the drafting — not in the settlement deviating from the rule as Kalshi reads it.

### Is there a fair criticism of Kalshi?

**Yes, but it is a design criticism, not a failure.** A contract that can pay a retracted result, while its own Expiration Value and 50/50 draw clause point to the corrected outcome, is poorly designed for same-event corrections — especially where the official result is permanently a draw. Resolving sports markets on an initial announcement creates a clean administrative cutoff but can mislead anyone who expects settlement to track the final, corrected result.[^predictionnews] That is a legitimate critique of the rule, but applying an express clause as drafted is not a rule violation.

### Overall classification

- **Settlement consistent with an express binding clause ("first official final result"):** Yes
- **Misapplication of the rules:** No
- **Reliance on the post-expiration-revision defense:** Rejected — correction preceded expiration
- **Internal contract inconsistency (Payout Criterion vs. Expiration Value vs. draw clause):** Yes
- **Weak contract design for same-event corrections:** Yes
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

To convert this into a resolution failure, one would need to show that the "first official final result" clause does not govern — for example, that the Expiration Value clause is the controlling term and overrides the Payout Criterion, or that Kalshi applied a rule other than the one in the certified contract. The contract is internally inconsistent rather than one-directional, and the Payout Criterion's express "first official final result" language gives Kalshi a defensible textual basis, which keeps this at No failure. The residual uncertainty is purely interpretive — which of two conflicting clauses controls — and is reflected in the medium confidence on the normative call. The per-market settlement object is no longer retained in Kalshi's public API, but the Padilla=Yes outcome is independently documented by two contemporaneous reports.[^predictionnews][^polypunter]

## Sources

[^api]: Kalshi API, series `KXUFCFIGHT` and event `KXUFCFIGHT-26APR11PADMED`. Title "UFC 327: Padilla vs Mederos"; sub_title "Padilla vs Mederos"; settlement sources The Wall Street Journal, ESPN, Fox Sports; series `important_info` (UFC-RULES4) stating draws/no-contests resolve 50/50 and that revisions after Expiration will not be considered. [Series][api-series] · [Event][api-event]

[^terms]: Kalshi, `UFC` contract terms (ACHIEVEMENTS rulebook), binding rules in force on the event date. Payout Criterion: "...the Expiration Values that it is reported that the **first** official final result of `<achievement>` event is `<participant>`." Expiration Date: "the day after the day the achievement event has an official final result." Expiration time: "10:00 AM ET." Expiration Value: "the value of the Underlying as documented by the Source Agency on the Expiration Date at the Expiration time." Revision clause: "any revisions after Expiration will not be considered... if... the official result of `<achievement>` is reversed or changed in any way after the Contract expires, that will not impact the market's resolution." Draw/no-contest 50/50 per series `important_info`. Governing version verified via Wayback CDX: the `UFC.pdf` terms file shares an identical content digest (`AGN3TK3VVFDXWXPYKNCUILO65KVNOZMK`) across snapshots dated 2026-01-11, 2026-03-08, and 2026-05-16 — byte-identical across the April 11, 2026 event. [Terms PDF][terms]

[^cert]: KalshiEX LLC, CFTC Regulation 40.6 amendment notification for the "Will `<achievement>` be held by `<participant>`?" contract (ACHIEVEMENTS rulebook), dated **July 18, 2025** — the operative certification governing the April 11, 2026 event; the amendment changed only the event-delay Payout Criterion, leaving the first-official-result, Expiration, draw, and revision clauses intact. [Cert PDF][cert]

[^mmaf-results]: Damon Martin, MMA Fighting, "UFC 327 results: Scoring error takes win away from Chris Padilla, fight declared majority draw," April 11, 2026, 11:42 PM UTC. Padilla initially scored a majority-decision win, then the result corrected to a majority draw. [Article][mmaf-results]

[^mmaf-draw]: MMA Fighting and corroborating reports (talkSPORT, LowkickMMA, Bloody Elbow, Cageside Press), April 11–12, 2026. The Padilla win was overturned to a majority draw the same night, announced on the live broadcast, after officials found all three judges missed the round-3 point deduction. [Article][mmaf-results]

[^mmaf-protest]: Mike Heck, MMA Fighting, "Chris Padilla submits formal protest after scoring error changed win to majority draw at UFC 327," April 12, 2026. [Article][mmaf-protest]

[^mmaf-denied]: Mike Heck, MMA Fighting, "Chris Padilla's formal protest to overturn UFC 327 result denied," April 23, 2026; corroborated by MMA Mania, "UFC fighter at center of scoring controversy KO'd by Florida commission," April 23, 2026. The Florida Athletic Commission denied the protest; the majority draw stands as the permanent official result. [Article][mmaf-denied]

[^polypunter]: PolyPunter, "Kalshi UFC Resolution on Padilla vs Mederos...," April 19, 2026. Reports Kalshi settled on the first announced result, paying Padilla contracts, and states "UFC announced the update during the live broadcast, but Kalshi had already settled its market"; draw/Mederos holders received nothing. [Article][polypunter]

[^predictionnews]: Chris Gerlacher, PredictionNews, "Kalshi UFC Resolution Echoes 2025 Oscars Viewership Market," April 2026. Reports the Padilla payout and nothing for Mederos; quotes the rule that "...any revisions after Expiration will not be considered"; draws the analogy to the 2025 Oscars viewership market where Kalshi settled on the initial reported figure. [Article][predictionnews]

[api-series]: https://api.elections.kalshi.com/trade-api/v2/series/KXUFCFIGHT
[api-event]: https://api.elections.kalshi.com/trade-api/v2/events/KXUFCFIGHT-26APR11PADMED
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/UFC.pdf
[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/UFC.pdf
[mmaf-results]: https://www.mmafighting.com/ufc/481933/ufc-327-results-scoring-error-takes-win-away-from-chris-padilla-fight-declared-majority-draw
[mmaf-protest]: https://www.mmafighting.com/ufc/482394/chris-padilla-submits-formal-protest-after-scoring-error-changed-win-to-majority-draw-at-ufc-327
[mmaf-denied]: https://www.mmafighting.com/ufc/484347/chris-padillas-formal-protest-to-overturn-ufc-327-result-denied
[polypunter]: https://polypunter.com/kalshi-ufc-resolution-on-padilla-vs-mederos-fight-sparks-debate-after-scorecard-correction-to-draw/
[predictionnews]: https://predictionnews.com/news/kalshi-ufc-resolution-echoes-2025-oscars-viewership-market
