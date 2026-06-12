# Polymarket: Strategy sells Bitcoin by May 31, 2026

## Bottom line

**Finding: Polymarket made both an outcome error and a rules/process error. Confidence: high.**

Strategy sold 32 bitcoin during May 26-31, 2026. The original market rule said the market would resolve Yes if Strategy sold any bitcoin by 11:59 p.m. ET on May 31. It did not say that Strategy had to disclose the sale, or that public evidence had to become available, before that deadline.[^market][^filing]

After Strategy disclosed the sale on June 1, Polymarket added a confirmation-timing requirement and endorsed No: information available within the market window had not confirmed a sale, and confirmation obtained after the window did not qualify.[^galaxy][^coindesk] The market ultimately resolved No after two No proposals were disputed and the matter proceeded to final review.[^market][^api]

The No result is understandable only if the original event condition is replaced with an announcement or confirmation condition. That condition was not in the published rule. Polymarket's own documentation says that post-launch clarifications cannot change a question's fundamental intent.[^resolution-docs] In this case, the clarification changed the relevant event from **Strategy selling bitcoin** to **the sale becoming publicly confirmable**.

## Market details

- **Venue:** Polymarket
- **Event:** `MicroStrategy sells any Bitcoin by ___ ?`
- **Disputed outcome:** `MicroStrategy sells any Bitcoin by May 31, 2026?`
- **Market opened:** May 5, 2026
- **Stated deadline:** May 31, 2026 at 11:59 p.m. ET
- **Final resolution:** No
- **Resolution path shown by Polymarket:** No proposed, disputed; No proposed again, disputed; final outcome No
- **Market page:** [Polymarket event page][market]
- **Primary metadata:** [Polymarket Gamma API record][api]

Polymarket's API currently reports approximately $375.8 million in volume for the May 31 outcome. Contemporary articles reported lower figures while trading and dispute activity were still in progress, so those figures should not be treated as contradictions.[^api][^coindesk][^galaxy]

## The original rule

The operative rule said:

> This market will resolve to "Yes" if MicroStrategy sells any of its Bitcoin by 11:59 PM ET on the date specified in the title.

The next sentence identified the evidence to be used: information from MSTR and on-chain data would be the primary resolution source, with a consensus of credible reporting also available.[^market][^api]

Two distinctions matter:

1. The operative event was a **sale**, not an announcement or confirmation.
2. The source clause identified how to establish whether the sale occurred. It did not state that the evidence itself had to be published before the event deadline.

This is reinforced by Polymarket's separately drafted Strategy purchase-announcement markets. Those rules expressly say that resolution is based on announcements made inside the designated window, regardless of when the purchases occurred.[^announcement-market] Polymarket therefore had established wording available when it intended the announcement date, rather than the underlying transaction date, to control.

## What happened

### May 31: the market deadline passed

The market's event deadline was May 31 at 11:59 p.m. ET.[^market] No public source had conclusively established a sale by that time, according to Polymarket's later clarification.[^galaxy][^coindesk]

That lack of contemporaneous public confirmation did not mean that no sale had occurred. It meant only that traders and resolvers did not yet have definitive public evidence of one.

### June 1: Strategy disclosed an in-window sale

Strategy filed a Form 8-K dated June 1. Its bitcoin update reported:

- 32 BTC sold;
- an aggregate sale price of $2.5 million;
- an average sale price of $77,135; and
- a transaction period of May 26 through May 31.

The filing presented the bitcoin activity and holdings as of May 31 at 4:00 p.m. ET, before the market's 11:59 p.m. deadline.[^filing]

This is direct evidence from the market's named primary source, Strategy itself, that at least one sale occurred by the deadline.

### June 1: Polymarket added a confirmation requirement

After the filing became public and Yes rose sharply, Polymarket posted "Additional context." Galaxy reproduces the statement and places it at approximately 1:00 p.m. ET:

> Confirmation achieved outside of the market's time frame does not qualify.

The full clarification said that no information from MSTR, on-chain data, or a credible-reporting consensus had confirmed a sale within the market timeframe.[^galaxy] CoinDesk independently reports the same clarification and its confirmation-based interpretation.[^coindesk]

The clarification did not dispute Strategy's filing or claim that the sale occurred after May 31. It instead made the date on which the sale became confirmable dispositive.

### June 1-3: two No proposals were disputed

Polymarket's market page and API record show the following sequence:

