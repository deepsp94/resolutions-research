# Polymarket: Cardi B Super Bowl halftime performance

## Bottom line

**Finding: Failure — an ambiguity / rule-design failure, not a proven misgrade. Polymarket's rule asked only whether Cardi B would "perform live and in person," with no definition of "perform." She made a staged cameo — dancing in a celebrity ensemble, never taking the mic, with reporting unable to confirm she sang. The market resolved Yes (`outcomePrices ["1","0"]`), but only after the proposed answer was disputed twice on the UMA oracle, the single contested outcome among five Yes-resolved performers. The Yes payout is defensible but under-specified; whether the right side was paid was never settled by the rule, only by adjudication. Failure-resolved: Unresolved. Confidence: medium-high.**

Polymarket asked whether Cardi B would "perform live and in person" during the Super Bowl LX halftime show.[^polymarket] Cardi B appeared during Bad Bunny's halftime show on a staged set, danced with an ensemble of celebrities, and — per uniform reporting — "never took the mic," with sources unable to confirm whether she was singing or merely mouthing words.[^kron4][^fos][^cbs] Reporting across outlets characterized the appearance as a **cameo**.[^kron4][^instyle][^nbc-ap]

Polymarket resolved the Cardi B outcome **Yes** (`outcomePrices ["1","0"]`).[^polymarket] What the prior draft of this file missed is the on-chain dispute history: the Yes answer was proposed, disputed, re-proposed, and disputed a second time before final resolution (`umaResolutionStatuses ["proposed","disputed","proposed","disputed"]`), and the Cardi B market closed February 12 — three days after the four other Yes-resolved performers, each of which cleared cleanly on a single proposal.[^polymarket] Cardi B was the only contested outcome in the event.

The allegation is that a cameo is not a performance. The strongest defense is that Polymarket's rule was simpler than Kalshi's: it required only that she "perform live and in person," with halftime footage as the primary source. It did not require audible singing, a microphone, a verse, a chorus, or instrumental performance. The best classification is therefore an **under-specified category boundary** — performance versus cameo — left to post-event judgment on a market that drew $5.6 million on the outcome and $10.5 million across the event. That is a rule-design failure even though the final Yes is not provably wrong.

## Market details

