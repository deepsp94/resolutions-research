# Polymarket: Ukraine agrees to Trump mineral deal before April?

## Bottom line

**Finding: Polymarket made a clear resolution-process and market-drafting error. It is not conclusive that the final Yes outcome was factually wrong under the published rule. Confidence: high on the process failure; medium on the outcome assessment.**

The original allegation is commonly summarized as: Polymarket resolved the market Yes even though the United States and Ukraine did not sign a minerals agreement until April 30, 2025. That summary omits a decisive part of the rule. The market did not require signature or enactment. It said that an **announcement of a deal would qualify regardless of whether or when it was enacted**.[^market]

There was a substantial textual basis for Yes. On February 25, Bloomberg and The Washington Post reported that the parties had agreed to a framework. On February 26, the Ukrainian Cabinet officially approved the draft bilateral agreement and authorized two ministers to sign it.[^bloomberg][^washington-post][^cabinet-order] Those facts could reasonably satisfy a rule asking whether the parties had "agree[d] to any deal."

The process nevertheless failed:

- An almost identical Polymarket contract covering February 25-28 resolved No, even though the February framework was already public.[^friday-market]
- Polymarket waited until approximately two minutes before the UMA voting commitment period ended to clarify that the broader market was too early to resolve and was not yet Yes.[^tenadome][^domah]
- The market then finalized Yes on March 25, before its March 31 deadline and contrary to that clarification.[^market][^onchain-resolution]
- Polymarket publicly acknowledged that the result contradicted its clarification, called the event unprecedented, promised new monitoring and clarification systems, but denied refunds because it said this was not a "market failure."[^polymarket-response][^wu-post]

The strongest conclusion is therefore not simply that a token whale changed a true No into a false Yes. The more firmly supported conclusion is that Polymarket published an ambiguous event test, applied that test inconsistently across related markets, issued a dispositive clarification too late for voters to respond normally, allowed the contrary result to finalize, and then declined to remedy it.

## Market details

- **Venue:** Polymarket
- **Question:** `Ukraine agrees to Trump mineral deal before April?`
- **Market opened:** February 3, 2025
- **Stated event window:** February 2 through March 31, 2025 at 11:59 p.m. ET
- **Final resolution:** Yes
- **Finalized:** March 25, 2025
- **Reported volume:** approximately $7.08 million
- **Market page:** [Polymarket][market]
- **Primary metadata:** [Polymarket Gamma API][api][^api]
- **On-chain resolution transaction:** [PolygonScan][onchain-resolution]

The market page records two Yes proposals, two disputes, and a final Yes outcome.[^market] The resolution transaction paid the first outcome slot, corresponding to Yes, on March 25 at 00:21 UTC.[^onchain-resolution]

## The rule

The operative clause said:

> This market will resolve to "Yes" if the United States and Ukraine agree to any deal between February 2 and March 31, 2025, 11:59 PM ET, that explicitly involves Ukrainian rare earth elements.

The rule included exchanges involving U.S. aid, partnerships, future resource rights, mining rights, and other forms of rare-earth cooperation. It then added:

> An announcement of a deal will qualify regardless of if/when the deal is enacted.

The stated resolution source was official information from the U.S. and Ukrainian governments.[^market]

The rule did **not** require:

- a signature;
- legal enactment;
- ratification;
- completion of all implementation details; or
- performance of the agreement.

It also did not define:

- whether a preliminary or framework agreement was a "deal";
- whether unilateral government approval of a negotiated draft proved bilateral agreement;
- whether a deal that later collapsed still qualified;
- whether the market could resolve before March 31 if the alleged agreement remained disputed; or
- what degree of official confirmation was required from each government.

## What happened

### February 25-26: a framework was reported as agreed

Bloomberg reported on February 25 that Ukraine had agreed with the United States to jointly develop natural resources. It described the instrument as a framework agreement and said Ukraine's cabinet was expected to recommend that it be signed.[^bloomberg]

The Washington Post separately reported that Ukraine and the United States had agreed to a framework for a minerals deal, citing a Ukrainian official and another person familiar with the matter.[^washington-post]

On February 26, Ukraine's Cabinet of Ministers issued an official order that:

1. approved the draft bilateral agreement establishing the rules and conditions of a reconstruction investment fund; and
2. authorized First Deputy Prime Minister Yuliia Svyrydenko or Foreign Minister Andrii Sybiha to sign it.[^cabinet-order]

This is the strongest evidence for Yes. It is official Ukrainian government information showing that a negotiated agreement text had advanced to approval and authorization for signature.

### February 28: the document was not signed

The planned White House signing did not occur after the contentious meeting between Donald Trump and Volodymyr Zelenskyy. The parties continued to describe a minerals agreement as something that remained to be signed.[^ap-oval-office]