1. No proposed.
2. Proposal disputed.
3. No proposed again.
4. Proposal disputed again.
5. Final outcome No.

Under Polymarket's documented process, a second dispute escalates resolution to a vote by UMA token holders.[^market][^api][^resolution-docs] The public market record establishes the final No outcome, although the detailed individual voter rationales are not preserved on the market page.

## The allegation against Polymarket

The strongest allegation is not merely that the result felt counterintuitive. It is that Polymarket changed the test after the event:

- **Original test:** Did Strategy sell any bitcoin by May 31?
- **Clarified test:** Was a sale confirmed by an approved source by May 31?

Those tests can produce different answers whenever a company executes a transaction before a deadline but reports it afterward. That is exactly what happened here.

The filing satisfies the original event-based test. The final No result therefore conflicts with both the ordinary reading and the grammatical structure of the original rule.[^market][^filing]

The clarification also appears inconsistent with Polymarket's published clarification policy. Its documentation permits "Additional context" after trading begins but says that a clarification cannot change the question's fundamental intent.[^resolution-docs] A market about when a sale occurred was converted into one about when evidence of the sale became public.

Galaxy Research reached the same substantive conclusion, calling the change retroactive. Its analysis is detailed and reproduces the relevant documents and market activity, but it must be read with its disclosed conflict: Galaxy stated that it held a financial interest in Yes shares in this market.[^galaxy]

## Polymarket's defense

### Explicit position

Polymarket's explicit position is contained in its Additional context notice:

- none of the permitted source categories confirmed a sale within the market timeframe; and
- confirmation obtained outside the timeframe did not qualify.[^galaxy][^coindesk]

This treats the deadline as closing both the event window and the evidence window.

Polymarket's public documentation also assigns the final decision to UMA's oracle process and says finalized UMA outcomes cannot be altered or reversed by Polymarket.[^dispute-docs] That explains why the on-chain No result remained final, but it does not answer whether Polymarket's clarification gave UMA the correct rule to apply.

### Strongest implicit defense

The strongest good-faith defense, reconstructed from the clarification and the arguments reported by CoinDesk, is:

1. A resolver must decide from information available at the deadline.
2. Permitting later disclosures to reach backward could leave apparently expired markets unsettled indefinitely.
3. Traders could dispute an unfavorable proposal and wait for later evidence, weakening deadline finality.
4. Previous Polymarket disputes were reportedly resolved using only information available within the stated timeframe.[^coindesk]

This is a real market-design concern. A contract should specify how long resolvers must wait for delayed reports and whether later evidence can prove an earlier event.

It is not, however, a sufficient defense of this resolution. The concern supports writing a confirmation cutoff into the rule before trading starts. It does not support adding one after the event. Polymarket demonstrated in its announcement-based Strategy markets that it could state such a condition expressly.[^announcement-market]

### Limits of the defense

The defense has three major weaknesses:

1. **The text separates event and evidence.** The event clause asks when Strategy sold; the source clause says what evidence can establish the sale.[^market]
2. **The named primary source later answered the event question directly.** Strategy's filing dates the sales to May 26-31.[^filing]
3. **Polymarket's own policy limits clarifications.** Additional context may address unforeseen circumstances but may not change fundamental intent.[^resolution-docs]

The finality problem was also foreseeable. Strategy generally disclosed bitcoin activity after the transaction period, with CoinDesk describing its reporting as usually weekly and on Mondays.[^coindesk] If same-window public confirmation was essential, that should have been part of the original contract.

## Assessment

### Was the real-world outcome wrong?

**Yes.**

The market asked whether Strategy sold any bitcoin by May 31. Strategy's own Form 8-K says it sold 32 BTC during May 26-31. The market resolved No.[^filing][^market]

This conclusion does not depend on whether traders could know about the sale before the deadline. Polymarket's resolution documentation distinguishes the market end date from the later point at which an outcome becomes known and can be finalized.[^resolution-docs] This contract did not make contemporaneous knowledge an element of Yes.

### Were the original rules deficient?

**Yes, but not because the event condition itself was unclear.**

The event condition was naturally event-based. The deficiency was that the rules did not state:

- how long resolution should wait for Strategy's next disclosure;
- whether post-deadline evidence could prove an in-window sale; or
- whether confirmation itself had to occur by the deadline.

That omission created an administrability problem. It did not make No the better reading.

### Was the clarification improper?

**Yes.**

