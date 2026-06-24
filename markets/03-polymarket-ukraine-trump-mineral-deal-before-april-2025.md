# Polymarket: Ukraine agrees to Trump mineral deal before April

## Bottom line

**Finding: Failure. Polymarket published an ambiguous "agree to any deal" test, applied it inconsistently across two materially identical contracts (the sister Feb 25-28 market resolved No on the same February facts that this market later treated as Yes), issued a dispositive "too early / not yet Yes" clarification roughly two minutes before the UMA vote-commit window closed, and then allowed the contrary result to finalize Yes. Polymarket acknowledged the result contradicted its clarification but denied refunds because it was "not a market failure." The process, drafting, and cross-market consistency failures are conclusive; whether Yes was substantively wrong is indeterminate because the rule never defined when negotiations become a "deal." Confidence: high on the process/drafting/inconsistency failure; medium on outcome-correctness. Failure-resolved: Unresolved.**

Gamma confirms the before-April market resolved **Yes** (`outcomePrices ["1","0"]`, `umaResolutionStatus: resolved`), and the on-chain resolution transaction paid the Yes slot (`payoutNumerators [1,0]`) at 2025-03-25 00:21:27 UTC.[^api][^onchain-resolution] The materially identical sister market resolved **No** (`outcomePrices ["0","1"]`).[^friday-api] Polymarket's own representative stated the market "resolved against the expectations of our users and our clarification" but that "because this wasn't a market failure, we are not able to issue refunds."[^polymarket-response][^wu-post]

The common summary — that Polymarket resolved Yes even though the U.S.-Ukraine minerals agreement was not signed until April 30, 2025 — omits a decisive part of the rule. The market did not require signature or enactment; it said an **announcement of a deal would qualify regardless of if/when the deal is enacted.**[^api] So the failure here is not simply a true No converted to a false Yes. It is a venue that drafted an under-specified event test, applied it inconsistently across related markets, clarified too late for voters to respond normally, let the contrary result finalize, and then declined to remedy it.

## Market details

- **Venue:** Polymarket
- **Question:** "Ukraine agrees to Trump mineral deal before April?" — gamma event id 17740, market id 521607.[^api]
- **Slug:** `ukraine-agrees-to-give-trump-rare-earth-metals-before-april`
- **Sister market:** `ukraine-agrees-to-trump-mineral-deal-by-friday`, "Ukraine agrees to Trump mineral deal by Friday?" (Feb 25-28 window).[^friday-api]
- **Stated event window:** February 2 through March 31, 2025, 11:59 PM ET (`endDate` 2025-03-31T12:00:00Z).[^api]
- **conditionId:** `0x1663edea3eba0d1ae8f064276dd426cb0497a19bb5188dae48a2f8fa8ea34da8`; **questionID:** `0x96bfe57cfa7b5373eaf8fd307993960738a1824a87943ea2e953540c5e263822`.[^api]
- **Resolver contract:** Polymarket UMA CTF Adapter V2, `0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74`.[^onchain-resolution]
- **Final resolution:** Yes; finalized 2025-03-25 00:21:27 UTC (`closedTime`, `umaEndDate`); `umaResolutionStatus: resolved`.[^api]
- **Reported volume:** approximately $7.08 million.[^api]

## What happened

### The rule (verbatim)

The before-April market's binding description read:

> This market will resolve to "Yes" if the United States and Ukraine agree to any deal between February 2 and March 31, 2025, 11:59 PM ET, that explicitly involves Ukrainian rare earth elements. Otherwise this market will resolve to "No". … An announcement of a deal will qualify regardless of if/when the deal is enacted. The resolution source for this market will be official information from the governments of the US and Ukraine.[^api]

The rule did not require a signature, legal enactment, ratification, or performance. It also never defined whether a framework or approved draft was a "deal," whether unilateral approval proved bilateral agreement, or whether the market could resolve before March 31 while the alleged agreement remained disputed.

### The sister market resolved No on the same facts

Polymarket simultaneously ran "Ukraine agrees to Trump mineral deal by Friday?" (Feb 25-28). Its rule was verbatim materially identical — same "agree to any deal," the same clause that "An announcement of a deal will qualify regardless of if/when the deal is enacted," and the same "official information from the governments of the US and Ukraine" source (the only differences are the Feb 25-28 window and the phrase "rare earth elements or minerals").[^friday-api] That market resolved **No** (`outcomePrices ["0","1"]`, resolved 2025-03-01 08:00:07 UTC).[^friday-api]

