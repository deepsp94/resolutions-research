# Kalshi: Cardi B Super Bowl halftime performance

## Bottom line

**Finding: This was a real resolution controversy and a rule-design failure, but not a proven Kalshi misgrade under the written rules. Confidence: high.**

Kalshi listed a 2026 Super Bowl halftime market asking who would perform at the Big Game. Cardi B appeared during Bad Bunny's halftime show with Karol G, Young Miko, Jessica Alba, and Pedro Pascal. Multiple reports described her as dancing and mouthing words, while noting that it was unclear whether she was actually singing.[^ap][^business-insider][^nypost]

Kalshi did not settle Cardi B as a normal binary Yes or No. It invoked its ambiguity process and settled the market at the last traded prices before trading was paused: **$0.26 for Yes holders and $0.74 for No holders**.[^kalshi-market][^ap][^business-insider]

The strongest criticism is that the contract's definitions made a high-volume market effectively irresolvable. The strongest defense is that Kalshi publicly identified the ambiguity, used the last-price mechanism provided by its rules, and distributed the contract value according to that mechanism rather than pretending the evidence clearly proved one side.

This should be tracked as a **rule-design and user-expectation failure**, not as a straightforward operational settlement error.

## Market details

- **Venue:** Kalshi
- **Market family:** `Who will perform at the Big Game?`
- **Series:** `KXPERFORMSUPERBOWLB`
- **Event:** 2026 Super Bowl halftime show, February 8, 2026
- **Relevant strike:** Cardi B
- **Market volume:** Kalshi's page shows approximately **$47.3 million** for the market family; AP also reported more than $47.3 million wagered on Kalshi's market.[^kalshi-market][^ap]
- **Settlement used for Cardi B:** last traded price before trading was paused: $0.26 for Yes, $0.74 for No.[^kalshi-market]
- **Platform page:** [Kalshi market page][kalshi-market]
- **Full contract terms:** [Kalshi `PERFORM` contract terms][perform-terms]

## The rule

Kalshi's full `PERFORM` terms defined the underlying as whether the named performer performs at the specified event or whether it is announced that the performer will perform at the event.[^perform-terms]

The full rules required more than presence. They required the performer to appear on stage or in the official broadcast, actively and perceptibly contribute to a musical performance by singing, rapping, playing an instrument, DJ-ing, or conducting a live band, and be either scheduled, a guest in another artist's set, or formally announced as a performer.[^perform-terms]

The same terms said a guest appearance counts when the performer performs at least one full verse, chorus, or musical segment, but they also excluded appearances without musical performance.[^perform-terms]

Kalshi's market page added an event-specific note that both Cardi B and Karol G strikes were suspended and that a February 5, 2026 clarification required the performer to appear on stage or in the official broadcast/stream and either be scheduled or make a guest appearance during another artist's performance.[^kalshi-market]

That combination created the problem. Cardi B clearly appeared in the show and appeared to participate physically, but the available public evidence did not clearly establish the active musical contribution that the full rules required.

## What happened

Cardi B joined the halftime show during Bad Bunny's set. AP reported that she danced to the music, but it was unclear whether she was singing along.[^ap] Business Insider similarly reported that she had no singing role but could be seen dancing and mouthing words.[^business-insider]

Kalshi's public market notice stated that, due to ambiguity over whether Cardi B's attendance constituted a qualifying performance, it was invoking Rule 6.3(c) and settling to the last traded price before trading was paused.[^kalshi-market]

Kalshi spokeswoman Elisabeth Diana gave the platform's explicit defense to multiple outlets: under the full rules, singing and dancing counted, but just dancing in the background did not; Cardi B was dancing and mouthing words, but it was unclear whether she was singing.[^ap][^business-insider][^nypost]

At least one Yes trader filed a CFTC complaint over Kalshi's handling of the contract, seeking $3,700 in damages.[^ap][^nypost]

## The allegation against Kalshi

### 1. The criteria pulled in opposite directions

Kalshi's terms included language that made a guest appearance during another artist's set count if the performer actively participated in a musical segment. But the terms also excluded dancing or appearing without singing or playing an instrument.[^perform-terms]

For a televised halftime cameo, those boundaries were not robust. A performer can be part of the official staging, visibly dance, mouth lyrics, and still leave viewers unable to determine whether there was live vocal contribution.

### 2. The market title was broader than the operative rule

The visible market was "Who will perform at the Big Game?" A normal user might treat an on-stage halftime cameo as a performance. Kalshi's detailed rule instead turned on a narrower question: whether Cardi B actively and perceptibly contributed musically in a qualifying way.

