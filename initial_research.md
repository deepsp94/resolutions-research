From ChatGPT: 

Got it. With the corrected definition, I’d frame the list as **“resolution blowups / semantic oracle failures”**, not “formal disputes.”

I used this inclusion test: **there was meaningful public uproar, and the case exposed a real mismatch between market wording, ordinary-language truth, source rules, timing, or platform execution.** I’m not claiming every final outcome below was objectively wrong; I’m saying these are the cases worth studying for the “natural-language markets are hard to resolve” thesis.

## Tier 1 — strongest cases: real blowups / platform looked bad

| Case                                                            | Platform            | Failure mode                                | What happened / why it matters                                                                                                                                                                                                                                                                                                                                                                          |
| --------------------------------------------------------------- | ------------------- | ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Strategy / MicroStrategy sells Bitcoin by May 31**            | Polymarket          | **Event date vs confirmation date**         | The market asked whether Strategy sold BTC by May 31. Strategy later disclosed it sold 32 BTC during May 26–31, but the filing came June 1. Polymarket resolved **No**, effectively treating confirmation before deadline as required, even though users argued the rule text was event-based. This is probably the cleanest modern example of “ordinary truth vs resolution rule drift.” ([Galaxy][1]) |
| **Zelenskyy wears a suit before July**                          | Polymarket          | **Ordinary-language category failure**      | Zelenskyy wore a black jacket/shirt/trousers outfit; BBC and NY Post described it as a suit, but UMA/Polymarket-side resolution landed **No**. The issue was not just “was there a dispute?” but that “suit” has no crisp boundary across fashion, journalism, diplomacy, and trader incentives. ([WIRED][2])                                                                                           |
| **Ukraine / Trump minerals deal before April 2025**             | Polymarket          | **Premature/oracle governance failure**     | Market resolved **Yes** before the deal was actually signed. Reports described it as an oracle/governance attack by a large UMA holder; Polymarket acknowledged the situation was abnormal but did not refund users. This is more oracle-process failure than semantic ambiguity, but it clearly belongs. ([CryptoSlate][3])                                                                            |
| **Barron Trump involved in $DJT token**                         | Polymarket          | **Oracle/platform contradiction**           | UMA resolved one way; Polymarket publicly overrode/compensated because it believed Barron was involved “in some way.” This is important because the platform effectively said its own resolution process produced the wrong answer. ([WIRED][2])                                                                                                                                                        |
| **Oscars 2025 viewership**                                      | Kalshi              | **Initial data vs final data**              | Kalshi resolved using an initial Nielsen/press figure around 18.1M, while later final reporting put Oscars viewership around 19.7M. By the market’s procedural source/timing logic, Kalshi may defend the outcome; as a market about “Oscar viewership,” it paid the side that looked wrong after final data. ([PredictionNews][4])                                                                     |
| **Cardi B Super Bowl halftime “performance”**                   | Kalshi + Polymarket | **Category boundary: cameo vs performance** | Cardi B appeared during Bad Bunny’s halftime show; whether she “performed” depended on whether dancing, mouthing lyrics, singing, or appearing counted. Kalshi split settlement by last traded prices due ambiguity; Polymarket resolved Yes and drew anger. Same event, two platforms, no clean binary truth. ([AP News][5])                                                                           |
| **Khamenei “out as Supreme Leader” after death**                | Kalshi              | **Title/common sense vs death carveout**    | Kalshi had a carveout saying if a leader leaves solely because they died, settlement could use last traded prices rather than Yes. After Khamenei was reportedly killed, users argued “out” plainly included death; Kalshi defended the carveout, and a lawsuit followed. ([Reuters][6])                                                                                                                |
| **NFL futures / win-total misgrading**                          | Kalshi              | **Operational settlement error**            | Some NFL futures/win-total markets were initially refunded or mispaid instead of paying winners; Kalshi later paid the correct $1 settlement after backlash. This is not a semantic edge case; it is a “truth machine made an execution mistake” case. ([Next Event Horizon][7])                                                                                                                        |
| **NBA preseason games resolved before game end / wrong winner** | Kalshi              | **Operational premature resolution**        | Kalshi reportedly resolved two NBA preseason games before completion and with the wrong winner, then moved them back to TBD / said users would not lose from it. Again, not semantic, but a genuine resolution blowup. ([Next Event Horizon][8])                                                                                                                                                        |

---

## Tier 2 — genuine semantic/rule ambiguity uproar, but more defensible