This is a direct internal contradiction: the February framework evidence later used to support Yes in the before-April market was the same evidence available during the by-Friday market. The two contracts treated the same event under materially the same rule as both No and Yes.

### A late Yes proposal and a last-minute clarification

Two contemporaneous participant reconstructions — Tenadome and `@Domahhhh` — report that a major Yes holder proposed Yes on Saturday evening, March 22, while the market was still open and trading at a low probability (around 15%). The proposal was disputed and escalated to a UMA token-holder vote.[^domah][^tenadome]

Both accounts report that Polymarket issued its clarification at approximately 11:58 PM UTC on March 23, roughly two minutes before the vote-commit period ended, and a second notice roughly two minutes before the reveal period ended on March 24 indicating it would allow the market to follow the UMA vote.[^tenadome][^domah] The accounts paraphrase the clarification as saying it was too early for the market to resolve and that the result was not yet Yes. **The exact verbatim clarification text is not preserved in any reachable primary source; both threads paraphrase it.**

UMA uses a commit-and-reveal process. Once votes are committed, voters cannot simply change them in response to a clarification; they can reveal or abstain.[^tenadome] A clarification delivered about two minutes before commit close therefore could not reliably guide already-committed votes.

### The contrary vote finalized Yes

The vote favored Yes, and the market finalized Yes at 2025-03-25 00:21:27 UTC. The on-chain resolution transaction recorded a Yes payout vector (`payoutNumerators [1,0]`).[^onchain-resolution][^api] Finalization occurred six days before the March 31 deadline; even if the February framework did not yet qualify, the market could have remained open through March 31 rather than converting an unresolved factual dispute into a final Yes.

### Polymarket acknowledged the breakdown

A statement from a Polymarket representative ("Tanner"), reproduced by Wu Blockchain and crypto.news, read:

> We are aware of the situation regarding the Ukrainian Rare Earth Market. This market resolved against the expectations of our users and our clarification. Unfortunately, because this wasn't a market failure, we are not able to issue refunds.[^polymarket-response][^wu-post]

Polymarket called the event unprecedented and promised collaboration with UMA, monitoring, and clearer rules.[^polymarket-response]

## The allegation against Polymarket

The allegation has four parts: (1) the market resolved Yes contrary to Polymarket's own clarification that it was too early; (2) the clarification was issued too late — about two minutes before the commit window closed — to guide committed UMA votes; (3) Polymarket applied materially identical rules inconsistently, with the sister market resolving No; and (4) concentrated UMA voting power overrode the venue's interpretation. Polymarket then acknowledged the contradiction but denied refunds.[^tenadome][^domah][^polymarket-response]

## Polymarket's defense

Polymarket's public position had two parts: the result contradicted its clarification and was unprecedented, but it was not classified as a "market failure," so refunds were unavailable.[^polymarket-response] The implicit procedural defense is that the contract resolved through the published, binding UMA mechanism, and Polymarket's decision to let the result follow the UMA vote is consistent with that.[^tenadome] This explains the non-reversal but does not explain why a binding result contrary to the venue's own clarification should not count as a failure.

There is also a stronger substantive defense of Yes than most reporting acknowledges. The rule required agreement, not signature, and expressly said an announcement qualified regardless of enactment. On February 25, Bloomberg and The Washington Post reported the parties had agreed to a framework; on February 26, Ukraine's Cabinet officially approved the draft bilateral agreement and authorized two ministers to sign it.[^bloomberg][^washington-post][^cabinet-order] Proponents also cited a February 27 Bessent (Fox Business) interview and Trump's expectation that a deal would be signed soon.[^domah] On a literal, broad reading of "agree to any deal," the February framework could satisfy the rule even though the contemplated signing did not occur on February 28.[^ap-oval-office]

Against that, the February document was described as a framework or draft; implementation details remained, the planned signing failed, and the parties kept speaking as though an operative agreement had not been concluded. Under that narrower reading — which Polymarket itself adopted in its clarification — the correct answer on March 23 was Too Early, then No if no qualifying agreement was reached by March 31.[^bloomberg][^ap-oval-office][^tenadome]

