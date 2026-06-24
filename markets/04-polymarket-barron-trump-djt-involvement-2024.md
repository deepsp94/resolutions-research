# Polymarket: Was Barron involved in $DJT?

## Bottom line

**Finding: Failure — a confirmed platform-level resolution-governance and transparency failure, but not a proven wrong contractual payout. The market designated UMA as its binding resolver; UMA's dispute process returned No and the contract settled No ($1 to No). Polymarket then publicly declared UMA "wrong," called Barron's involvement "conclusive… in some way," and separately reimbursed Yes holders — all without disclosing evidence tied to the operative "involved in the creation" criterion and the June 23 cutoff. The official No payout was left in place while the platform told users the truth was effectively Yes. Confidence: high on the governance/transparency failure; low on any conclusive factual answer about Barron. Failure-resolved: Unresolved.**

The binding rule resolved Yes only if "a preponderance of evidence suggests that Barron Trump was involved in the **creation** of the Solana token $DJT," with UMA making the determination "as of 12 PM ET, June 23."[^api] The optimistic oracle received two No proposals, each disputed; UMA's adjudication produced a final **No**, and the CTF market settled accordingly — `outcomePrices` `["0","1"]`, No paid $1.[^api][^market]

After finalization, Polymarket publicly stated "We firmly believe that UMA got this resolution wrong," then two days later said it was "conclusive" Barron was involved "in some way" and announced refunds for Yes holders — providing no evidence and never tying its claim to the narrower creation criterion.[^wrong-statement][^refund-statement][^coindesk-final] That contradiction between the platform's official settlement (No) and its public statement (effectively Yes), absent auditable evidence, is the established failure. It is **not** established that UMA misapplied the written rule, that Yes was the required answer, or that No holders were paid contrary to the contract.

## Market details

- **Venue:** Polymarket
- **Event/Market:** `was-barron-involved-in-djt` — event id 11201, market id 502710.[^api]
- **Question:** "Was Barron involved in $DJT?" (operative criterion narrower than the title).
- **conditionId:** `0x8fb1c85df2e64bedc411454f69267ae172a34d4c9b1693e7a768fc604c299ea0`; **questionID:** `0x1f9fdf6ad9554657a931af64b5abb986b8cf7fb28066f91337f0c30d95455514`.[^api]
- **Payout Criterion (verbatim):** "This market will resolve to 'Yes' if a preponderance of evidence suggests that Barron Trump was involved in the creation of the Solana token $DJT. Otherwise this market will resolve to 'No'. Determination as to whether Barron was involved in the creation of $DJT will be made by this market's decentralized resolver, UMA, and will take into account all available evidence as of 12 PM ET, June 23."[^api]
- **Resolver:** UMA optimistic oracle via `UmaCtfAdapter` `0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74` (`resolvedBy`); umaBond 500, umaReward 5.[^api][^adapter]
- **Final resolution:** No. `outcomePrices` `["0","1"]`; `umaResolutionStatus` "resolved"; `automaticallyResolved` true; closed 2024-06-26 00:20:11 UTC.[^api]
- **Reported volume:** ≈ $1,143,639.[^api]

## What happened

Polymarket listed the market June 20, 2024, with an evidence cutoff of 12 PM ET, June 23. The optimistic oracle recorded the following resolution sequence: outcome proposed No → disputed → outcome proposed No → disputed → final outcome No.[^market] The first and third entries were proposals to the optimistic oracle, not two independent UMA rulings; the final No came through UMA's disputed adjudication. The CTF market settled to No, with No shares paying $1 and Yes shares $0.[^api][^market]