That fact supports No only if "agree to any deal" is interpreted to require a final, presently operative agreement. The written rule expressly said that signature and enactment were unnecessary, so absence of signature was not independently sufficient for No.

### A related Polymarket market had already resolved No

Polymarket also operated `Ukraine agrees to Trump mineral deal by Friday?`, covering February 25-28. Its substantive rule was nearly identical:

- the parties had to "agree to any deal";
- an announcement qualified regardless of enactment; and
- official U.S. and Ukrainian information controlled.

That market resolved No without a dispute.[^friday-market]

This creates a direct internal contradiction. The evidence later used to support Yes in the before-April market was the same February framework evidence available during the by-Friday market. The two contracts therefore treated the same event under materially the same rule as both No and Yes.

### March 22-23: a late Yes proposal and a last-minute clarification

A detailed contemporaneous reconstruction by trader `@Domahhhh` and a separate account by Tenadome report that a major Yes holder proposed Yes on March 22, when the market was still open and trading at a low probability. The proposal was disputed and escalated to an UMA token-holder vote.[^domah][^tenadome]

Both accounts report that Polymarket issued its clarification at 11:58 p.m. UTC on March 23, approximately two minutes before the vote commitment period ended. Tenadome summarizes the clarification as saying that it was too early for the market to resolve and that the result was not yet Yes.[^tenadome]

This timing mattered. UMA uses a commit-and-reveal process. Once votes had been committed, voters could not simply change them in response to the clarification. They could reveal the committed votes or abstain from revealing.[^tenadome]

### March 24-25: Polymarket allowed the contrary vote to finalize

The same contemporaneous accounts report that shortly before the reveal period ended, Polymarket issued a further notice indicating that it would allow the market to resolve in line with the UMA vote. The vote favored Yes, and the market finalized Yes at 00:21 UTC on March 25.[^domah][^tenadome][^onchain-resolution]

The finalization occurred six days before the stated event deadline. Even if the February framework did not qualify, Polymarket could have allowed the market to remain open through March 31 rather than converting an unresolved factual dispute into a final Yes.

### March 26: Polymarket acknowledged the breakdown

A screenshot published by Wu Blockchain preserves a statement from a Polymarket representative, Tanner:

> This market resolved against the expectations of our users and our clarification. Unfortunately, because this wasn't a market failure, we are not able to issue refunds.

The statement called the event unprecedented, said Polymarket and UMA had been working in internal "war rooms," and promised better systems, monitoring, clearer rules, and a more defined and timely clarification system.[^wu-post][^polymarket-response]

That is an admission that the process produced a result Polymarket did not intend or expect. Calling it "not a market failure" appears to have been a classification used to deny refunds, not a substantive defense that the process worked correctly.

## The allegation against Polymarket

### 1. The market resolved contrary to Polymarket's own clarification

Polymarket told voters the market was too early and was not yet Yes. The final result was Yes. Polymarket then expressly acknowledged that the outcome contradicted its clarification.[^tenadome][^polymarket-response]

This establishes a failure in the venue's resolution stack regardless of whether the underlying February framework ultimately should have qualified.

### 2. Polymarket issued the clarification too late

A clarification delivered approximately two minutes before the end of a commit period cannot reliably guide votes already committed. Polymarket's later promise to build a more timely clarification system implicitly recognized that defect.[^tenadome][^wu-post]

The timing also created severe informational asymmetry for traders. Market participants could see a platform clarification pointing away from Yes while the committed UMA vote was not yet visible.

### 3. Polymarket applied materially identical rules inconsistently

The February 25-28 market resolved No. The before-April market resolved Yes based on the February framework. Both rules said an announced deal qualified without enactment.[^market][^friday-market]

This is not a subtle difference between market titles. It is an inconsistent answer to whether the February framework constituted an agreed deal.

### 4. Concentrated oracle voting overrode the venue's interpretation

Contemporaneous reports attributed a large share of voting power to a small number of UMA holders. The exact descriptions conflict:

- Wu Blockchain reported five million tokens across three accounts, approximately 25% of votes.[^wu-post]
- CoinDesk focused on `BornTooLate.eth`, reporting approximately 1.3 million UMA and describing the address as a top-five governance staker.[^coindesk]
- Tenadome disputed the "governance attack" characterization and argued that ordinary recurring UMA voters ignored the clarification to avoid losses or slashing on already committed votes.[^tenadome]

The evidence supports a concentration and incentive-design concern. It does not conclusively establish that one actor bought tokens specifically to corrupt this market, controlled every cited address, traded the underlying Polymarket contract, or made a substantial profit from the result.

## Polymarket and UMA's defense

### Polymarket's explicit defense

Polymarket's public position had two parts:

1. the result contradicted its clarification and was unprecedented; but
2. it was not classified as a "market failure," so refunds were unavailable.[^polymarket-response]

The implicit procedural defense is that the contract was resolved through the published UMA mechanism and that the final token-holder vote was binding. Polymarket's later decision to allow the result to follow the UMA vote is consistent with that position.[^tenadome]

This explains why Polymarket did not reverse the payout. It does not explain why a binding result contrary to the venue's own clarification should not count as a failure.

### The strongest substantive defense of Yes

Yes has a stronger rule-based defense than most reporting about the controversy acknowledges:

1. The rule required agreement, not signature.
2. It expressly said an announcement qualified regardless of enactment.
3. Major reporting on February 25 said the parties had agreed to a framework.
4. Ukraine's Cabinet officially approved the draft and authorized its signature on February 26.[^bloomberg][^washington-post][^cabinet-order]

On a literal and broad reading of "agree to any deal," the February framework could satisfy the market even though the contemplated signature did not occur.

### The strongest substantive argument for No or Too Early

The February document was described as a framework or draft. Implementation details remained to be negotiated, the planned signing failed, and the parties continued speaking as though an operative agreement had not yet been concluded.[^bloomberg][^ap-oval-office]

Ukraine's Cabinet order proved that Ukraine approved a draft and authorized signature. It did not by itself prove that both governments regarded the draft as a concluded bilateral deal. Under this narrower interpretation, the correct result on March 23 was Too Early, followed by No if no qualifying agreement was reached by March 31.

Polymarket adopted this narrower interpretation in its clarification, but too late to guide the committed UMA votes effectively.[^tenadome]

## Assessment

### Was the final Yes outcome clearly false?

**No.**

The fact that the agreement was not signed until April 30 does not decide this market. Signature was expressly unnecessary. The February reporting and Ukrainian Cabinet order provide a serious basis for finding that the parties had agreed to a framework deal.[^market][^cabinet-order]

Yes therefore cannot responsibly be described as having no factual or contractual support.

### Was Yes clearly the correct outcome?

**No.**

The rule did not define whether an approved framework or draft constituted a completed "deal." The failed signing and subsequent negotiations support the view that the parties had not yet reached the kind of agreement the market intended to measure.

Polymarket itself clarified that the market was too early and not yet Yes. Its almost identical by-Friday market had already resolved No.[^friday-market][^tenadome]

### Did Polymarket make a resolution-process error?

**Yes, conclusively.**

The venue:

- issued its interpretation too late for normal voter response;
- allowed the opposite result to finalize;
- produced inconsistent outcomes across materially identical rules;
- acknowledged that the result contradicted its clarification;
- called the situation unprecedented; and
- promised systems intended to prevent recurrence.[^polymarket-response]

### Did Polymarket make a rule-drafting error?

**Yes.**

The decisive phrase, "agree to any deal," did not distinguish:

- political agreement from legal agreement;
- a framework from a completed deal;
- an approved draft from a bilaterally concluded instrument; or
- a deal that later collapsed from one that remained in force.

The no-signature clause broadened the trigger without supplying a substitute test for when negotiations became an agreement.

### Was this a proven governance attack?

**Not conclusively.**

Concentrated voting power and poor incentives clearly affected the process. Public sources disagree about the relevant wallets, token amounts, coordination, and motive. CoinDesk reported that no participant appeared to earn a large payoff relative to the alleged cost of accumulating the UMA position.[^coindesk]

The documented failure does not depend on proving malicious manipulation. Negligence, untimely clarification, conflicting incentives, and an under-specified rule are sufficient to explain the outcome.

### Overall classification

- **Resolution-process failure:** Yes
- **Rule-drafting failure:** Yes
- **Inconsistent related-market resolution:** Yes
- **Untimely clarification:** Yes
- **Final outcome error:** Indeterminate; Yes and Too Early/No each had material textual support
- **Governance attack:** Alleged, not conclusively established
- **Remediation failure:** Yes; Polymarket acknowledged the breakdown but denied refunds
- **Confidence:** High on platform/process failure; medium on whether Yes was substantively wrong

## Precise blocker to a conclusive outcome finding

The blocker is the rule's failure to define when negotiations become a "deal."

The factual record is reasonably clear:

- the parties negotiated a framework;
- press reports said they had agreed to it;
- Ukraine officially approved the draft and authorized signature;
- the planned signature did not occur;
- the parties continued negotiating; and
- a later agreement was signed on April 30.[^cabinet-order][^ap-oval-office][^final-agreement]

What is missing is a predetermined contractual rule assigning those facts to Yes, No, or Too Early. Polymarket attempted to supply that rule through a clarification only after votes had already been committed.

## Sources

### Primary

[^market]: Polymarket, [“Ukraine agrees to Trump mineral deal before April?”][market]. Contains the original rule, proposal/dispute sequence, final Yes outcome, and current volume.

