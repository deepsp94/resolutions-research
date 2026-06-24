# Kalshi: Cardi B Super Bowl halftime performance

## Bottom line

**Finding: Failure — a rule-design and contract-drafting failure, not an operational misgrade. The contract that actually governed on February 8, 2026 was internally self-contradictory about whether dancing counts as performing, so a ~$47.3M market could not produce a clean binary answer and was force-settled to the last traded price ($0.26 Yes / $0.74 No) under Rule 6.3(c). Kalshi later amended the contract to remove the ambiguity, effectively conceding the defect. Failure-resolved: Unresolved. Confidence: high.**

Kalshi listed a 2026 Super Bowl halftime market, `KXPERFORMSUPERBOWLB`, asking who would perform at the Big Game. Cardi B appeared during Bad Bunny's halftime show alongside Karol G, Young Miko, Jessica Alba, and Pedro Pascal. Reporting consistently describes her as dancing to the music and mouthing words, with no confirmed singing.[^cbs][^nbc] Kalshi did not settle her strike as a normal binary. It invoked its ambiguity process and settled to the last traded prices before trading was paused: **$0.26 for Yes holders and $0.74 for No holders.**[^kalshi-event][^cbs]

The decisive question is *which contract governed*. The version in force on February 8, 2026 — the `PERFORM` terms as archived January 11, 2026 — defined "performs" loosely and **contradicted itself**: its core criterion said a performer "Performs (including **dancing**, singing, DJ-ing, e.g.)," while its exclusion list said "**Dancing** or appearing on stage without singing/playing instruments" does NOT constitute a performance.[^terms-jan2026] A televised cameo of someone dancing and mouthing lyrics falls into the exact gap between those two clauses. The contract could not resolve itself, and Kalshi force-settled to market price.

Critically, the stricter language the prior version of this case file quoted — requiring the performer to "actively and perceptibly contribute to a musical performance by singing... rapping... DJ-ing, or conducting a live band" — is **not** the governing rule. It is the **post-event amendment**, certified to the CFTC on March 2, 2026, whose own cover letter lists "Change to Payout Criterion for clarity."[^terms-current][^cert-mar2026] Kalshi rewrote the definition *after* the Cardi B dispute. Settling a market under a self-contradictory rule, then amending the rule, is a drafting failure — not a defensible application of a clean written standard.

## Market details