| Case                                               | Platform   | Failure mode                                             | Why it belongs                                                                                                                                                                                                                                                                                                                               |
| -------------------------------------------------- | ---------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TikTok banned in the U.S. before May 2025**      | Polymarket | **Legal ban vs practical availability/enforcement**      | The law took effect and TikTok briefly became unavailable, but then enforcement was delayed and access returned. Users argued “banned” should mean practically banned, not technically subject to a statute. Polymarket resolved Yes and faced backlash. ([TradingView][9])                                                                  |
| **RFK Jr. drops out / withdraws before September** | Polymarket | **Suspending campaign vs withdrawing**                   | RFK Jr. suspended his campaign and endorsed Trump, but remained on ballots and did not legally terminate the campaign in the clean way some traders expected. The core bug was using ordinary political shorthand like “drops out” without specifying legal/electoral criteria. ([CoinDesk][10])                                             |
| **Ethereum ETF approved by May 31**                | Polymarket | **What counts as “approved”?**                           | SEC approval of 19b-4 filings happened, but S-1 effectiveness/trading approval came later. The market turned on whether “ETF approved” meant one procedural approval, full launch approval, or credible media consensus. ([DL News][11])                                                                                                     |
| **Titan submarine “found” by June 23**             | Polymarket | **Found object vs debris vs confirmation timing**        | This older case became a canonical “what does found mean?” problem: wreckage/debris, official confirmation, and time cutoff did not map cleanly onto a binary question. I’d include it as an early Polymarket semantic-resolution case, though the public record is less tidy than the 2025–26 cases. ([DL News][12])                        |
| **Israel invades Lebanon in September 2024**       | Polymarket | **Geopolitical term ambiguity**                          | “Invasion” is a messy term: cross-border raids, ground incursions, occupation, official declarations, and media phrasing can diverge. PredictionNews explicitly cited the market as an example of incorrect/ambiguous resolution. ([PredictionNews][13])                                                                                     |
| **Trump spoke to Xi in March 2026**                | Polymarket | **Claim by one party vs credible-source confirmation**   | Trump claimed he had spoken with Xi; China did not confirm. The issue became whether a politician’s statement was enough, or whether credible-source consensus was required. Polymarket’s intervention may have prevented a bad outcome, but the case belongs because the market sentence itself was under-specified. ([PredictionNews][14]) |
| **UFC 327 winner later corrected to draw**         | Kalshi     | **Initial official result vs corrected official result** | Kalshi resolved based on the initial decision, then scorecards were corrected to a draw. The rules may have supported using the initial decision, but the market outcome no longer matched the final real-world sports result. ([PredictionNews][4])                                                                                         |
| **Kalshi X CEO market title change**               | Kalshi     | **Title/rules mismatch**                                 | Kalshi reportedly changed a market title before resolution because the original title was telling users the wrong thing relative to the rules. This is a softer case, but important: market title is what many traders actually price, while the fine print does the legal work. ([Next Event Horizon][15])                                  |

---

## Tier 3 — lower-confidence, Reddit-heavy, or “near miss” cases worth tracking

These are less cleanly documented, but I would keep them in a research appendix because they fit the same pattern and had at least some visible user uproar.

| Case                                                                                | Platform   | Why I’d keep it on the radar                                                                                                                                                                                                                                                                   |
| ----------------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Polymarket Astros/Dodgers wrong winner**                                          | Polymarket | Event Horizon described a sports market where the Astros beat the Dodgers 18–1 but the market was initially resolved as Dodgers winning, allegedly due to broken/malicious bots; Polymarket later said Astros bettors were paid. Operational failure, if confirmed. ([Next Event Horizon][16]) |
| **Kalshi 49ers point-total source listed as San Francisco Unified School District** | Kalshi     | Looks like a listing/source bug rather than final wrong settlement, but it is exactly the kind of source-specification failure that can become a resolution problem. ([Next Event Horizon][17])                                                                                                |
| **Kalshi executive-order count market**                                             | Kalshi     | Reddit users argued the source/count for Trump executive orders did not match what Kalshi was using. I would not rely on this without more evidence, but it fits the “official source vs platform interpretation” bucket. ([Reddit][18])                                                       |
| **Kalshi weather/NWS corrected temperature report**                                 | Kalshi     | Reddit users claimed Kalshi settled based on an incorrect NWS figure that was later corrected. This is structurally similar to Oscars and UFC: initial authoritative data vs corrected authoritative data. ([Reddit][19])                                                                      |
| **Trump sues Wall Street Journal**                                                  | Kalshi     | Semantic/legal-entity ambiguity: Trump sued people/entities connected to WSJ, including Dow Jones/News Corp/Murdoch/reporters, but users debated whether that counted as suing “The Wall Street Journal.” This may be defensible as Yes, but it is a useful edge case. ([Reddit][20])          |
| **Government shutdown duration / UTC vs ET cutoff**                                 | Kalshi     | Reddit-only evidence, but users alleged a timing convention mismatch around whether a shutdown crossed the 43-day threshold. Time zones are a classic resolution footgun. ([Reddit][21])                                                                                                       |

