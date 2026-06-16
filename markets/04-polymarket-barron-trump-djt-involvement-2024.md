# Polymarket: Was Barron involved in $DJT?

## Bottom line

**Finding: This was a real Polymarket resolution-governance and transparency failure, but it is not proven that the market paid the wrong side under its written rules. Confidence: high on the platform-level failure; low on any conclusive factual answer about Barron's involvement.**

The market asked whether a preponderance of evidence suggested that Barron Trump was involved in the **creation** of the Solana token `$DJT`. Its rules expressly assigned that determination to UMA, using evidence available by 12 p.m. ET on June 23, 2024.[^market]

The oracle process received two `No` proposals, both of which were disputed. UMA's final disputed resolution was `No`, and the market settled that way.[^market] Calling this "UMA deciding No twice" would be inaccurate: the first two entries were optimistic-oracle proposals, while the final disputed answer came through UMA's adjudication process.

After finalization, Polymarket publicly said UMA was wrong and later said it was conclusive that Barron had been involved "in some way." It disclosed neither the supporting evidence nor how that broader phrase satisfied the narrower contractual requirement of involvement in **creation**.[^wrong-statement][^refund-statement][^coindesk-final]

That contradiction is the established failure. Polymarket had:

- written a broad title but a narrower operative criterion;
- listed a question whose decisive evidence was likely private, anonymous, or difficult for tokenholders to authenticate;
- made UMA the named decision-maker;
- finalized the market to UMA's answer; and
- then asserted a different factual answer without publishing evidence tied to the exact rule and cutoff.

The public record does not establish that UMA's `No` was wrong. The `Yes` case included relevant first-person and source-based claims, but their independence, authenticity, and precise connection to token creation were not publicly verifiable. The `No` case therefore had a rational basis. Conversely, a preponderance standard does not require official confirmation or definitive proof, so the absence of a Barron statement or verified wallet does not make `No` conclusively correct.

Polymarket left the official `No` payout in place and separately reimbursed `Yes` holders. That reimbursement was a reasonable loss-mitigation measure, not itself the failure. It was not a reversal or a $1-per-share `Yes` payout, and Polymarket did not publicly explain the exact calculation.[^refund-statement][^refund-transaction]

The most defensible final characterization is therefore:

- **Contractual misresolution:** not established.
- **Factual answer:** indeterminate from the public record.
- **Oracle corruption or manipulation:** not established.
- **Platform failure:** established, because Polymarket's market design and later unsupported repudiation of its own designated resolver produced two incompatible official accounts of what the market was supposed to mean and whether it had resolved truthfully.

## Market details

- **Venue:** Polymarket
- **Question:** `Was Barron involved in $DJT?`
- **Created:** June 20, 2024
- **Evidence cutoff:** June 23, 2024 at 12 p.m. ET
- **Final resolution:** No
- **Finalized:** June 26, 2024 at 00:20 UTC
- **Reported volume:** approximately $1.14 million
- **Market page:** [Polymarket][market]
- **Primary metadata:** [Polymarket Gamma API][api]

The Polymarket page records this resolution sequence:

1. Outcome proposed: No
2. Disputed
3. Outcome proposed: No
4. Disputed
5. Final outcome: No

The first and third entries were proposals submitted to the optimistic oracle, not two final UMA rulings. After the disputes, UMA's adjudication produced the final `No` answer. The page and API continue to record `No` as the official outcome.[^market][^api][^adapter]

## The rule

The operative test was whether:

> a preponderance of evidence suggests that Barron Trump was involved in the creation

of `$DJT`. The rule otherwise required No. It said UMA would make the determination using all evidence available as of noon ET on June 23.[^market]

The title, `Was Barron involved in $DJT?`, was broader than that operative test. A trader reading only the title could reasonably understand later promotion, distribution, advice, or wallet activity as sufficient. Under the detailed rule, those acts mattered only if they established involvement in **creation**. The detailed rule controlled the settlement, but the mismatch became material when Polymarket later defended `Yes` by saying Barron was involved merely "in some way."[^refund-statement]