## Assessment

### Did the venue resolve against its own clarification?

**Yes.** Polymarket told voters the market was too early and not yet Yes; the final result was Yes; and Polymarket expressly acknowledged the contradiction.[^polymarket-response][^tenadome] This establishes a failure in the resolution stack regardless of whether the February framework ultimately should have qualified.

### Was the clarification issued too late?

**Yes.** Two independent participant accounts place the clarification at roughly two minutes before the commit window closed, after which committed UMA votes could not normally be changed.[^tenadome][^domah] Polymarket's later promise of a more timely clarification system implicitly conceded the defect.[^polymarket-response]

### Were materially identical rules applied inconsistently?

**Yes.** Gamma confirms verbatim that the sister Feb 25-28 market and the before-April market shared the operative "agree to any deal" and "announcement … qualify regardless of if/when enacted" language and the same government source. The sister market resolved No (`["0","1"]`); the before-April market resolved Yes (`["1","0"]`).[^api][^friday-api]

### Was the final Yes outcome clearly wrong?

**Indeterminate.** Signature was expressly unnecessary, and the February reporting plus the Ukrainian Cabinet order give Yes serious textual support; but the rule never defined whether an approved framework was a completed "deal," and the failed signing supports Too Early/No.[^api][^cabinet-order][^bloomberg][^ap-oval-office] Both readings had material support.

### Was this a proven governance attack?

**No, not conclusively.** CoinDesk reported `BornTooLate.eth` accumulated roughly 1.3 million UMA as a top-five governance staker, but found no profitable attack: building that position would have cost over $2 million, while the largest winner gained about $55,000 and the largest loser forfeited about $73,000.[^coindesk] crypto.news described five million tokens across three accounts (about 25% of votes).[^polymarket-response] Tenadome argued the deciding voters were ordinary recurring UMA whales protecting committed votes from slashing, not a coordinated attacker.[^tenadome] The economics cut against a profit-motivated attack; the documented failure does not depend on proving manipulation.

### Overall classification

- **Resolution-process failure:** Yes (untimely clarification; contrary result finalized)
- **Rule-drafting failure:** Yes ("agree to any deal" never defined when negotiations become a deal)
- **Inconsistent related-market resolution:** Yes (sister No vs. this Yes, verbatim-identical rule)
- **Final-outcome error:** Indeterminate — Yes and Too Early/No each had material textual support
- **Governance attack:** Alleged, not established; CoinDesk economics cut against a profit motive
- **Remediation:** Failure acknowledged but refunds denied
- **Best public verdict:** Failure (process + drafting + inconsistency conclusive; final-outcome correctness indeterminate). Failure-resolved: Unresolved.

## Precise blocker to a stronger finding

The blocker to a conclusive *outcome* finding is the rule's failure to define when negotiations become a "deal." The factual record is reasonably clear — the parties negotiated a framework, press reports said they had agreed to it, Ukraine officially approved the draft and authorized signature, the planned signature did not occur, the parties continued negotiating, and a later agreement was signed on April 30.[^cabinet-order][^ap-oval-office][^final-agreement] What is missing is a predetermined contractual rule assigning those facts to Yes, No, or Too Early; Polymarket tried to supply that rule via a clarification only after votes were committed. Two further evidentiary blockers: the exact clarification wording is paraphrased in every reachable source (not a verified quote), and gamma's `umaResolutionStatuses` array is empty, so the often-cited "two proposals / two disputes" count rests on the market-page UI, not the API.[^api][^tenadome]

## Sources

### Primary

[^api]: Polymarket Gamma API, [event record for the before-April market][api]. Preserves the verbatim rule, dates, volume, `conditionId`/`questionID`, `umaResolutionStatus: resolved`, `closedTime`/`umaEndDate` 2025-03-25 00:21:27 UTC, and final `outcomePrices ["1","0"]` (Yes). `umaResolutionStatuses` is empty.

[^friday-api]: Polymarket Gamma API, [event record for the by-Friday sister market][friday-api]. Verbatim materially identical rule (Feb 25-28 window); final `outcomePrices ["0","1"]` (No); resolved 2025-03-01 08:00:07 UTC.