---

## Adjacent but not exactly “platform messed up”

These are important for the broader thesis, but I would not classify them as clean resolution failures.

| Case                                            | Why adjacent                                                                                                                                                                                                                                      |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Iran strikes Israel / reporter pressure**     | The market was reportedly clear enough, but traders pressured/threatened a journalist whose reporting affected resolution. This is a source-pressure/adversarial-ground-truth problem, not necessarily a platform mistake. ([PredictionNews][22]) |
| **War-map / source manipulation cases**         | These belong in the broader “prediction markets can pressure or manipulate sources of truth” category. Some may become resolution failures, but they need case-by-case verification.                                                              |
| **Insider-trading / information-leakage cases** | Important market-integrity failures, but not resolution failures unless the final outcome itself was wrong or ambiguous.                                                                                                                          |

---

## The pattern

The genuine cases cluster into a few repeatable failure modes:

1. **Event happened vs event was confirmed before deadline**
   Strategy BTC sale, Oscars final data, UFC corrected result, weather corrections.

2. **Ordinary-language category has fuzzy boundaries**
   Zelenskyy “suit,” Cardi B “performance,” RFK “drops out,” TikTok “ban,” Ethereum ETF “approved.”

3. **Title says one thing, fine print says another**
   Khamenei “out,” Kalshi X CEO title change, Wall Street Journal lawsuit, maybe Oscars.

4. **Oracle/source/governance can be gamed or contradicted**
   Ukraine minerals deal, Barron/$DJT, Trump-Xi call, Israel/Lebanon invasion semantics.

5. **Plain operational settlement failures**
   Kalshi NFL futures, NBA preseason, Polymarket Astros/Dodgers.

The highest-quality “case law” set, in my view, is:

**Strategy BTC sale, Zelenskyy suit, Ukraine minerals deal, Barron/$DJT, Oscars viewership, Cardi B performance, Khamenei death carveout, RFK dropout, TikTok ban, Ethereum ETF approval, Titan sub found, Kalshi NFL futures, Kalshi NBA preseason, UFC corrected draw.**

Those are the ones I’d build the core argument around.