This was not a market requiring:

- a statement from Barron;
- definitive proof;
- proof beyond a reasonable doubt; or
- official Trump campaign involvement.

It was a more-likely-than-not evidentiary test. But the rule left several decisive questions undefined:

- What acts counted as involvement in "creation"?
- Did promotion, distribution, funding, wallet management, or giving advice count?
- What did "preponderance of evidence suggests" mean in practice?
- Did anonymous reporting count, and with what weight?
- Could private evidence unavailable to UMA voters count?
- How should screenshots be authenticated?

These omissions were material because almost every disputed fact depended on anonymous sources, interested participants, or screenshots whose identities could not be publicly verified.

Not every omitted evidentiary detail was necessarily a drafting defect. The rule deliberately delegated judgment to UMA, and open-textured standards normally require a fact-finder to weigh credibility. The deeper design problem was using that standard for a question where the best evidence was likely private while providing no transparent way to reconcile private platform knowledge with public oracle adjudication.

## A separate Barron market

Polymarket also operated a different market titled `Did Barron Trump launch $DJT?`.[^launch-market]

That sibling market required definitive evidence made public by 11:59 p.m. ET on June 23 and resolved No. It should not be conflated with this case:

- `Did Barron Trump launch $DJT?` required definitive public evidence of direct launch involvement.
- `Was Barron involved in $DJT?` required only a preponderance concerning involvement in creation.

The two No results are not inherently inconsistent because the evidentiary standards differed. The controversy documented here is Polymarket's repudiation of UMA's answer in the broader, lower-threshold market.

## What evidence existed by the cutoff

### Pirate Wires reported that Barron was "spearheading"

On June 17, Pirate Wires posted that, based on conversations, Trump was launching an official Solana token and that Barron was "spearheading."[^pirate-wires]

This was evidence in favor of Yes. It was a direct public assertion by a media outlet claiming source conversations.

Its limitations were also substantial:

- the sources were not identified;
- the underlying material was not published;
- "spearheading" was not broken down into specific acts;
- the claim that the token was an official Trump launch remained unconfirmed; and
- it was unclear whether the source chain was independent from Shkreli and his associates.

### ZachXBT established Shkreli's connection to the token

Blockchain investigator ZachXBT publicly documented that Shkreli contacted him shortly after he submitted evidence for Arkham's bounty identifying the creator of `$DJT`. Shkreli then announced that he was the creator.[^zach-thread][^coindesk-june25]

This materially strengthened the proposition that Shkreli had first-hand knowledge of the token. It did not independently prove his separate claim about Barron.

One screenshot in ZachXBT's thread showed Shkreli telling ZachXBT that he had created the token with Barron and possessed more than 1,000 pieces of evidence.[^zach-thread] The screenshot establishes that Shkreli made the claim. It is not itself corroboration of the claim, and Shkreli did not publish the promised body of evidence before the cutoff.

### Shkreli publicly claimed Barron was part of the project

Shkreli said in an X Spaces discussion that Barron was among a team of approximately 40 to 50 people involved with the token. Reporting also quoted him as saying that he and Barron were friends and that Barron wanted to make money.[^nymag][^newsweek]

Because Shkreli was involved in creating the token, his statement was not mere outside speculation. It was relevant first-person testimony.

Its weight was reduced by:

- his financial and reputational interest in the token and the surrounding wagers;
- the absence of the extensive evidence he claimed to possess;
- the lack of confirmation from Barron or an authenticated representative; and
- the lack of independently verified communications or wallet records tying Barron to creation.

Shkreli's securities-fraud history was relevant to credibility, but it was not by itself a reason to disregard everything he said. The more important problem was that his Barron allegation remained materially uncorroborated.

### The `BT` screenshot was suggestive but unauthenticated

On June 20, Shkreli posted a screenshot of a conversation with a contact saved as `BT`. The contact discussed connecting the correct wallet, liquidity-provider wallets, fees, and whether the coin had a tax.[^bt-screenshot]