The public Yes case rested on: a June 17 Pirate Wires report that Barron was "spearheading" the project; blockchain investigator ZachXBT establishing that Martin Shkreli was the token's creator, plus a screenshot of Shkreli claiming he created the token "with Barron"; Shkreli's X Spaces claims that Barron was among a ~40–50-person team; an unauthenticated screenshot of a contact saved as "BT" discussing wallets, liquidity, fees, and a token tax; and Mike Solana saying his sources gave him high confidence as to creation, distribution, and promotion.[^market] None of this evidence was independently authenticated, and the decisive material (a Barron statement, a verified wallet, Shkreli's claimed "1,000 pieces of evidence") was never publicly produced.[^coindesk-june24][^dlnews-vote]

After the market finalized No, Polymarket repudiated its own resolver. On June 26 it posted that UMA "got this resolution wrong" and promised a near-term solution; on June 28 it called the involvement "conclusive… in some way," announced refunds for Yes holders, and said it was working to improve its oracle and resolution methodology — without disclosing any supporting evidence.[^wrong-statement][^refund-statement][^coindesk-final]

## The allegation against Polymarket

Polymarket made UMA the binding resolver, the market finalized No through the proper optimistic-oracle dispute process, and Polymarket then publicly said UMA was wrong and separately reimbursed Yes holders — without disclosing evidence tied to the "involved in creation" criterion and the June 23 cutoff. It left the official No payout in place while telling users the truth was effectively Yes, producing two irreconcilable official accounts of what the market meant and how it resolved. The factual premise is confirmed on every point; the question is whether it amounts to a misresolution or a governance/transparency failure.

## Polymarket's defense

Polymarket did not defend the official No result; its public position was that UMA had resolved incorrectly, that markets must resolve to truth by the best available means, and that Barron's involvement was conclusive.[^wrong-statement][^refund-statement] The strongest defense of its *conduct* (as distinct from the substantive Yes claim) is that it may have trusted information unavailable to UMA voters, that by the time it objected the on-chain result had already finalized, and that reimbursing Yes holders mitigated harm without removing the ordinary No payout from traders who relied on the written process. Those points are inferences from the sequence and the remedy; Polymarket never published a technical explanation or the evidence underlying its "conclusive" claim.

## UMA's defense

UMA's process has a coherent, sourced defense of No. Founder Hart Lambur told DL News that "our voters did well and acted honestly. This was ambiguous and voters thought a 'NO' answer was the least bad answer in a difficult situation."[^dlnews-vote] A voter articulated the operative distinction: "I think there's a preponderance of evidence that the key players here have been in contact with Barron Trump. However, I don't think the evidence is there that Barron was involved in the creation of the token."[^dlnews-vote] The contract asked about creation, not contact, promotion, or later involvement — so weighing the unauthenticated public Yes evidence as falling short of creation was a rational application of the rule. There is no sourced basis to allege vote manipulation, corruption, or governance attack.

## The reimbursement

Polymarket did not replace No with Yes and did not pay Yes shares as winners. It made a separate USDC reimbursement to Yes holders, executed on-chain June 28, 2024.[^refund-transaction] The decoded `disperseToken` payload (via Disperse.app, `0xD152f549545093347A162Dce210e7293f1452150`) distributed to **exactly 133 recipients** totaling **$95,106.2647** — not a $1-per-share Yes payout. The amounts track purchase cost/loss, not winnings:

- Address `0x0bb3ef…10bd` bought 847.264703 Yes shares for ≈ $190.91 and received **188.3673 USDC** — not the 847.26 a $1/share payout would imply.[^refund-example-large]
- Address `0x5c40…d4eb` bought 33.333332 Yes shares for ≈ $10.00 and received **9.90 USDC** — not 33.33.[^refund-example-small]

Both decoded amounts were re-verified against the on-chain transaction. Polymarket never published the eligibility snapshot or calculation formula. The reimbursement was reasonable loss-mitigation, not itself the failure — and not a two-sided market cancellation.

## Assessment

### Was the operative rule "involved in the creation," with a June 23 cutoff?

**Yes.** Verified verbatim from the gamma API description: Yes only if "a preponderance of evidence suggests that Barron Trump was involved in the creation of… $DJT," determined by UMA "as of 12 PM ET, June 23."[^api] The broad title ("Was Barron involved in $DJT?") is wider than this operative test; the mismatch became material when Polymarket later defended Yes with the looser "in some way" phrasing.[^refund-statement]

### Did the market settle No through the written process?

**Yes.** `outcomePrices` `["0","1"]` (No paid $1), `umaResolutionStatus` "resolved," `resolvedBy` the UMA CTF adapter, closed 2024-06-26.[^api] The sequence was two No proposals, two disputes, and a final adjudicated No — UMA's encoded process, not a deviation from it.[^market][^dlnews-vote]

### Was UMA's No clearly wrong, or the factual truth clearly No?

**Neither.** The public Yes case was substantial enough to create a genuine dispute but consisted of anonymous sourcing, an interested participant (Shkreli), and unauthenticated screenshots; the No reading had a rational basis (contact established, creation not).[^dlnews-vote][^coindesk-june24] Conversely, a preponderance standard does not require official confirmation, so the absence of a Barron statement or verified wallet does not make No conclusively correct. The factual answer is indeterminate from the public record.

### Did Polymarket establish that Yes was correct?

**No.** It announced a conclusion without publishing its basis and described involvement "in some way," which need not satisfy the narrower creation criterion.[^refund-statement][^coindesk-final] CoinDesk confirms the X account "did not provide any evidence supporting its claim."[^coindesk-final] A statement of belief is not auditable evidence.

### Was this a misresolution, or a governance/transparency failure?

**A governance/transparency failure, not a proven misresolution.** On the contract as written, No was the authoritative result produced by the named resolver through the expected dispute process. The confirmed failure is that Polymarket repudiated its own designated resolver in public, asserted a contrary "conclusive" truth without auditable evidence tied to the exact criterion and cutoff, and left an official No settlement standing alongside a public statement that the truth was effectively Yes — three incompatible messages from one venue. Outsourcing adjudication does not remove Polymarket's responsibility for designing a market its chosen stack could resolve credibly.

### Was the failure resolved?

**No — Unresolved.** The reimbursement mitigated Yes holders' losses but did not reconcile the contradiction: the official outcome remains No, the platform's stated truth remains Yes, no evidence was disclosed, and the reimbursement formula/eligibility were never published.

### Overall classification

- **Wrong contractual payout:** Not established
- **Wrong factual answer:** Indeterminate
- **Oracle corruption or manipulation:** Not established
- **Encoded oracle procedure followed:** Yes, on the available record
- **Resolution-governance / platform-vs-oracle contradiction:** Yes
- **Unsupported post-final platform claim:** Yes
- **Material title/rule mismatch:** Yes
- **Reimbursement:** Reasonable mitigation; 133 recipients / $95,106.2647, not $1/share; formula undisclosed
- **Best public verdict:** Failure (governance/transparency); Failure-resolved: Unresolved
- **Confidence:** High on the platform-level contradiction; low on a conclusive Yes/No factual answer

## Precise blocker to a stronger finding

A conclusive factual finding is blocked by missing and unauthenticated evidence: the source material behind Pirate Wires, authentication that "BT" was Barron and concerned $DJT, verified wallet/transaction evidence tying Barron to creation, Shkreli's claimed evidence trove, a statement from Barron or an authenticated representative, or the evidence Polymarket relied on for "conclusive." The timing would also need to fall within the noon-ET June 23 cutoff. Separately, the exact eligibility snapshot and formula behind the reimbursement were never disclosed; the decoded on-chain amounts establish only that it was a reimbursement (133 recipients, $95,106.2647), not a Yes winning payout.

## Sources

[^api]: Polymarket Gamma API, event `was-barron-involved-in-djt`. Records event id 11201, market id 502710, the verbatim creation/UMA/cutoff rule, conditionId, questionID, `outcomePrices` `["0","1"]`, `umaResolutionStatus` "resolved", `resolvedBy` `0x6A9D…4F74`, umaBond/umaReward, volume ≈ $1,143,639, and closedTime 2024-06-26 00:20:11 UTC. [API][api]

[^market]: Polymarket, "Was Barron involved in $DJT?" market page. Records the rule, the two No proposals, two disputes, final No outcome, and resolution time; surfaces the public Yes evidence (Pirate Wires, ZachXBT/Shkreli, the "BT" screenshot, Mike Solana). [Market][market]

[^adapter]: Polygon Blockscout, verified `UmaCtfAdapter` contract used by Polymarket as `resolvedBy`. [Contract][adapter]

[^wrong-statement]: Polymarket, X statement, June 26, 2024: "We firmly believe that UMA got this resolution wrong. We're working on a near term solution and will announce it today. It's critical to uphold the integrity of the marketplace and pricing. Standby." [X][wrong-statement]

[^refund-statement]: Polymarket, X statement, June 28, 2024: Barron was "conclusive[ly]… involved in some way"; announced refunds for Yes holders and that it is "working to improve our oracle and resolution methodology"; provided no evidence. [X][refund-statement]

[^refund-transaction]: Polygon Blockscout, USDC reimbursement transaction `0x8037705f9ecfb375bb114318fed11aede3c8d001eabccbc5d66ae711b7479ac1`, June 28, 2024, 03:38 UTC. Decoded `disperseToken` input distributes to exactly 133 recipients totaling $95,106.2647 USDC.e via Disperse.app (`0xD152f549545093347A162Dce210e7293f1452150`). [Tx][refund-transaction]

[^refund-example-large]: Polymarket Data API, trades for `0x0bb3ef70625830cc6df761e1ea03a76113ac10bd`: 847.264703 Yes shares for ≈ $190.91; reimbursement of 188.3673 USDC (decoded on-chain). [Trades][refund-example-large]

[^refund-example-small]: Polymarket Data API, trades for `0x5c407bf7c5472a012cedb6cc3c74b2e6c475d4eb`: 33.333332 Yes shares for ≈ $10.00; reimbursement of 9.90 USDC (decoded on-chain). [Trades][refund-example-small]

[^dlnews-vote]: DL News, "Polymarket slams vote on Barron Trump, DJT token," June 2024. Quotes Hart Lambur ("our voters did well and acted honestly… 'NO' answer was the least bad answer"), the voter "contact… but not creation" reasoning, and Mike Solana's claims. [DL News][dlnews-vote]

[^coindesk-june24]: CoinDesk, June 24, 2024. Records the two disputed No proposals, the absence of a Barron or campaign statement, and reliance on Shkreli's account. [CoinDesk][coindesk-june24]

[^coindesk-final]: CoinDesk, "Polymarket Says It's 'Conclusive' Barron Trump Was Involved in $DJT," updated June 28, 2024. Reports Barron was "involved in the token 'in some way,'" that the X account "did not provide any evidence supporting its claim," that Polymarket "plans to refund holders of the 'yes' side," and is "working to improve our oracle and resolution methodology." [CoinDesk][coindesk-final]

[api]: https://gamma-api.polymarket.com/events?slug=was-barron-involved-in-djt
[market]: https://polymarket.com/event/was-barron-involved-in-djt
[adapter]: https://polygon.blockscout.com/address/0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74?tab=contract
[wrong-statement]: https://x.com/Polymarket/status/1805998648788173006
[refund-statement]: https://x.com/Polymarket/status/1806479362377814378
[refund-transaction]: https://polygon.blockscout.com/tx/0x8037705f9ecfb375bb114318fed11aede3c8d001eabccbc5d66ae711b7479ac1
[refund-example-large]: https://data-api.polymarket.com/trades?user=0x0bb3ef70625830cc6df761e1ea03a76113ac10bd&market=0x8fb1c85df2e64bedc411454f69267ae172a34d4c9b1693e7a768fc604c299ea&limit=10000&takerOnly=false
[refund-example-small]: https://data-api.polymarket.com/trades?user=0x5c407bf7c5472a012cedb6cc3c74b2e6c475d4eb&market=0x8fb1c85df2e64bedc411454f69267ae172a34d4c9b1693e7a768fc604c299ea&limit=10000&takerOnly=false
[dlnews-vote]: https://www.dlnews.com/articles/defi/polymarket-slams-vote-on-barron-trump-and-djt-token/
[coindesk-june24]: https://www.coindesk.com/news-analysis/2024/06/24/biden-likely-to-win-popular-vote-but-not-presidency-prediction-market-signals
[coindesk-final]: https://www.coindesk.com/markets/2024/06/27/polymarket-contradicts-its-oracle-service-in-rarity-for-prediction-market