[1]: https://www.galaxy.com/insights/research/strategy-bitcoin-sale-polymarket-resolution-dispute-may-2026 "Strategy Sold Bitcoin in May. Polymarket Says It Didn't. | Galaxy"
[2]: https://www.wired.com/story/volodymyr-zelensky-suit-polymarket-rebellion "Volodymyr Zelensky’s Clothing Has Sparked a Polymarket Rebellion | WIRED"
[3]: https://cryptoslate.com/polymarket-faces-backlash-over-resolving-disputed-7-million-trump-ukraine-market/ "Polymarket faces backlash over resolving disputed $7 million Trump-Ukraine market"
[4]: https://predictionnews.com/news/kalshi-ufc-resolution-echoes-2025-oscars-viewership-market "Kalshi UFC Resolution Echoes 2025 Oscars Viewership Market — PredictionNews"
[5]: https://apnews.com/article/d3b51d8848934d69c39ff92fa2c51278 "Cardi B's cameo in Bad Bunny's Super Bowl halftime show sparks debate on prediction markets | AP News"
[6]: https://www.reuters.com/world/middle-east/kalshi-sued-over-ouster-iran-leader-prediction-market-2026-03-06/ "Kalshi sued over ouster of Iran leader prediction market | Reuters"
[7]: https://nexteventhorizon.substack.com/p/why-wasnt-kalshi-paying-traders-that-won-nfl-futures "Why Wasn't Kalshi Paying Traders That Won NFL Futures Bets?"
[8]: https://nexteventhorizon.substack.com/p/kalshi-resolved-two-nba-preseason-games-wrong "Kalshi Resolved Two NBA Preseason Games Early And With The Wrong Winner"
[9]: https://www.tradingview.com/news/cointelegraph%3A3f4adad24094b%3A0-polymarket-faces-backlash-over-tiktok-ban-prediction-resolution/ "Polymarket faces backlash over TikTok ban prediction resolution — TradingView News"
[10]: https://www.coindesk.com/markets/2024/08/26/did-rfk-jr-really-drop-out-polymarket-bettors-argue-over-contract-resolution "Did RFK Jr. Really 'Drop Out'? Polymarket Bettors Argue Over Contract Resolution"
[11]: https://www.dlnews.com/articles/web3/ethereum-etf-ok-may-prompt-11-million-row-on-polymarket/ "Ethereum ETF approval will cause an $11m dispute on Polymarket — here’s why - DL News"
[12]: https://www.dlnews.com/articles/markets/crypto-bets-on-titan-sub-cause-uproar-at-uma-polymarket/?utm_source=chatgpt.com "Crypto bettors' uproar over Titan submarine puts spotlight on ..."
[13]: https://predictionnews.com/politics/polymarkets-quandary-defining-an-invasion?utm_source=chatgpt.com "Polymarket's Quandary: Defining an Invasion"
[14]: https://predictionnews.com/news/polymarket-overrules-uma-voters-in-trump-xi-call-market "Polymarket Overrules UMA Voters in Trump-Xi Call Market — PredictionNews"
[15]: https://nexteventhorizon.substack.com/p/kalshi-changed-the-title-of-a-market?utm_source=chatgpt.com "Kalshi Changed The Title Of A Market About X's CEO, And It ..."
[16]: https://nexteventhorizon.substack.com/p/the-debacle-that-is-polymarket?utm_source=chatgpt.com "The Debacle That Is Polymarket And Betting On Ukraine's ..."
[17]: https://nexteventhorizon.substack.com/p/why-is-kalshi-saying-a-school-district-is-source-for-nfl-markets?utm_source=chatgpt.com "Why Is Kalshi Saying A School District Is The Source For Who ..."
[18]: https://www.reddit.com/r/Kalshi/comments/1i7d8d4/how_does_one_dispute_a_kalshi_outcome_anyone_else/?utm_source=chatgpt.com "How does one dispute a Kalshi outcome? Anyone else ..."
[19]: https://www.reddit.com/r/Kalshi/comments/1h1zjhb/were_you_impacted_by_kalshis_incorrect_resolution/?utm_source=chatgpt.com "Were you impacted by Kalshi's incorrect resolution of the “ ..."
[20]: https://www.reddit.com/r/Kalshi/comments/1m6t4qr/can_someone_help_me_understand_kalshis_resolution/?utm_source=chatgpt.com "Can someone help me understand Kalshi's resolution of ..."
[21]: https://www.reddit.com/r/Kalshi/comments/1pmvnnc/kalshi_is_scamming_right_now/?utm_source=chatgpt.com "Kalshi is scamming right now"
[22]: https://predictionnews.com/news/death-threats-the-newest-resolution-manipulation-attempt "Death Threats: The Newest Resolution Manipulation Attempt — PredictionNews"


From Grok:
**Method I used (and reviewed iteratively for thoroughness):**  
To find *every* documented instance (not just the famous ones), I started with broad web searches for terms like “Kalshi controversial resolutions / bad resolutions / outcry / backlash” and the same for Polymarket/UMA disputes, plus targeted queries on “defirate.com resolution controversies,” Substack/Reddit/news. This surfaced the key aggregator article on defirate.com (which maintains the closest thing to compiled tables). I then evolved the search: extracted every new incident from those results and ran specific follow-ups (e.g., “Kalshi UFC 327 resolution,” “Polymarket Clavicular pregnancy dispute,” “Kalshi Stephen Miran misresolved”). I cross-checked X keyword/semantic searches for real-time trader outcry (engagement, Discord/Reddit storms) and platform docs.  

**Evaluation criteria (reviewed after each batch of results):** Only included *legitimate* cases with verifiable public backlash—high trading volume, media coverage (Forbes, WSJ, PredictionNews, Bloomberg, The Defiant, Substack analysts like Dustin Gouker), lawsuits/CFTC complaints, or widespread trader frustration on Discord/Reddit/X. Excluded pure legal/gaming-law suits, insider-trading enforcement, or isolated gripes without evidence of broader outrage. Prioritized resolution-specific issues (factual errors, rigid rules vs. spirit, whale votes, data-source rigidity). This yielded a more exhaustive list than prior responses; defirate.com tables + cross-references confirm these are the main ones through mid-2026. No single “hall of shame” site exists, but these are the documented public outcries.

Here is the most complete list of legitimate public outcry moments (high-volume or high-profile, with clear trader/platform backlash):

### Kalshi (centralized team resolutions → errors or rigid “initial data only” rules)
Kalshi’s issues cluster around operational mistakes or strict contract wording (“no post-expiration revisions,” initial announcements count).