If `BT` was Barron Trump and the screenshot was authentic, the exchange would be meaningful evidence of operational involvement with the token.

The public screenshot did not establish:

- that `BT` was Barron Trump;
- when the underlying conversation occurred;
- that the coin under discussion was `$DJT`;
- that the image had not been edited; or
- whether the conduct occurred during creation rather than after launch.

DL News reported that these same uncertainties were debated by UMA voters.[^dlnews-vote]

### Mike Solana defended his reporting

Mike Solana, the founder of Pirate Wires, said on a podcast that he was as certain as he could be that Barron was involved. He described the involvement as including creation and, at minimum, distribution and promotion.[^dlnews-vote]

This was the strongest publicly reported defense of Yes apart from Shkreli's own account. It suggested that Pirate Wires believed it had information beyond Shkreli's public claims.

But the underlying sources and evidence were not made available to UMA voters. Solana later criticized a system in which people without private insight voted on a question involving largely private information.[^solana-criticism] That criticism identified a real design problem, but it did not give voters access to the missing information.

### Evidence supporting No

By the cutoff:

- Barron had not publicly confirmed involvement.
- The Trump campaign had not officially confirmed the token or Barron's role.
- No wallet had been publicly and reliably attributed to Barron.
- The public screenshots did not authenticate `BT`.
- Shkreli had not produced the extensive supporting material he claimed to possess.
- Contact between project participants and Barron, even if established, would not necessarily prove involvement in creation.

CoinDesk reported on June 24 that Yes advocates were relying largely on Shkreli's word and that neither Barron nor the campaign had made a public statement.[^coindesk-june24]

DL News reported that an insider with direct knowledge of campaign decisions said the campaign was not involved. The Trump campaign itself had not publicly answered the allegation.[^dlnews-vote][^the-block] That did not rule out a private project involving Barron, but it weakened claims that `$DJT` was an official Trump effort.

## Material published after the cutoff

Evidence published after noon ET on June 23 could not properly change the answer unless it merely authenticated material already available by the cutoff and the rule permitted that use. The rule did not explain how later verification should be treated.

On June 27, Shkreli posted another screenshot in which an unidentified Telegram account said lawyers were discouraging Barron from speaking and later said Barron was no longer allowed to do anything with the token.[^post-cutoff-screenshot]

That screenshot:

- was posted four days after the cutoff;
- came from a deleted or unidentified account;
- did not authenticate its author's access to Barron; and
- still did not establish the exact role Barron allegedly played in creation.

Polymarket's June 28 assertion that involvement was conclusive was also after the cutoff and was a conclusion, not disclosed evidence.[^refund-statement]

## UMA's decision and defense

The optimistic oracle received two `No` proposals, and each was disputed. The final adjudicated answer was `No`.[^market] The distinction matters: proposers initially assert an answer; they are not themselves "UMA decisions." The disputed process is what supplied the final authoritative result.

UMA founder Hart Lambur told DL News that he believed voters acted honestly and that No was the "least bad answer" to an ambiguous question. He identified two separate interpretive problems:

1. voters had to decide what the market meant by a preponderance of evidence; and
2. they had to determine whether enough such evidence was publicly available at the relevant time.[^dlnews-vote]

The UMA discussion reflected the central distinction in the case. One participant reportedly believed there was enough evidence that key people had been in contact with Barron, but not enough that Barron had participated in **creating** the token.[^dlnews-vote]

That is a coherent defense of `No`. The contract did not ask whether Barron knew the creators, discussed the token, promoted it, or became involved later. It asked whether the evidence more likely than not showed involvement in creation.

There is no sourced basis in this case for alleging a governance attack, corrupt vote, or whale manipulation. Disagreement with the evidentiary judgment is not evidence that the oracle process was compromised.

## The allegation against Polymarket

### 1. Polymarket's official positions became irreconcilable

The rule expressly said UMA would determine whether Barron was involved. After UMA returned No, Polymarket publicly said:

> We firmly believe that UMA got this resolution wrong.

It promised a near-term solution in order to uphold market integrity and pricing.[^wrong-statement]

This is direct evidence that Polymarket believed its specified resolution process had produced the wrong factual answer. It is not, by itself, proof that UMA misapplied the written rule.

### 2. Polymarket did not substantiate its competing conclusion

Two days later, Polymarket called Barron's involvement conclusive but did not publish evidence supporting that conclusion.[^refund-statement][^coindesk-final]

That omission prevents an independent finding that the market should have resolved `Yes`. The market was explicitly an evidence-weighing exercise. Announcing a different conclusion does not demonstrate that an evidence-based resolution was wrong.

Without the material Polymarket relied on, traders could not assess:

- whether the evidence existed by the June 23 cutoff;
- whether it was authentic;
- whether it concerned creation rather than later involvement; or
- whether it outweighed the weaknesses in the public Yes case.

### 3. Polymarket's explanation did not match the operative criterion

The final statement said it was conclusive that Barron was involved "in some way."[^refund-statement]

The contract required involvement in the **creation** of `$DJT`. "In some way" could include later promotion, holding tokens, contact with the team, or attempted distribution. None necessarily satisfied the written criterion.

Polymarket may have intended its statement as shorthand for creation involvement. Because it did not identify the conduct or evidence, the statement did not establish that the market's narrower test was met.

### 4. The reimbursement mitigated losses but did not resolve the contradiction

Polymarket did not replace the official No result with Yes. No shares remained the winning shares, while Polymarket separately said it would refund Yes holders.[^market][^refund-statement]

The commonly repeated description that Polymarket "refunded both sides" is inaccurate:

- No holders received the ordinary benefit of the No resolution.
- Polymarket separately reimbursed Yes holders.
- The reimbursement was not a Yes winning payout of $1 per share.
- The public statement did not specify the precise eligibility cutoff or calculation.

The reimbursement was distributed in a separate USDC transaction totaling approximately **$95,106.26** among 133 addresses.[^refund-transaction] Individual payments show its nature:

- One address bought **847.264703 Yes shares** for approximately **$190.91** and received **$188.3673**, not the **$847.264703** it would have received from a $1-per-share Yes payout.[^refund-example-large]
- Another bought **33.333332 Yes shares** for approximately **$10.00** and received **$9.90**, not **$33.333332**.[^refund-example-small]

The payments therefore reimbursed some measure of purchase cost or loss rather than treating Yes as the winner. The examples do not prove that every eligible holder received a complete return of principal. Small differences from recorded purchase cost, along with lower payments to some late buyers, suggest that Polymarket applied an eligibility snapshot, netting, fees, or another adjustment that it did not publicly explain.

The payment mitigated harm to Yes holders and was not itself an improper act. Its relevance is evidentiary: it confirms that Polymarket lacked confidence in the official result. The remaining criticism is narrower. Polymarket did not disclose the remedy's formula or explain a general policy for comparable cases.

### 5. The resolution architecture did not produce one authoritative public answer

Polymarket had made UMA authoritative but evidently retained a substantive view of the correct answer. The rule did not say what would happen when those judgments diverged.

The result was three incompatible messages:

- the contract said UMA would determine the answer;
- UMA and the market page said No; and
- Polymarket said Yes was conclusive enough to compensate losing Yes holders.

That is a resolution-governance failure even if Polymarket privately possessed reliable evidence. A prediction market can intentionally make an oracle final, or it can reserve a transparent review power. The failure here was not simply the absence of an appeal. It was that the venue publicly repudiated the final answer without supplying either auditable evidence or a pre-announced framework that explained the status of its contrary judgment.

The verified UMA adapter also included emergency administrative controls before final CTF resolution.[^adapter] The public record does not show that Polymarket had reached its contrary conclusion in time to use them, so it would be speculative to accuse Polymarket of knowingly allowing a result it already considered wrong to finalize. By the time Polymarket publicly objected, the market had already finalized.[^market][^wrong-statement]