- **Venue:** Polymarket
- **Event:** `Who will perform at 2026 Big Game halftime show?` — slug `who-will-perform-at-super-bowl-halftime-show` (event id 28829).[^polymarket]
- **Market:** `Will Cardi B perform during the Super Bowl LX halftime show?` — slug `will-cardi-b-perform-during-the-super-bowl-lx-halftime-show` (market id 555793).[^polymarket]
- **Event:** Super Bowl LX halftime show, February 8, 2026 (Levi's Stadium, Santa Clara, CA).
- **Market opened:** June 25, 2025.[^polymarket]
- **End date / close:** Cardi B market closed February 12, 2026 (06:50 UTC); the four other Yes performers closed February 9.[^polymarket]
- **Governing rule:** Yes if Cardi B "performs live and in person"; otherwise No. Primary source is halftime footage, plus a consensus of credible reporting. **No definition of "perform."**[^polymarket]
- **Outcome volume:** approximately $5.6 million on Cardi B; approximately $10.5 million across the event.[^polymarket][^fos]
- **Settled outcome:** Yes (`outcomePrices ["1","0"]`).[^polymarket]
- **UMA resolution:** `resolved`, after two dispute rounds (`["proposed","disputed","proposed","disputed"]`).[^polymarket]

## The rule

The Polymarket market description reads, verbatim:

> "This market will resolve to 'Yes' if Cardi B performs live and in person during the Super Bowl LX halftime show currently scheduled for February 8, 2026. Otherwise, this market will resolve to 'No.' … The primary resolution source for this market will be footage of the Super Bowl LX halftime show, however a consensus of credible reporting will also be used."[^polymarket]

That rule does not define "performs." It does not say whether dancing, lip-syncing, mouthing lyrics, appearing as part of staged choreography, or making a celebrity cameo counts. The same template applied to every performer in the event; only the name changed.[^polymarket]

## What happened

Cardi B joined Bad Bunny's halftime show on a staged set with other guest celebrities, dancing in an ensemble that included Karol G, Young Miko, Jessica Alba, and Pedro Pascal.[^kron4][^eonline] Reporting was consistent that she did not take the microphone and did not perform her Bad Bunny collaboration "I Like It," and that it was unclear whether she was singing.[^kron4][^eonline][^cbs] One outlet noted she "appeared to be singing" but that it was "possible she was simply mouthing."[^fos] Outlets across the board described the appearance as a cameo.[^kron4][^instyle][^nbc-ap]

Polymarket decided this counted and resolved the Cardi B outcome Yes.[^polymarket] The Associated Press reported that "Polymarket's contract was resolved as Cardi B had performed, but the yes was disputed," with a final decision expected the following Wednesday (February 11).[^nbc-ap] The on-chain record confirms the contest: the Yes answer was disputed twice on the UMA oracle before final resolution, and the market did not close until February 12.[^polymarket]

## The allegation against Polymarket

### 1. A cameo may not be a performance

The strongest No-side argument is ordinary-language based. Reporting described the appearance as a cameo, with no established singing role; she "never took the mic."[^kron4][^fos] If "perform" means actively delivering music, vocals, a verse, or a defined segment, a silent or inaudible stage appearance with dancing is not enough.

### 2. Polymarket gave traders little ex ante boundary guidance

Polymarket's rule did not specify whether dancing, mouthing lyrics, or appearing without a microphone would count.[^polymarket] That omission matters because halftime shows routinely include celebrity cameos, backing dancers, pre-recorded vocals, lip-syncing, and staged non-musical appearances. The rule left the decisive boundary to post-event judgment.

### 3. The dispute record shows the boundary was genuinely unstable

This is the decisive new evidence. Of the five performers Polymarket resolved Yes — Bad Bunny, Karol G, Lady Gaga, Ricky Martin, and Cardi B — only Cardi B drew a dispute. The other four cleared on a single proposal and closed February 9; Cardi B's Yes was proposed, disputed, re-proposed, and disputed again before resolving, closing February 12.[^polymarket] The UMA proposers themselves could not agree the first time, which is direct, on-chain evidence that the category was unstable rather than a matter the rule cleanly answered.

### 4. The parallel Kalshi market split the same event

Kalshi did not treat the appearance as a clean Yes. Citing "ambiguity over whether or not Cardi B's attendance … constituted a qualifying 'performance,'" it invoked an ambiguity rule and settled at the last traded price — $0.74 for No holders and $0.26 for Yes holders — returning all money to users.[^nbc-ap][^cbs] A Kalshi Yes holder filed a complaint with the CFTC over the handling.[^nbc-ap][^cbs] Different rules, but the same underlying fact pattern producing opposite treatments confirms the category was genuinely contested.[^fos]

## Polymarket's defense

Polymarket did not publish a detailed public defense. The strongest defense is implicit in the rule and the final market page:

- Cardi B appeared live and in person during the official halftime show.[^kron4][^eonline]
- She was part of the staged presentation, not an audience member.[^kron4]
- She visibly danced as part of the musical set.[^eonline][^fos]
- The rule did not require audible singing, a microphone, a full verse, or official billing as a performer.[^polymarket]
- After two dispute rounds, the UMA oracle upheld Yes.[^polymarket]

Under that broader reading, "performance" can include visible participation in a live staged halftime number even if the contribution is mostly dance or cameo-style staging.

## Assessment

### Did Cardi B appear live and in person?

**Yes.** Reporting and footage descriptions agree she appeared on the staged set during the halftime show.[^kron4][^eonline][^instyle]

### Did she clearly perform in the narrower musical sense?

**Not established.** Reporting says she "never took the mic," did not perform her own song, and that it was unclear whether she was singing or mouthing.[^kron4][^fos][^cbs]

### Did Polymarket's written rule require that narrower musical sense?

**No, not explicitly.** The rule used the broad phrase "performs live and in person" and named halftime footage as the primary source. It added no exclusions for dancing, mouthing words, or appearing without singing.[^polymarket]

### Was Polymarket's Yes resolution clearly wrong?

**No.** No is a plausible ordinary-language outcome if "performance" means active musical contribution; Yes is also plausible under the broader wording because Cardi B visibly participated in the staged number. The two-round UMA dispute shows reasonable on-chain actors disagreed.[^polymarket]

### Was this a real failure for the tracker?

**Yes — as an ambiguity / rule-design failure.** Polymarket should have defined what kind of participation counts as a halftime performance before the event. A market that drew $5.6 million on the outcome turned on a predictable category boundary — performance versus cameo — that the rule never addressed and that was settled only through contested adjudication. That is enough to include the case, but not enough to say the final Yes payout was objectively false.

### Was the failure resolved?

**Unresolved.** The boundary was not settled by the rule text. It was settled only by the UMA dispute process upholding Yes after two challenges. Whether the right side was paid remains a matter of judgment, not of any pre-defined criterion.

### Overall classification

- **Operational settlement error:** Not established
- **Semantic ambiguity:** Yes
- **Rule-design weakness:** Yes
- **Final outcome plainly wrong:** Not established
- **Best public verdict:** Failure — defensible but under-specified Yes resolution, unresolved as to which side was right

## Precise blocker to a stronger finding

The blocker is the lack of a crisp contractual definition of "perform" and the lack of definitive public evidence about Cardi B's exact audio contribution. If Polymarket had required audible singing, No would be much stronger. If official production credits or audio evidence showed a live vocal or choreographed musical segment, Yes would be much stronger. The present public record — a cameo with no confirmed vocal, resolved Yes only after two UMA disputes — supports an ambiguity failure rather than a proven misgrade.

## Sources

### Platform / primary

[^polymarket]: Polymarket gamma-api, event `who-will-perform-at-super-bowl-halftime-show` (id 28829) and market `will-cardi-b-perform-during-the-super-bowl-lx-halftime-show` (id 555793). Records the verbatim rule ("performs live and in person," no definition of "perform"), `outcomePrices ["1","0"]` (Yes), `umaResolutionStatus resolved` with `umaResolutionStatuses ["proposed","disputed","proposed","disputed"]`, Cardi B outcome volume ~$5.57M, event volume ~$10.46M, June 25 2025 open, and the February 12 2026 close (vs. February 9 for the four other Yes performers). [Event][polymarket] · [gamma][gamma]

### Reporting

[^nbc-ap]: Associated Press via NBC News, "Cardi B's cameo in Bad Bunny's Super Bowl halftime show leads to dispute over prediction markets," February 11, 2026. Reports Polymarket "resolved as Cardi B had performed, but the yes was disputed," a final decision expected Wednesday; the Kalshi 74¢/26¢ ambiguity settlement and CFTC complaint; ~$10M Polymarket volume and $47.3M on Kalshi. [Article][nbc-ap]

[^cbs]: CBS News, "Dispute over Cardi B's Super Bowl cameo roils prediction markets," February 11, 2026. "Unclear if the artist was singing"; Polymarket to issue a final decision Wednesday; Kalshi's partial 74¢/26¢ payout and CFTC complaint. [Article][cbs]

[^fos]: Front Office Sports, "Cardi B Is a Cautionary Tale for Prediction Markets," February 10, 2026. ~$5M+ of ~$10M Polymarket volume on Cardi B; "appeared to be singing … possible she was simply mouthing"; Kalshi rule that dancing-only does not count. [Article][fos]

[^kron4]: KRON4 (Nexstar), "Cardi B, Pedro Pascal, Jessica Alba and more make cameos in Bad Bunny halftime show," February 8, 2026. "Cardi was there … but she never took the mic … dancing under the stage as part of an ensemble." [Article][kron4]

[^eonline]: E! News, "Super Bowl 2026: Cardi B at Bad Bunny Halftime Show," February 8, 2026. Notes she "didn't perform 'I Like It' with Bad Bunny" and danced onstage to "Yo Perreo Sola." [Article][eonline]

[^instyle]: InStyle, "Cardi B Stuns in Corset Dress for Super Bowl 2026 Halftime Show Cameo," February 8, 2026. Describes a "surprise cameo" during Bad Bunny's halftime show. [Article][instyle]

[polymarket]: https://polymarket.com/event/who-will-perform-at-super-bowl-halftime-show
[gamma]: https://gamma-api.polymarket.com/events?slug=who-will-perform-at-super-bowl-halftime-show
[nbc-ap]: https://www.nbcnews.com/business/business-news/cardi-b-cameo-bad-bunnys-super-bowl-halftime-show-leads-dispute-predi-rcna258553
[cbs]: https://www.cbsnews.com/news/cardi-b-super-bowl-prediction-market-dispute/
[fos]: https://frontofficesports.com/cardi-b-is-a-cautionary-tale-for-prediction-markets/
[kron4]: https://www.kron4.com/sports/super-bowl-lx/did-you-miss-cardi-b-pedro-pascals-quick-cameos-in-the-bad-bunny-halftime-show/
[eonline]: https://www.eonline.com/news/1427758/super-bowl-2026-cardi-b-at-bad-bunny-halftime-show
[instyle]: https://www.instyle.com/cardi-b-super-bowl-2026-halftime-show-bad-bunny-corset-dress-11897983