That mismatch was especially important because the relevant fact was not just whether she appeared, but whether she sang or otherwise contributed musically enough to satisfy the filed criteria.

### 3. The last-price settlement did not make either side whole

Kalshi's mechanism distributed $0.26 to Yes holders and $0.74 to No holders. That preserved the total contract value, but it did not refund every trader's principal. A Yes buyer who paid materially above $0.26 still lost money, and a No buyer who paid materially above $0.74 still lost money.

That is not necessarily a rule violation. It is the practical consequence of using a market price as a settlement proxy when the contract proves ambiguous.

## Kalshi's defense

Kalshi's explicit defense was that the evidence did not determine whether Cardi B satisfied the full performance definition. Its spokesperson said the broadcast showed dancing and mouthing words, but did not make clear whether she was singing.[^ap][^business-insider]

Kalshi also argued that its rules addressed this kind of ambiguity and that the last-price settlement split value according to the market price rather than letting Kalshi retain the disputed amount.[^nypost]

The rule-based defense is substantial:

- the full terms required active musical contribution, not merely presence;
- public reporting did not establish live singing or another qualifying musical contribution;
- the market page disclosed the ambiguity settlement and the exact Yes/No prices;
- the outcome was not a normal No misgrade; and
- the platform did not silently change the binary result after the fact.

## Assessment

### Did Cardi B plainly perform under Kalshi's full rule?

**Not established.**

She plainly appeared in the halftime show, but the full Kalshi rule required a qualifying musical contribution. The cited reports support ambiguity rather than a clean Yes.[^ap][^business-insider]

### Did Kalshi plainly violate its own rule?

**Not established.**

Kalshi identified the ambiguity and used a last-price settlement mechanism. The available public sources do not show that the contract required a normal Yes payout once ambiguity existed.

### Did Kalshi create a badly specified market?

**Yes.**

The rule tried to distinguish performance from cameo, but the distinction depended on facts that could be hard or impossible for viewers to verify from the broadcast. That is a design problem for a large consumer-facing market.

### Was this a real failure for the tracker?

**Yes, with careful classification.**

This belongs in the tracker because the market failed to produce a clean binary answer to the question users were trading, generated a formal complaint and public backlash, and exposed a drafting problem in performance markets. It should not be described as Kalshi simply paying the objectively wrong side.

### Overall classification

- **Operational settlement error:** Not established
- **Rule followed as written:** Plausibly yes
- **Rule-design failure:** Yes
- **User-expectation failure:** Yes
- **Conclusive platform mistake:** Yes, in market design; not proven in final settlement mechanics

## Precise blocker to a stronger finding

The main blocker is evidentiary. The public sources do not establish whether Cardi B was actually singing or otherwise making an audible musical contribution. Without broadcast audio, production audio, or an official performer statement resolving that fact, the strongest conclusion is that the contract was ambiguous in exactly the way Kalshi said it was.

## Sources

### Platform / primary

[^kalshi-market]: Kalshi, [`Who will perform at the Big Game?` market page][kalshi-market]. Records the Cardi B ambiguity notice, last-price settlement values, market volume, timeline, and source/rule summary.

[^perform-terms]: Kalshi, [`PERFORM` contract terms][perform-terms]. Defines what qualifies and does not qualify as a performance for performer markets.

### Reporting

[^ap]: Associated Press, ["Cardi B's cameo in Bad Bunny's Super Bowl halftime show leads to dispute on prediction markets"][ap], February 2026. Reports the appearance, volume, CFTC complaint, Kalshi's explanation, and Polymarket contrast.

[^business-insider]: Business Insider, ["Kalshi and Polymarket split over whether Cardi B 'performed' at the Super Bowl halftime show"][business-insider], February 9, 2026. Describes the appearance, Kalshi's rules, Kalshi's last-price settlement, and Polymarket's different outcome.

[^nypost]: New York Post, ["Kalshi's Cardi B. Super Bowl halftime show market draws millions - and is mired in controversy"][nypost], February 11, 2026. Quotes Kalshi's defense and describes the disputed payouts.

[kalshi-market]: https://kalshi.com/markets/kxperformsuperbowlb/who-will-perform-at-the-super-bowl/kxperformsuperbowlb-26
[perform-terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/PERFORM.pdf
[ap]: https://apnews.com/article/super-bowl-kalshi-cardi-b-bad-bunny-d3b51d8848934d69c39ff92fa2c51278
[business-insider]: https://www.businessinsider.com/kalshi-polymarket-cardi-b-performance-super-bowl-2026-2
[nypost]: https://nypost.com/2026/02/11/betting/kalshis-controversial-cardi-b-super-bowl-halftime-show-market-draws-millions/