## Polymarket's defense

### Explicit defense

Polymarket did not defend the official `No` result. Its public position was that UMA had resolved the market incorrectly, that prediction markets must resolve to truth by the best means available, and that Barron's involvement was conclusive. It reimbursed `Yes` holders and said it was improving its oracle and resolution methodology.[^wrong-statement][^refund-statement]

The strongest defense of Polymarket's conduct, as distinct from its substantive `Yes` claim, is:

1. Polymarket possessed or trusted information unavailable to UMA voters.
2. The rules had transparently designated UMA, whose final answer became the contractual settlement.
3. By the time Polymarket publicly objected, the on-chain result had finalized.
4. Reimbursing `Yes` holders mitigated the harm without taking the ordinary `No` payout away from traders who had relied on the written process.
5. Publicly acknowledging the disagreement and promising process improvements was more transparent than concealing it.

The first, third, and fourth points are inferences from the sequence and the remedy; Polymarket did not publish a full technical explanation. The adapter had emergency controls before final resolution, but there is no evidence that Polymarket had reached its contrary view before those controls ceased to be useful.[^adapter]

### Strongest substantive defense of Yes

Yes was not baseless. Before the cutoff:

- Pirate Wires said Barron was spearheading the project.
- Shkreli, whose involvement in the token was independently exposed, said he created it with Barron.
- Shkreli posted a conversation with `BT` discussing wallets, liquidity, fees, and a token tax.
- Mike Solana said his reporting sources gave him very high confidence and specifically referred to creation, distribution, and promotion.[^pirate-wires][^zach-thread][^bt-screenshot][^dlnews-vote]

The market required a preponderance, not definitive proof. A fact-finder could reasonably give enough weight to these mutually reinforcing claims to choose Yes.

### Why the substantive defense remains insufficient

The evidence was not demonstrably independent or authenticated:

- Pirate Wires did not disclose its sources.
- Shkreli was both a participant and an interested promoter.
- `BT` was only a contact label.
- No public wallet or communication was verified as Barron's.
- The alleged 1,000 pieces of evidence were not released.
- Polymarket never identified what made the case conclusive.

Polymarket's private confidence therefore cannot establish, for outside reviewers, that `Yes` was the required contractual answer. To do so, it would need to disclose evidence that existed by the cutoff and showed involvement in creation, or at least explain enough about that evidence to make the conclusion auditable.

## Assessment

### Was UMA's No result clearly wrong?

**No.**

The public Yes case was substantial enough to create a genuine dispute, but it remained a collection of source assertions and unauthenticated screenshots. Shkreli's proven knowledge of the project made his testimony relevant; it did not make every additional assertion more likely than not true.

`No` was a reasonable application of the creation criterion to the evidence voters could inspect. That does not prove it was the only reasonable application.

### Was No clearly the factual truth?

**No.**

Shkreli and Solana may have had genuine first-hand or source-based knowledge. The `BT` exchange, if authentic and correctly attributed, would support operational involvement. The missing evidence may exist.

The record supports uncertainty, not a conclusive finding that Barron had no involvement. Nor does the lack of official confirmation defeat `Yes`: a preponderance can be established through credible testimony and circumstantial evidence.

### Did Polymarket establish that Yes was correct?

**No.**

Polymarket announced a conclusion without publishing its basis. It also described involvement "in some way," not necessarily involvement in creation.

Its statement is evidence of Polymarket's belief. It is not evidence sufficient to audit or prove the market outcome.

### Did the oracle process violate the written market procedure?

**Not on the evidence available.**

The rules designated UMA to make the evidentiary determination. The market received proposals and disputes, UMA supplied the final answer, and the CTF market settled to that answer. No evidence establishes vote manipulation, corruption, or departure from the encoded process.

This is why it is too strong to describe the case as a proven "wrong payout." Under the contract as written, `No` was the authoritative result.

### Did Polymarket nevertheless make a platform-level resolution error?