[^onchain-resolution]: PolygonScan, [resolution transaction `0x0f0d…807ea`][onchain-resolution], 2025-03-25 00:21:27 UTC. Records a Yes payout vector (`payoutNumerators [1,0]`); resolver is the Polymarket UMA CTF Adapter V2 (`0x6A9D…4F74`).

[^cabinet-order]: Cabinet of Ministers of Ukraine, [Order approving the draft bilateral agreement and authorizing signature][cabinet-order], February 26, 2025.

[^final-agreement]: Cabinet of Ministers of Ukraine, [Ukraine and the United States sign Economic Partnership Agreement][final-agreement], May 1, 2025. Records the April 30 signature.

[^wu-post]: Wu Blockchain, [X post reproducing Polymarket's Discord statement][wu-post], March 26, 2025. (Direct page access was paywalled at re-verification; quote corroborated via crypto.news.)

### Contemporaneous reporting and reconstruction

[^bloomberg]: Bloomberg via BNN Bloomberg, [Ukraine to Agree With US on Terms for Minerals Deal][bloomberg], February 25, 2025.

[^washington-post]: The Washington Post, [Ukraine and U.S. agree to framework for minerals deal][washington-post], February 25, 2025.

[^ap-oval-office]: Associated Press, [Zelenskyy leaves White House without signing minerals deal after Oval Office blowup][ap-oval-office], February 28, 2025.

[^polymarket-response]: crypto.news, [Polymarket suffers governance attack due to UMA whale intervention][polymarket-response], March 26, 2025. Reproduces the verbatim Tanner refund-denial statement and the five-million-tokens / three-accounts / ~25% figure. Its "proven attack" framing is stronger than the evidence supports.

[^coindesk]: CoinDesk, [A Contentious Ukraine Bet Leads to Clash Between Polymarket, UMA Communities][coindesk], March 26-27, 2025. Reports `BornTooLate.eth` ~1.3M UMA / top-five staker, and that the position cost over $2M while the largest winner gained ~$55K and largest loser ~$73K — no profitable attack.

[^tenadome]: Tenadome, [archived thread disputing the governance-attack characterization][tenadome], March 26, 2025. Provides the commit/reveal and clarification timeline (~11:58 PM UTC March 23, ~2 min before commit close). Participant account, not an official record.

[^domah]: `@Domahhhh`, [archived investigation of the proposal and vote sequence][domah], March 27, 2025. Documents the Saturday March 22 ~15% proposal, the sister-market contradiction, the clarification timing, and the Yes argument (including the Feb 27 Bessent interview). Advocacy-oriented trader reconstruction, used cautiously.

[api]: https://gamma-api.polymarket.com/events?slug=ukraine-agrees-to-give-trump-rare-earth-metals-before-april
[friday-api]: https://gamma-api.polymarket.com/events?slug=ukraine-agrees-to-trump-mineral-deal-by-friday
[onchain-resolution]: https://polygonscan.com/tx/0x0f0d0bd28dfae70d35269f883986e1780b58398fffe34f72a30aa3e998c807ea
[cabinet-order]: https://www.kmu.gov.ua/npas/pro-pidpysannia-dvostoronnoi-uhody-pro-vstanovlennia-pravyl-ta-umov-investytsiinoho-fondu-t260225
[final-agreement]: https://www.kmu.gov.ua/en/news/ukraina-i-ssha-pidpysaly-uhodu-pro-ekonomichne-partnerstvo-ta-stvorennia-investytsiinoho-fondu-vidbudovy
[wu-post]: https://x.com/WuBlockchain/status/1904772495649235117
[bloomberg]: https://www.bnnbloomberg.ca/investing/commodities/2025/02/25/ukraine-to-agree-with-us-on-terms-for-minerals-deal/
[washington-post]: https://www.washingtonpost.com/politics/2025/02/25/ukraine-minerals-deal-trump-zelensky/
[ap-oval-office]: https://apnews.com/article/eebdf97b663c2cdc9e51fa346b09591d
[polymarket-response]: https://crypto.news/polymarket-suffers-governance-attack-due-to-uma-whale-intervention/
[coindesk]: https://www.coindesk.com/markets/2025/03/26/polymarket-suffers-uma-governance-attack-after-rouge-actor-becomes-top-5-token-staker
[tenadome]: https://threadreaderapp.com/thread/1904789723383529517.html
[domah]: https://threadreaderapp.com/scrolly/1905258165777596812
