# Polymarket: TikTok banned in the U.S. before May 2025

## Bottom line

**Finding: No failure. The governing market rule resolved Yes if a federally mandated ban on TikTok download and/or use went into effect by April 30, 2025 — with no minimum-duration, permanence, or through-May requirement. The federal divest-or-ban law's prohibitions took effect January 19, 2025 (the Supreme Court having upheld the law January 17), and TikTok went dark in the U.S. from the night of January 18 for roughly twelve hours. Both the legal trigger and the practical outage satisfied the rule, and Polymarket resolved Yes. The "too brief to count as a ban" objection is a consumer-expectation complaint, not a rule violation. Confidence: high.**

The market's `outcomePrices` are `["1","0"]` — Yes — and it is closed and `automaticallyResolved`, with `umaResolutionStatus` "resolved" and an empty `umaResolutionStatuses` array, i.e. no recorded UMA dispute cycle.[^gamma] The verbatim resolution text required only that a ban "mandated by US federal law, policy, or the court system" have "gone into effect" by April 30, 2025; it imposed no duration condition and contained a sale-into-compliance carve-out (resolve No) that never triggered.[^gamma] The Protecting Americans from Foreign Adversary Controlled Applications Act's prohibitions became effective January 19, 2025, the app went dark before that effective date and was pulled from app stores, and Trump's January 20 executive order paused enforcement while expressly acknowledging the January 19 effective date.[^supreme-court][^npr][^white-house] Under the actual rule, Yes was a correct application, not a misresolution.

## Market details

- **Venue:** Polymarket
- **Question:** "TikTok banned in the US before May 2025?" — gamma event id `12641`, market id `507276`, slug `tiktok-banned-in-the-us-before-may-2025`, conditionId `0xef8cf8b45ef7e3a607a72b6e1d56bede869fdd81795b63db847de1090bf11c41`.[^gamma]
- **Governing rule (verbatim, gamma description — unchanged since creation September 17, 2024):** "This market will resolve to "Yes" if the TikTok app is banned for download and/or use by the majority of Americans in the United States by April 30, 2025, 11:59 PM ET. Otherwise, this market will resolve to "No". For this market to resolve to "Yes", a ban mandated by US federal law, policy, or the court system must have gone into effect (as defined above) within the above-stated timeframe. If TikTok is sold to another entity in such a way that it comes into compliance with U.S. laws and regulations this market will resolve to "No". The primary resolution source for this market will be information from the US federal government, however a consensus of credible reporting will also be used."[^gamma]
- **Deadline:** April 30, 2025, 11:59 PM ET (`endDate` 2025-04-30).[^gamma]
- **Settled outcome:** `outcomePrices ["1","0"]` = Yes; `closed: true`; `automaticallyResolved: true`; `umaResolutionStatus` "resolved"; `umaResolutionStatuses` `[]`; `closedTime` 2025-01-22 00:31:19 UTC.[^gamma]
- **Reported volume:** approximately $119.65 million.[^gamma]

## What happened

The contract asked whether a federally mandated ban on TikTok download and/or use would go into effect by April 30, 2025. The Supreme Court upheld the Protecting Americans from Foreign Adversary Controlled Applications Act on January 17, 2025, and the Act's prohibitions became effective January 19, 2025 absent a qualified divestiture.[^supreme-court]

| Date (ET) | Event |
|---|---|
| Jan 17, 2025 | Supreme Court upholds the Act in *TikTok Inc. v. Garland*; prohibitions effective Jan 19.[^supreme-court] |
| Night of Jan 18, 2025 | TikTok goes dark in the U.S. roughly two hours before the Jan 19 effective date, showing an in-app "banned" message; app pulled from Apple App Store and Google Play.[^npr][^cnn] |
| Jan 19, 2025 | Service restored after about twelve hours following Trump's public assurances.[^nbc] |
| Jan 20, 2025 | Trump signs an executive order pausing enforcement for 75 days; the order states the Act's prohibitions "became effective on January 19, 2025."[^white-house] |

Polymarket resolved the market Yes; it is closed and `automaticallyResolved`, with `closedTime` 2025-01-22 00:31:19 UTC — roughly three months before the April 30 deadline — and no recorded UMA dispute.[^gamma]

## The allegation against Polymarket

The No-side objection was that TikTok was not meaningfully or durably banned, because the outage lasted only about twelve hours and service resumed after Trump's intervention.[^tradingview] In ordinary speech, some users expected "banned" to mean sustained practical unavailability, and they argued the brief app-store removal and outage should not count.

The objection would have force if the rule had required TikTok to remain unavailable, to be removed from app stores for a minimum period, or to stay banned through May 1.

## Polymarket's defense

The defense is the written rule and the public legal timeline:

- The rule resolves Yes if a ban "mandated by US federal law, policy, or the court system" has "gone into effect" by April 30, 2025; it imposes no duration, permanence, or through-May requirement.[^gamma]
- The Act's prohibitions became effective January 19, 2025, supplying the federal mandate and the effective date.[^supreme-court][^white-house]
- The rule covers a ban on download "and/or" use; TikTok went dark and was pulled from app stores, satisfying that test in practice as well as in law.[^npr][^cnn]
- Trump's January 20 executive order paused enforcement but expressly acknowledged the prohibitions had become effective January 19 — it delayed prosecution, it did not declare that the ban never took effect.[^white-house]
- The sale-into-compliance carve-out (resolve No) never triggered, as no qualified divestiture occurred by the deadline.[^gamma]

## Assessment

### Did a federally mandated ban go into effect before the deadline?