**Yes.**

The confirmed error was in market and resolution governance:

- The broad title and narrower creation criterion invited different understandings of the question.
- The market depended heavily on private or anonymously sourced evidence that a public token-holder vote could not readily authenticate.
- Polymarket later repudiated its designated resolver but did not publish evidence satisfying the exact creation criterion and cutoff.
- It left the official `No` result in place while publicly telling users that the truth was effectively `Yes`.

From a trader's perspective, UMA was part of Polymarket's chosen resolution stack. Outsourcing adjudication does not remove Polymarket's responsibility for designing a market that its chosen stack can resolve credibly. At the same time, Polymarket's disagreement does not retroactively prove that the oracle answer was contractually wrong.

### Was the rule itself defective?

**Materially weak, but not every ambiguity was an error.**

The phrase "preponderance of evidence suggests" was imprecise, "involved in creation" was undefined, and the title was broader than the rule. The rule also gave no guidance on anonymous sources or authentication even though those issues were predictable for this question.

However, a rule need not contain a complete evidence code, and designating UMA to exercise judgment was itself a disclosed term. The strongest criticism is not simply that the rule was subjective or lacked an appeal. It is that Polymarket chose an evidence-weighing oracle for a question whose decisive information was likely private, then relied on undisclosed information to reject that oracle's conclusion.

### Was the reimbursement itself a failure or a full reversal?

**No.**

The official market remained `No`. Polymarket reimbursed `Yes` holders separately rather than paying their shares as winners. There is no sourced basis for describing this as a two-sided market cancellation. The reimbursement was a defensible mitigation once Polymarket had lost confidence in the outcome. The narrower transparency problem is that the accessible public record does not establish its exact formula or eligibility policy.

### Overall classification

- **Wrong contractual payout:** Not established
- **Wrong factual answer:** Indeterminate
- **Oracle corruption or manipulation:** Not established
- **Encoded oracle procedure followed:** Yes, on the available record
- **Resolution-governance failure:** Yes
- **Platform/oracle contradiction:** Yes
- **Unsupported post-final platform claim:** Yes
- **Material title/rule mismatch:** Yes
- **Rule and market-design weakness:** Yes
- **Reimbursement as mitigation:** Reasonable, but formula not publicly explained
- **Refund of both sides:** No; Yes holders were separately reimbursed after No won
- **Yes paid as winner:** No; payments were far below $1 per Yes share
- **Confidence:** High on the platform-level contradiction and design failure; low on a conclusive `Yes` or `No` factual answer

## Final assessment

Polymarket made a real mistake, but the mistake must be described precisely.

It is **not established** that UMA violated the rule, that `Yes` was the required answer, or that `No` holders were paid contrary to the disclosed contract. The final `No` was produced by the decision-maker named in the rule, through the expected dispute process, and had a rational evidentiary basis.

The established failure was that Polymarket created a market its chosen resolver could not resolve to the venue's own satisfaction, then publicly declared the resolver wrong without supplying auditable evidence that met the market's narrower creation criterion and cutoff. The venue's official settlement remained `No`, while the venue's public statement said the underlying truth was conclusively on the other side. That is a serious failure of resolution design, rule communication, and post-resolution transparency even though a substantive misresolution cannot be proven.

The refund should be treated as remediation, not as part of the offense. It reduced the loss to `Yes` holders while preserving the contractual payout to `No` holders. Its unexplained calculation is a secondary transparency issue.

For a public tracker, the concise verdict should be:

> **Confirmed platform-level resolution-governance failure; unproven wrong contractual outcome.** Polymarket's broad title, narrower rule, unsuitable evidence environment, and unsupported post-final repudiation of UMA created an irreconcilable split between the official result and the platform's stated view of the truth. The public record is insufficient to determine conclusively whether Barron was involved in creating `$DJT`.

## Precise blocker to a conclusive factual finding

The blocker is missing and unauthenticated evidence.

A conclusive assessment would require at least one of the following:

- the source material underlying Pirate Wires' report;
- authentication that `BT` was Barron and that the conversation concerned `$DJT`;
- verified wallet or transaction evidence tying Barron to creation;
- the evidence Shkreli claimed to possess;
- a statement from Barron or an authenticated representative; or
- the evidence Polymarket relied on when it called involvement conclusive.

The timing of that evidence would also need to be established. Material first available after noon ET on June 23 could not straightforwardly determine this market under its written cutoff.

The public record does not disclose the exact eligibility snapshot, formula, or adjustments Polymarket used to reimburse Yes holders. That prevents a complete accounting of the remedy, but the on-chain amounts establish that it was a reimbursement rather than a Yes winning payout.

## Sources

### Primary

[^market]: Polymarket, [“Was Barron involved in $DJT?”][market]. Contains the rule, two No proposals, two disputes, final No outcome, and resolution time.

[^api]: Polymarket Gamma API, [market metadata for event `was-barron-involved-in-djt`][api]. Records market ID `502710`, approximately $1.14 million in volume, final prices, contract identifiers, and the No result.

[^adapter]: Polygon Blockscout, [verified `UmaCtfAdapter` contract used by Polymarket][adapter]. The published source includes `pause`, `flag`, and time-delayed `emergencyResolve` functions available before ordinary CTF finalization.