The clarification supplied a new substantive requirement rather than explaining an existing one. It changed which date controlled and thereby determined who won. On the available evidence, this conflicts with Polymarket's rule that a clarification cannot change the fundamental intent of the question.[^resolution-docs]

### Did the oracle process independently correct the problem?

**No.**

The two disputes forced additional review, but the final result remained No.[^market][^api] The process ratified the confirmation-based interpretation rather than correcting it.

### Overall classification

- **Resolution-outcome failure:** Yes
- **Post-launch rule/clarification failure:** Yes
- **Original drafting failure:** Yes, because delayed official reporting was foreseeable and untreated
- **Pure oracle malfunction:** Not established; UMA appears to have followed Polymarket's clarification
- **Evidence of fraud or deliberate favoritism:** Not established
- **Confidence:** High

## Remaining evidentiary limits

These limits do not prevent a conclusion on the core error:

- The publicly rendered market page no longer displays the full Additional context notice. Its exact wording and approximate posting time are preserved by Galaxy and corroborated by CoinDesk, rather than presently visible on the market page.[^galaxy][^coindesk]
- The market page does not preserve the detailed rationale or position holdings of individual UMA voters. It therefore does not support claims about particular voters' motives or conflicts.
- Galaxy's analysis is unusually detailed but financially interested. The decisive facts do not rely on Galaxy alone: the original rule, filing, final result, clarification policy, and event metadata are available from primary Polymarket and Strategy sources.[^market][^api][^filing][^resolution-docs]

## Sources

### Primary

[^market]: Polymarket, [“MicroStrategy sells any Bitcoin by ___ ?”][market]. The page contains the original rule and displays the No resolution and dispute sequence.

[^api]: Polymarket Gamma API, [event metadata for `microstrategy-sell-any-bitcoin-in-2025`][api]. The May 31 outcome record contains the original description, creation time, volume, dispute statuses, and final No price.

[^filing]: Strategy Inc., [Form 8-K dated June 1, 2026][filing], pp. 2-3. The filing reports 32 BTC sold during May 26-31 and says the bitcoin information is presented as of May 31 at 4:00 p.m. ET.

[^resolution-docs]: Polymarket Documentation, [“Resolution”][resolution-docs]. It describes the dispute process and states that post-launch clarifications cannot change a question's fundamental intent.

[^dispute-docs]: Polymarket Help Center, [“How Are Markets Disputed?”][dispute-docs]. It explains UMA voting and Polymarket's position that finalized outcomes are immutable.

[^announcement-market]: Polymarket, [“MicroStrategy announces >1000 BTC purchase May 12-18?”][announcement-market]. This comparator expressly makes announcements within the window controlling regardless of when purchases occurred.

### Contemporaneous reporting and analysis

[^coindesk]: Sam Reynolds, CoinDesk, [“Strategy sold bitcoin in late May, and told the market in June”][coindesk], published June 2 and updated June 8, 2026. It reports the arguments on all sides and independently reproduces Polymarket's confirmation-based clarification.

[^galaxy]: Will Owens, Galaxy Research, [“Strategy Sold Bitcoin in May. Polymarket Says It Didn't”][galaxy], June 4, 2026. It reproduces the rule, clarification, filing, market chronology, and final outcome. Galaxy discloses that it held a financial interest in Yes shares.

[market]: https://polymarket.com/event/microstrategy-sell-any-bitcoin-in-2025/microstrategy-sells-any-bitcoin-by-may-31-2026
[api]: https://gamma-api.polymarket.com/events?slug=microstrategy-sell-any-bitcoin-in-2025
[filing]: https://assets.contentstack.io/v3/assets/bltf8d808d9b8cebd37/blt01aedf36c9f1b5b3/6a1cdb95487e7818fe49dd85/form-8-k_06-01-2026.pdf
[resolution-docs]: https://docs.polymarket.com/concepts/resolution
[dispute-docs]: https://help.polymarket.com/en/articles/13364551-how-are-markets-disputed
[announcement-market]: https://polymarket.com/event/microstrategy-announces-1000-btc-purchase-may-12-18
[coindesk]: https://www.coindesk.com/markets/2026/06/02/strategy-sold-bitcoin-in-late-may-and-told-the-market-in-june-here-s-how-polymarket-bettors-are-fighting-over-when-it-counts
[galaxy]: https://www.galaxy.com/insights/research/strategy-bitcoin-sale-polymarket-resolution-dispute-may-2026