[^api]: Polymarket Gamma API, [event record for the before-April market][api]. Preserves the rule, dates, volume, contract identifiers, and final prices.

[^friday-market]: Polymarket, [“Ukraine agrees to Trump mineral deal by Friday?”][friday-market]. Contains the materially similar February 25-28 rule and final No outcome.

[^cabinet-order]: Cabinet of Ministers of Ukraine, [Order No. 164-r approving the draft bilateral agreement and authorizing signature][cabinet-order], February 26, 2025.

[^final-agreement]: Cabinet of Ministers of Ukraine, [“Ukraine and the United States sign Economic Partnership Agreement and establish the Reconstruction Investment Fund”][final-agreement], May 1, 2025. Records the April 30 signature.

[^onchain-resolution]: PolygonScan, [resolution transaction for question `0x96bfe...3822`][onchain-resolution], March 25, 2025. The transaction records a Yes payout vector.

[^wu-post]: Wu Blockchain, [X post reproducing Polymarket's Discord statement][wu-post], March 26, 2025. Its attached screenshot preserves Tanner's statement that the result contradicted Polymarket's clarification and describes planned remediation.

### Contemporaneous reporting and reconstruction

[^bloomberg]: Bloomberg via BNN Bloomberg, [“Ukraine to Agree With US on Terms for Minerals Deal”][bloomberg], February 25, 2025. Reports that Ukraine agreed with the United States on a framework and that cabinet approval and signature were expected.

[^washington-post]: The Washington Post, [“Ukraine and U.S. agree to framework for minerals deal, Ukrainian official says”][washington-post], February 25, 2025.

[^ap-oval-office]: Associated Press, [“Zelenskyy leaves White House without signing minerals deal after Oval Office blowup”][ap-oval-office], February 28, 2025.

[^polymarket-response]: crypto.news, [“Polymarket suffers governance attack due to UMA whale intervention”][polymarket-response], March 26, 2025. Reproduces Polymarket's Discord response and its no-refund position. The article's characterization of the incident as a proven attack is stronger than the evidence established here.

[^coindesk]: CoinDesk, [“A Contentious Ukraine Bet Leads to Clash Between Polymarket, UMA Communities”][coindesk], March 26-27, 2025. Reports UMA concentration, limited apparent trading profits, Polymarket's response, and competing characterizations of the incident.

[^tenadome]: Tenadome, [archived thread disputing the governance-attack characterization][tenadome], March 26, 2025. Provides the detailed commit/reveal and clarification timeline. This is a participant account, not an official record.

[^domah]: `@Domahhhh`, [archived investigation of the proposal and vote sequence][domah], March 27, 2025. Documents the sister-market inconsistency, reported clarification timing, and Yes argument. This is an advocacy-oriented trader reconstruction and is used cautiously.

[market]: https://polymarket.com/event/ukraine-agrees-to-give-trump-rare-earth-metals-before-april
[api]: https://gamma-api.polymarket.com/events?slug=ukraine-agrees-to-give-trump-rare-earth-metals-before-april
[friday-market]: https://polymarket.com/event/ukraine-agrees-to-trump-mineral-deal-by-friday
[cabinet-order]: https://www.kmu.gov.ua/npas/pro-pidpysannia-dvostoronnoi-uhody-pro-vstanovlennia-pravyl-ta-umov-investytsiinoho-fondu-t260225
[final-agreement]: https://www.kmu.gov.ua/en/news/ukraina-i-ssha-pidpysaly-uhodu-pro-ekonomichne-partnerstvo-ta-stvorennia-investytsiinoho-fondu-vidbudovy
[onchain-resolution]: https://polygonscan.com/tx/0x0f0d0bd28dfae70d35269f883986e1780b58398fffe34f72a30aa3e998c807ea
[wu-post]: https://x.com/WuBlockchain/status/1904772495649235117
[bloomberg]: https://www.bnnbloomberg.ca/investing/commodities/2025/02/25/ukraine-to-agree-with-us-on-terms-for-minerals-deal/
[washington-post]: https://www.washingtonpost.com/politics/2025/02/25/ukraine-minerals-deal-trump-zelensky/
[ap-oval-office]: https://apnews.com/article/eebdf97b663c2cdc9e51fa346b09591d
[polymarket-response]: https://crypto.news/polymarket-suffers-governance-attack-due-to-uma-whale-intervention/
[coindesk]: https://www.coindesk.com/markets/2025/03/26/polymarket-suffers-uma-governance-attack-after-rouge-actor-becomes-top-5-token-staker
[tenadome]: https://threadreaderapp.com/thread/1904789723383529517.html
[domah]: https://threadreaderapp.com/scrolly/1905258165777596812