[^wrong-statement]: Polymarket, [X statement saying UMA's resolution was wrong][wrong-statement], June 26, 2024.

[^refund-statement]: Polymarket, [X statement calling involvement conclusive and announcing refunds for Yes holders][refund-statement], June 28, 2024.

[^refund-transaction]: Polygon Blockscout, [USDC reimbursement transaction `0x8037705f9ecfb375bb114318fed11aede3c8d001eabccbc5d66ae711b7479ac1`][refund-transaction], June 28, 2024. The Disperse.app transaction distributed 95,106.2647 bridged USDC among 133 recipients.

[^refund-example-large]: Polymarket Data API, [trades for address `0x0bb3ef70625830cc6df761e1ea03a76113ac10bd` in this market][refund-example-large]. Its three Yes purchases total 847.264703 shares and approximately $190.91; the reimbursement transaction sent the same address 188.3673 USDC.

[^refund-example-small]: Polymarket Data API, [trades for address `0x5c407bf7c5472a012cedb6cc3c74b2e6c475d4eb` in this market][refund-example-small]. It bought 33.333332 Yes shares at approximately $0.30 and received 9.90 USDC in the reimbursement transaction.

[^pirate-wires]: Pirate Wires, [original X report saying Barron was “spearheading” the token][pirate-wires], June 17, 2024.

[^zach-thread]: ZachXBT, [X thread documenting Shkreli's identification as the token creator and Shkreli's Barron claim][zach-thread], June 19, 2024. The attached screenshots preserve the underlying messages.

[^bt-screenshot]: Martin Shkreli, [X post containing the `BT` wallet and token screenshot][bt-screenshot], June 20, 2024.

[^solana-criticism]: Mike Solana, [X post criticizing the use of public voter speculation to decide private information][solana-criticism], June 26, 2024.

[^post-cutoff-screenshot]: Martin Shkreli, [X post containing a later Telegram screenshot][post-cutoff-screenshot], June 27, 2024. Included only to establish timing and the nature of post-cutoff material.

[^launch-market]: Polymarket, [“Did Barron Trump launch $DJT?”][launch-market]. This was a separate market with a definitive-public-evidence standard.

### Contemporaneous reporting

[^dlnews-vote]: DL News, [“Polymarket slams vote on Barron Trump, DJT token”][dlnews-vote], June 26-27, 2024. Reports UMA's rationale, Mike Solana's claims, the evidence debated by voters, and Hart Lambur's defense of No.

[^coindesk-june24]: CoinDesk, [“Biden Likely to Win Popular Vote, but Lose Presidency, Prediction Market Signals”][coindesk-june24], June 24, 2024. Contemporaneously records the two disputed No proposals, the absence of a Barron or campaign statement, and the reliance on Shkreli's account.

[^coindesk-june25]: CoinDesk, [“PoliFi Tokens Return to Business After Proof of DJT-Trump Link Fails to Materialize”][coindesk-june25], June 25, 2024. Reports that Shkreli's role was established but credible proof of Trump-family involvement had not materialized.

[^coindesk-final]: CoinDesk, [“Polymarket Says It's 'Conclusive' Barron Trump Was Involved in $DJT”][coindesk-final], updated June 28, 2024. Reports that Polymarket supplied no evidence for its conclusion and announced a refund for Yes holders.

[^the-block]: The Block, [“Polymarket contradicts UMA's resolution on Barron Trump's involvement with DJT token”][the-block], June 27, 2024. Preserves Polymarket's initial objection and the lack of a Trump campaign response.

[^nymag]: New York Magazine, [“Did Barron Trump Launch DJT Crypto With Martin Shkreli?”][nymag], June 21, 2024. Reviews Shkreli's claims and the absence of the extensive proof he said he possessed.

[^newsweek]: Newsweek, [“Is Barron Trump Behind Mysterious New DJT Coin? What We Know”][newsweek], June 20, 2024. Contemporaneously reports Shkreli's claim, his alleged team size, and the absence of a Barron statement.

[market]: https://polymarket.com/event/was-barron-involved-in-djt
[api]: https://gamma-api.polymarket.com/events?slug=was-barron-involved-in-djt
[adapter]: https://polygon.blockscout.com/address/0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74?tab=contract
[wrong-statement]: https://x.com/Polymarket/status/1805998648788173006
[refund-statement]: https://x.com/Polymarket/status/1806479362377814378
[refund-transaction]: https://polygon.blockscout.com/tx/0x8037705f9ecfb375bb114318fed11aede3c8d001eabccbc5d66ae711b7479ac1
[refund-example-large]: https://data-api.polymarket.com/trades?user=0x0bb3ef70625830cc6df761e1ea03a76113ac10bd&market=0x8fb1c85df2e64bedc411454f69267ae172a34d4c9b1693e7a768fc604c299ea&limit=10000&takerOnly=false
[refund-example-small]: https://data-api.polymarket.com/trades?user=0x5c407bf7c5472a012cedb6cc3c74b2e6c475d4eb&market=0x8fb1c85df2e64bedc411454f69267ae172a34d4c9b1693e7a768fc604c299ea&limit=10000&takerOnly=false
[pirate-wires]: https://x.com/PirateWires/status/1802825492405669930
[zach-thread]: https://x.com/zachxbt/status/1803240784436797871
[bt-screenshot]: https://x.com/MartinShkreli/status/1803824556827615721
[solana-criticism]: https://x.com/micsolana/status/1805788069649695173
[post-cutoff-screenshot]: https://x.com/MartinShkreli/status/1806130264558453089
[launch-market]: https://polymarket.com/event/did-barron-trump-launch-djt
[dlnews-vote]: https://www.dlnews.com/articles/defi/polymarket-slams-vote-on-barron-trump-and-djt-token/
[coindesk-june24]: https://www.coindesk.com/news-analysis/2024/06/24/biden-likely-to-win-popular-vote-but-not-presidency-prediction-market-signals
[coindesk-june25]: https://www.coindesk.com/markets/2024/06/25/polifi-tokens-return-to-business-after-proof-of-djt-trump-link-fails-to-materialize
[coindesk-final]: https://www.coindesk.com/markets/2024/06/27/polymarket-contradicts-its-oracle-service-in-rarity-for-prediction-market
[the-block]: https://www.theblock.co/post/302171/polymarket-contradicts-umas-resolution-on-barron-trumps-involvement-with-djt-token
[nymag]: https://nymag.com/intelligencer/article/barron-trump-djt-crypto-martin-shkreli.html
[newsweek]: https://www.newsweek.com/crypto-djt-barron-trump-martin-shkreli-1915147