**Yes.** The Supreme Court upheld the Act on January 17, 2025, and its prohibitions became effective January 19, 2025; the White House executive order issued January 20 also states that the prohibitions "became effective on January 19."[^supreme-court][^white-house] That is a ban mandated by U.S. federal law that went into effect well before the April 30 deadline.

### Did TikTok become practically unavailable?

**Yes, temporarily.** TikTok went dark in the U.S. on the night of January 18, roughly two hours before the January 19 effective date, displaying an in-app message that it was banned, and was removed from the Apple and Google app stores; service was restored about twelve hours later on January 19.[^npr][^cnn][^nbc]

### Did the rule require the ban to last for any minimum duration?

**No.** The verbatim rule required only that the mandated ban "have gone into effect" within the timeframe. It did not require continuous enforcement, permanence, app-store removal for any minimum period, or unavailability through May.[^gamma]

### Did the sale carve-out or the enforcement pause defeat Yes?

**No.** No qualified divestiture brought TikTok into compliance, so the sale carve-out never triggered.[^gamma] Trump's executive order paused enforcement for 75 days but expressly acknowledged the January 19 effective date; an enforcement pause does not undo a prohibition that has already taken effect.[^white-house]

### Was Polymarket's Yes resolution correct, not merely defensible?

**Correct.** Both the legal trigger (prohibitions effective January 19) and the practical outage (the January 18 dark period and app-store removal) independently satisfy the rule. The market is `automaticallyResolved` to Yes with no recorded UMA dispute.[^gamma][^supreme-court][^npr]

### Overall classification

- **Resolution failure:** No
- **Misapplication of the rules:** No
- **Semantic ambiguity:** Low once the rule's "gone into effect" / no-duration text is read
- **Final Yes outcome:** Correct under the rule
- **Best public verdict:** No failure; a brief ban still qualified because the rule did not require duration

## Precise blocker to a stronger finding

None material. The decisive facts are verified from primary sources: the gamma description supplies the verbatim rule (including the sale-into-compliance carve-out) and the settlement data (`outcomePrices ["1","0"]`, `automaticallyResolved`, `umaResolutionStatuses []`); the Supreme Court opinion and the White House executive order fix the January 19 effective date; and contemporaneous reporting documents the January 18 dark period and roughly twelve-hour outage. The only residual is the absence of an archived capture of the rendered polymarket.com page at settlement, which is immaterial because the gamma description is the authoritative rule text and has not changed since the market was created.

## Sources

[^gamma]: Polymarket Gamma API, event `tiktok-banned-in-the-us-before-may-2025` (id 12641; market id 507276; conditionId `0xef8cf8b45ef7e3a607a72b6e1d56bede869fdd81795b63db847de1090bf11c41`). Supplies the verbatim resolution rule (download and/or use; ban mandated by federal law/policy/court must have "gone into effect" by April 30, 2025; sale-into-compliance carve-out resolves No), the settlement data (`outcomePrices ["1","0"]` = Yes; `closed: true`; `automaticallyResolved: true`; `umaResolutionStatus` "resolved"; `umaResolutionStatuses` `[]`; `closedTime` 2025-01-22 00:31:19 UTC), and reported volume ~$119.65M. [API][gamma]

[^supreme-court]: Supreme Court of the United States, *TikTok Inc. v. Garland*, 604 U.S. 56, January 17, 2025. Upholds the Act and describes the prohibitions as effective beginning January 19, 2025 absent qualified divestiture. [Opinion PDF][supreme-court]

[^white-house]: The White House, "Application of Protecting Americans from Foreign Adversary Controlled Applications Act to TikTok," January 20, 2025. States that the Act's prohibitions became effective January 19 and instructs the Attorney General not to enforce the Act for 75 days. [Action][white-house]

[^npr]: NPR, "TikTok is offline in the U.S. after Supreme Court upholds ban," January 18, 2025. Reports TikTok going offline in the U.S. the night of January 18 ahead of the ban, with an in-app message and removal from app stores. [NPR][npr]

[^cnn]: CNN Business, "TikTok ban: App shuts down in the United States hours ahead of a ban," January 18, 2025. Reports the shutdown hours before the ban's effective date and disappearance from the Apple App Store and Google Play. [CNN][cnn]

[^nbc]: NBC News, "What to know as TikTok resumes service following Trump's statement on delaying the ban," January 2025. Reports service restored about twelve hours after the outage following Trump's assurances. [NBC][nbc]

[^tradingview]: Cointelegraph via TradingView, "Polymarket faces backlash over TikTok ban prediction resolution," January 2025. Reports the market title, volume, Yes resolution, user backlash, and competing user interpretations of "banned." [TradingView][tradingview]

[gamma]: https://gamma-api.polymarket.com/events?slug=tiktok-banned-in-the-us-before-may-2025
[supreme-court]: https://www.supremecourt.gov/opinions/24pdf/604us1r07_k536.pdf
[white-house]: https://www.whitehouse.gov/presidential-actions/2025/01/application-of-protecting-americans-from-foreign-adversary-controlled-applications-act-to-tiktok/
[npr]: https://www.npr.org/2025/01/18/nx-s1-5266146/tiktok-offline-supreme-court-ban
[cnn]: https://www.cnn.com/2025/01/18/business/trump-tiktok-ban
[nbc]: https://www.nbcnews.com/news/us-news/tiktok-ban-sunday-what-to-know-rcna188256
[tradingview]: https://www.tradingview.com/news/cointelegraph%3A3f4adad24094b%3A0-polymarket-faces-backlash-over-tiktok-ban-prediction-resolution/