- **Oscars Viewership (2025)**: Settled “No” on preliminary Nielsen fast nationals (~18.1M viewers). Final numbers (~19.7M, including streaming) flipped it to “Yes.” Traders noted media called prelims non-final; Kalshi stuck to initial release per rules. Backlash: “Yell at them in Discord” was the only suggested recourse; platform conceded it “did not capture the spirit” but called it “legal and correct.” No reversal.

- **NFL Season Win Totals misgraded (Jan 2026)**: Multiple markets (e.g., 49ers over 10.5—they won 12) resolved early/incorrectly. Winners initially got only stakes refunded. Massive Discord/X outcry + Dustin Gouker Substack (>1M views) forced reversal: full $1 payouts issued. Clear operational error fixed under pressure.

- **Ali Khamenei “Out as Supreme Leader” (Feb–Mar 2026)**: ~$54M volume. After death in strikes, Kalshi invoked “death carveout” and settled at last traded price (not full Yes). Accusations of “hidden” rule, “bait-and-switch,” deceptive marketing. Class-action lawsuit filed; Kalshi reimbursed net losses + fees (~$2.2M) but did not reverse to full Yes. Major Capitol Hill scrutiny.

- **Cardi B Super Bowl Halftime (Feb 2026)**: $47M+ volume. Ambiguity whether Cardi B (dancing/mouthing lyrics in Bad Bunny’s set) counted as “performance.” Kalshi used Rule 6.3(c) to settle at last traded price (favoring No). Subjective interpretation sparked CFTC complaint and widespread trader frustration.

- **Sanders Greensboro Rally mention market (Feb 2026)**: $3.6M volume. Resolved No despite video evidence of Sanders using the exact words. Reddit/Trustpilot backlash; Kalshi later revised contract language for future markets.

- **UFC 327 prelim (Padilla vs. Mederos, Apr 11 2026)**: Initial Bruce Buffer announcement: Padilla win. Minutes later, UFC corrected scoring error to majority draw. Kalshi paid out on initial announcement per rules (“revisions after expiration not considered”). Direct parallel to Oscars controversy; PredictionNews headline: “Kalshi UFC Resolution Echoes 2025 Oscars Viewership Market.” No reversal despite live correction and fighter protest (denied by commission).

- **Stephen Miran contracts (recent 2026)**: Trader reported misresolution; filed formal CFTC complaint citing precedent and lack of response. Acknowledged by Kalshi support but unresolved publicly. Smaller-scale but fits pattern of rigid data-source issues.

### Polymarket (UMA Optimistic Oracle + token-holder votes)
Issues center on ambiguous wording, whale influence (~20% of judges with financial ties per analyses), or strict “confirmation timing” rules.

- **Ukraine mineral deal with Trump (Mar 2025)**: $7M+ volume. Resolved Yes via UMA whale (~25% vote via 3 accounts) despite no confirmed deal at deadline (signed later). Polymarket called it “unprecedented governance attack”; no refunds. Major backlash over manipulation.

- **Zelenskyy “wear a suit” (Jul 2025)**: ~$14M–$160M volume. Photos showed formal attire (called a “suit” by media/experts). UMA reversed initial Yes to No. Outcry over subjective interpretation and whale influence; Polymarket/UMA faced “disinformation engine” accusations.

- **Venezuela “Invasion” (Jan 2026)**: $10.5M+ volume. U.S. captured Maduro; resolved No because contract required specific “control over territory” wording. Payouts withheld; traders argued real-world event should have paid Yes. Significant frustration.

- **MicroStrategy (Strategy) Bitcoin sale (May–Jun 2026)**: $60M+ volume. Company sold 32 BTC in-window (confirmed in 8-K). Resolved No because public filing was post-deadline. Multiple disputes → UMA vote upheld No. Huge outcry (“event happened but market said no”); calls for UMA reform.

- **Clavicular pregnancy market (Apr 2026)**: $16M+ volume. Disputed twice through UMA rounds; prominent trader (Domahhhh) called UMA a “disinformation engine run by rogue traders.” Part of pattern with prior whale controversies; ongoing scrutiny.

- **Hezbollah cease-fire / other recent UMA disputes (2026)**: WSJ highlighted “mysterious crypto judges” with potential conflicts; multiple high-stakes votes drew unease over anonymous token-holder influence.

Rare refund precedent: Barron Trump “involved in DJT” market—Polymarket overrode UMA and refunded both sides (only known full refund case).

**Broader notes**: These represent the documented public outcries through June 2026. Kalshi fixes sometimes happen under social-media pressure (NFL); Polymarket rarely refunds once UMA finalizes. Defirate.com’s settlement article is the best ongoing reference for tables. Prediction markets are maturing, so new edge cases will arise—always read full rules. This list is as exhaustive as public sources allow; no hidden comprehensive tracker exists.