- **Venue:** Kalshi
- **Series:** `KXPERFORMSUPERBOWLB`, "Who will perform at the Super Bowl"; event `KXPERFORMSUPERBOWLB-26`.[^kalshi-event]
- **Event:** Super Bowl LX halftime show (Bad Bunny), February 8, 2026.
- **Relevant strike:** Cardi B (individual market ticker since pruned from Kalshi's public API).
- **Governing contract (Feb 2026):** `PERFORM` terms as archived January 11, 2026; the governing CFTC certification predates the event (the next certification is the March 2, 2026 amendment).[^terms-jan2026][^cert-mar2026]
- **Settlement:** ambiguity force-settlement to last traded price under Rule 6.3(c): **$0.26 Yes, $0.74 No.**[^kalshi-event]
- **Market family volume:** approximately **$47.3 million** on Kalshi (vs. ~$10M on Polymarket).[^cbs]

## The rule that governed

The `PERFORM` terms in force on February 8, 2026 defined the Payout Criterion as whether `<performer>` performs (or it is announced they will perform) at `<event>` during the official event timeframe.[^terms-jan2026]

For purposes of the contract, "performs" meant (verbatim):
- "The performer appears on stage or in the official broadcast/stream AND
- Performs (**including dancing**, singing, DJ-ing, e.g.) AND
- Is either a scheduled performer OR makes a guest appearance during another artist's performance."[^terms-jan2026]

The same terms then listed what does NOT constitute a performance, including (verbatim): "**Dancing or appearing on stage without singing/playing instruments**" and "Performances that are cancelled or cut short before reaching 30 seconds."[^terms-jan2026]

Those two passages are in direct conflict. The affirmative clause folds dancing into the meaning of "performs"; the exclusion clause carves dancing-without-singing back out. The contract pointed to Rule 6.3(b) for determining payouts when an Expiration Value cannot be determined, and to Rule 6.3(d) for the Market Outcome Review Process.[^terms-jan2026]

That combination created the problem. Cardi B plainly appeared in the broadcast and visibly danced, placing her squarely in the contradiction: the affirmative clause would count her, the exclusion clause would not, and no reading of the broadcast resolved which clause controlled.

## What happened

Cardi B joined Bad Bunny's set on a porch-style stage with Karol G, Young Miko, Jessica Alba, and Pedro Pascal. Reporting describes her dancing to the music and mouthing words; it was not established that she sang or otherwise made an audible musical contribution, and she did not take a microphone.[^cbs][^nbc] Kalshi's own characterization, via spokesperson Elisabeth Diana, was that she was "dancing and mouthing words to the song, but it was unclear if she was 'singing.'"[^cbs]

Kalshi's public notice on the event stated (verbatim): "Due to ambiguity over whether or not Cardi B's attendance at the 2026 Super Bowl halftime show constituted a qualifying 'performance', Kalshi is invoking Rule 6.3(c) to settle this market to the last traded price before trading was paused. Those prices are $0.26 for Yes holders and $0.74 for No holders. Conversely, per Kalshi's full rules, celebrities that danced in the background during the halftime show but did not visibly sing or play an instrument did not 'perform' for purposes of the contract."[^kalshi-event]

At least one Yes trader filed a complaint with the CFTC, alleging Kalshi violated the Commodity Exchange Act through unfair and deceptive conduct, and seeking **$3,700** (the trader received $1,300 versus an anticipated $5,000).[^cbs][^readwrite]

The parallel Polymarket market reached the **opposite** outcome: it resolved **Yes** (Cardi B performed) via its UMA dispute process, paying Yes holders in full — though that resolution was itself disputed, with traders complaining that clarifying context was added only after the show.[^fortune][^nbc]

## The allegation against Kalshi

### 1. The governing rule contradicted itself

The core "performs" clause included dancing; the exclusion list removed dancing-without-singing. A performer who is part of the official staging and visibly dances — exactly Cardi B's situation — satisfies one clause and fails the other. The contract supplied no tiebreaker, so the central question users were trading had no determinable answer under the written rule.[^terms-jan2026]

### 2. The market title was broader than even the operative rule intended

The visible market asked "Who will perform at the Big Game?" An ordinary user would treat an on-stage halftime cameo as a performance. The rule's own exclusion list intended a narrower test, but the affirmative clause undercut it, so neither the headline nor the fine print produced a clean standard.

### 3. The last-price settlement made neither side whole

The 6.3(c) mechanism distributed $0.26 to Yes and $0.74 to No. That preserved total contract value but refunded no trader's principal: a Yes buyer who paid above $0.26 still lost, and a No buyer who paid above $0.74 still lost. The CFTC complainant received $1,300 against a $5,000 expectation.[^cbs] That is the practical cost of using a market price as a settlement proxy when the contract is irresolvable.

## Kalshi's defense

Kalshi's position was that the evidence did not establish whether Cardi B satisfied the performance definition — the broadcast showed dancing and mouthing words but did not make clear whether she was singing — and that its rules addressed exactly this kind of ambiguity, with the last-price split distributing value by market price rather than letting Kalshi retain the disputed amount.[^cbs]

The defense has real force on the *mechanics*: Kalshi disclosed the ambiguity, named the rule, and did not silently flip a binary. But the defense does not rehabilitate the *contract*. The reason the evidence "could not determine" the outcome is that the governing rule itself pointed in two directions on dancing. And Kalshi's later amendment is hard to square with a claim that the original rule was clear.

## Assessment

### Did Cardi B plainly perform under the governing rule?

**Indeterminate by construction.** She plainly danced on the broadcast. The governing rule's affirmative clause counted dancing; its exclusion clause did not. The rule could not answer its own question.[^terms-jan2026][^cbs]

### Did Kalshi follow a clean written rule?

**No — because there was no clean written rule.** The prior framing credited Kalshi with applying a definition that required "active musical contribution... singing, rapping, playing an instrument, DJ-ing, or conducting a live band." That language did not govern on February 8, 2026. It is the March 2, 2026 amendment.[^terms-current][^cert-mar2026] The rule actually in force was self-contradictory.

### Did Kalshi create a badly specified market?

**Yes — demonstrably.** A contract whose affirmative and exclusion clauses conflict on the precise fact in dispute is defective. Kalshi's own post-event amendment, certified "for clarity," is direct evidence of the defect.[^cert-mar2026]

### Was this a real failure for the tracker?

**Yes.** A ~$47.3M consumer-facing market failed to produce the binary answer users were trading, force-settled to a price that made neither side whole, drew a federal complaint, and resolved opposite to Polymarket on identical facts — all traceable to a self-contradictory rule that Kalshi then rewrote. This is a rule-design failure, not Kalshi paying the objectively wrong side of a clean contract.

### Overall classification

- **Operational settlement error:** Not established
- **Rule applied as written:** No — the governing rule was internally contradictory
- **Rule-design / contract-drafting failure:** Yes (confirmed by the post-event amendment)
- **User-expectation failure:** Yes
- **Best public verdict:** Failure; Failure-resolved: Unresolved

## Precise blocker to a stronger finding

The residual blocker is evidentiary on the underlying fact: public sources do not establish whether Cardi B made any audible musical contribution, only that she danced and mouthed words.[^cbs][^nbc] But this blocker no longer affects the verdict. Whether or not she sang, the governing contract could not resolve the case — its affirmative and exclusion clauses conflicted — which is itself the failure. The individual Cardi B market has been pruned from Kalshi's public API, so the settlement is verified from the event's `important_info` metadata and contemporaneous reporting rather than a live market page; those agree on the $0.26/$0.74 split.

## Sources

### Platform / primary

[^kalshi-event]: Kalshi, trade API event `KXPERFORMSUPERBOWLB-26` (`api.elections.kalshi.com/trade-api/v2/events/KXPERFORMSUPERBOWLB-26`). The `product_metadata.important_info` note records the Rule 6.3(c) ambiguity settlement and the exact last-traded prices ($0.26 Yes / $0.74 No). The individual Cardi B strike market has been pruned from the public markets endpoint. [API][kalshi-event]

[^terms-jan2026]: Kalshi, `PERFORM` contract terms as archived January 11, 2026 — the version governing the February 8, 2026 event. Defines "performs" as appearing on stage/broadcast AND "Performs (including dancing, singing, DJ-ing, e.g.)" AND being a scheduled or guest performer, while separately excluding "Dancing or appearing on stage without singing/playing instruments." Points to Rule 6.3(b) for payout determination and Rule 6.3(d) for the review process. [Wayback PDF][terms-jan2026]

[^terms-current]: Kalshi, current `PERFORM` contract terms (post-event amendment). Replaces the loose "performs (including dancing... e.g.)" language with a requirement that the performer "actively and perceptibly contributes to a musical performance by singing (including audible lead or backing vocals), rapping, playing a musical instrument, DJ-ing, or conducting a live band," and that a guest must perform "at least one full verse, chorus, or musical segment." This stricter language did NOT govern on February 8, 2026. [PDF][terms-current]

[^cert-mar2026]: KalshiEX LLC, CFTC Regulation 40.6 notification amending the "Will `<performer>` perform at `<event>`?" contract, dated March 2, 2026 — filed after the event. Cover letter lists the changes, including "Change to Payout Criterion for clarity," confirming Kalshi tightened the performance definition after the Cardi B dispute. [Cert PDF][cert-mar2026]

### Reporting

[^cbs]: CBS News, "Dispute over Cardi B's Super Bowl cameo roils prediction markets," February 2026. Reports the $0.26 Yes / $0.74 No split, ~$47.3M Kalshi volume vs ~$10M Polymarket, the CFTC complaint ($3,700 sought; $1,300 received vs $5,000 expected), spokesperson Elisabeth Diana's "dancing and mouthing words... unclear if she was 'singing'" characterization, and the Polymarket contrast. [CBS][cbs]

[^nbc]: NBC News, "Cardi B's cameo in Bad Bunny's Super Bowl halftime show leads to dispute over prediction markets," February 2026. Describes Cardi B on the porch set with Karol G, Young Miko, Jessica Alba, and Pedro Pascal, dancing to the music with singing unclear, and the divergent Kalshi/Polymarket outcomes. [NBC][nbc]

[^fortune]: Fortune, "Prop bet chaos as Kalshi calls Cardi B's Super Bowl cameo ambiguous and Polymarket pays out on disputed wager," February 11, 2026. Reports Polymarket resolving Yes via UMA while Kalshi force-settled to last price. [Fortune][fortune]

[^readwrite]: ReadWrite, "CFTC complaint filed over Kalshi Cardi B Super Bowl decision," February 2026. Reports the Yes holder's CFTC complaint alleging Commodity Exchange Act violation and the $3,700 in damages sought. [ReadWrite][readwrite]

[kalshi-event]: https://api.elections.kalshi.com/trade-api/v2/events/KXPERFORMSUPERBOWLB-26
[terms-jan2026]: https://web.archive.org/web/20260111210154id_/https://kalshi-public-docs.s3.amazonaws.com/contract_terms/PERFORM.pdf
[terms-current]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/PERFORM.pdf
[cert-mar2026]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/PERFORM.pdf
[cbs]: https://www.cbsnews.com/news/cardi-b-super-bowl-prediction-market-dispute/
[nbc]: https://www.nbcnews.com/business/business-news/cardi-b-cameo-bad-bunnys-super-bowl-halftime-show-leads-dispute-predi-rcna258553
[fortune]: https://fortune.com/2026/02/11/did-cardi-b-perform-at-super-bowl-prop-bet-kalshi-polymarket/
[readwrite]: https://readwrite.com/cftc-complaint-filed-kalshi-cardi-b-super-bowl-event-decision/
