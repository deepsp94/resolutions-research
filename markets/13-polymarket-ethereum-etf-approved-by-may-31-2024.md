# Polymarket: Ethereum ETF approved by May 31, 2024

## Bottom line

**Finding: Failure — a rule-drafting failure that produced a defensible-but-contested resolution. The binding rule asked whether a spot Ethereum ETF would "receive approval from the SEC" by May 31, 2024 but never defined "approval," and the SEC's two-step process made that ambiguity outcome-determinative. The market resolved Yes on the May 23 19b-4 listing approval — one of two required SEC steps — while the products remained barred from trading pending S-1 effectiveness, which did not occur until July. Confidence: medium.**

Polymarket asked whether any spot Ethereum ETF would receive SEC approval by May 31, 2024. The gamma-verified rule resolves Yes "if any spot Ethereum ETF receives approval from the SEC by May 31, 2024, 11:59:59 PM ET," with SEC information as the primary source and "a consensus of credible reporting" as a backup.[^gamma] It does **not** define "approval" — it never names Rule 19b-4 approval, S-1 registration-statement effectiveness, listing, launch, or first trading as the controlling milestone.[^gamma] The market resolved **Yes** (gamma `outcomePrices` = `["1","0"]`, `umaResolutionStatus: resolved`, closed 2024-05-24).[^gamma]

The trigger was the SEC's May 23, 2024 order (Release No. 34-100224), titled "Order Granting Accelerated Approval of Proposed Rule Changes... to List and Trade Shares of Ether-Based Exchange-Traded Products."[^sec-order] That order approved only the **19b-4** exchange-listing step. The products were not cleared to trade: contemporaneous primary reporting confirmed the SEC still had to make each issuer's **S-1 registration statement** effective before investors could buy in, a separate review.[^coindesk][^mayerbrown] Spot ether ETFs did not begin trading until **July 23, 2024** — after the deadline.[^investopedia-july]

The failure is in the drafting, not in a clear misgrade. The rule used broad everyday "approval" language for a known two-step regulatory process, then resolved on the earlier, partial step. The ambiguity was foreseeable — DL News warned of a large dispute *before* the decision, and industry experts publicly held that an ETF is not "approved" until both the 19b-4 and the registration form are signed off.[^dlnews][^cointelegraph] Because the SEC did issue a literal "approval" order and major outlets used broad approval language, the Yes resolution was **not baseless**; this is best read as a drafting failure yielding a defensible-but-contested outcome, not a clean misresolution.

## Market details

- **Venue:** Polymarket
- **Market:** "Ethereum ETF approved by May 31?" — gamma event id `903219`, market id `253750`, conditionId `0x4fdc8c72f3013001dccc152e318cb3fcb16da16c741816c3078a42947702ece5`.[^gamma]
- **Governing rule (gamma, verbatim):** "This market will resolve to \"Yes\" if any spot Ethereum ETF receives approval from the SEC by May 31, 2024, 11:59:59 PM ET. Otherwise, this market will resolve to \"No\". The primary resolution source for this market will be information from the SEC, however a consensus of credible reporting may also be used."[^gamma]
- **Definition of "approval":** **None.** The rule does not specify 19b-4 approval, S-1 effectiveness, listing, launch, or first trading.[^gamma]
- **Outcome:** Yes — `outcomePrices` = `["1","0"]`; `umaResolutionStatus: resolved`; `closed: true`; closedTime / umaEndDate 2024-05-24T00:14:40Z; `resolvedBy` `0x6A9D222616C90FcA5754cd1333cFD9b7fb6a4F74`; `umaBond` 500, `umaReward` 5.[^gamma]
- **Displayed volume:** about $13.2 million.[^gamma]
- **Disputes:** The Yes resolution was disputed on UMA before settling Yes. Press confirms it "was briefly disputed but ultimately resolved with the same Yes outcome."[^cointelegraph] The often-cited "two disputed Yes proposals" sequence is **INFERRED from the Polymarket page UI**; the gamma response does not retain a dispute array, so the exact count is not independently verified here.

## What happened

There were two distinct SEC-controlled milestones for a spot ether ETF, and the rule's word "approval" did not say which one counted.[^gamma][^dlnews]

First, exchanges needed SEC approval of proposed rule changes under Rule 19b-4 to list and trade the shares. On **May 23, 2024**, the SEC issued Release No. 34-100224 granting accelerated approval of the 19b-4 rule changes for NYSE Arca, Nasdaq, and Cboe BZX covering eight ether-based products.[^sec-order] The market resolved Yes on this order.[^gamma][^cointelegraph]

Second, each issuer's registration statement (Form S-1) still had to become effective before the products could be offered or traded. As of May 23 those statements remained under SEC review. CoinDesk reported the same day that the ETFs were "not yet cleared to trade... the regulator must approve their S-1 filings before investors can buy them."[^coindesk] Mayer Brown's May 30 alert confirmed the registration statements "remain under review by the SEC... through a separate review process."[^mayerbrown] Spot ether ETFs began trading **July 23, 2024**.[^investopedia-july]

Ahead of the decision, DL News reported that Polymarket users were already preparing for the largest dispute in the platform's history precisely because the rule did not specify which filing must be approved.[^dlnews] After the May 23 order, the Yes resolution drew backlash and a UMA dispute before settling Yes.[^cointelegraph]

## The allegation against Polymarket

The core allegation is that Polymarket treated approval of one required SEC step as approval of the ETF itself. "No" holders argued a U.S. ETF needs both an approved 19b-4 filing and an effective Form S-1 to begin trading, so without the S-1 there should be no "Yes."[^cointelegraph] They pointed to contemporaneous expert consensus: VanEck's Matthew Sigel ("ETFs are not considered 'approved' until both the relevant registration form... & the 19b-4 filing have been signed off on by the SEC") and Bitwise's Matt Hougan describing it as a two-key scenario requiring both filings to "turn."[^cointelegraph]

The objection is not mere pedantry. The SEC's own order approved only the listing step, and the products could not trade until the separate S-1 process completed.[^sec-order][^coindesk] If the market asked whether a spot ether ETF had been "approved by the SEC," ordinary traders could reasonably expect full SEC clearance, not approval of only the exchange-rule component.

## Polymarket's basis for Yes

Two grounds gave Yes a real basis, both verifiable from primary sources:

1. **A literal SEC approval order existed.** The rule said "receives approval from the SEC," and Release No. 34-100224 is, on its face, an SEC order "Granting Accelerated Approval" of rule changes "to List and Trade Shares of Ether-Based Exchange-Traded Products," dated May 23, 2024 — before the deadline.[^sec-order][^gamma]
2. **Credible reporting used broad approval language.** The rule allowed "a consensus of credible reporting" as a source, and many outlets headlined the May 23 event as SEC approval of spot ether ETFs.[^gamma][^cointelegraph]

That basis explains why Yes was plausible. It does not eliminate the failure: the rule used broad product-approval language for a multi-step SEC process and then resolved on the earlier, partial step without ever telling traders that 19b-4 approval alone would count.

## Assessment

### Did the SEC approve the 19b-4 listing rule changes before May 31?

**Yes.** Release No. 34-100224, dated May 23, 2024, granted accelerated approval of the 19b-4 proposed rule changes to list and trade shares of multiple ether-based products.[^sec-order]

### Were the spot ether ETFs cleared by the SEC to trade before May 31?

**No.** The products could not trade until each issuer's S-1 registration statement became effective — a separate SEC review still pending on May 23. Spot ether ETFs began trading July 23, 2024.[^coindesk][^mayerbrown][^investopedia-july]

### Did the rule specify that 19b-4 approval alone was enough?

**No.** The gamma-verified rule said only "receives approval from the SEC." It did not name 19b-4 approval, S-1 effectiveness, listing, launch, or first trading as the controlling milestone.[^gamma]

### Was the Yes resolution baseless?

**No.** The May 23 approval order and the contemporaneous broad "approval" media language gave Yes a genuine basis, and "consensus of credible reporting" was an allowed source.[^sec-order][^gamma][^cointelegraph]

### Was this a failure?

**Yes — a rule-drafting failure.** The market used everyday "approval" language for a two-step SEC process and did not tell traders that the earlier 19b-4 step alone would resolve Yes. The ambiguity was foreseeable (flagged before the decision) and outcome-determinative, and the resolution landed on the partial milestone.[^dlnews][^cointelegraph][^gamma]

### Overall classification

- **Rule-drafting failure:** Yes — "approval" undefined for a known two-step process
- **Clear misresolution:** No — Yes had a literal SEC-order basis and broad media support
- **Yes-side basis:** Real (an actual SEC approval order, plus broad reporting)
- **No-side basis:** Stronger under a full-clearance / launch reading (S-1 pending, no trading until July)
- **Best public verdict:** Failure (drafting failure producing a defensible-but-contested resolution)

## Precise blocker to a stronger finding

Two blockers keep this short of a clean misresolution. First, the rule did not define "approval," so the Yes resolution cannot be called baseless — a literal SEC approval order existed before the deadline. Second, the exact UMA dispute sequence (the "two disputed Yes proposals" commonly cited) is inferred from the Polymarket page UI rather than verified from primary data; gamma confirms only that the question was disputed and ultimately resolved Yes. Neither blocker prevents classifying the case as a failure, because the ambiguity was foreseeable and outcome-determinative.

## Sources

[^gamma]: Polymarket gamma API, `https://gamma-api.polymarket.com/events?slug=ethereum-etf-approved-by-may-31` (event id 903219; market id 253750). Verbatim rule: "This market will resolve to \"Yes\" if any spot Ethereum ETF receives approval from the SEC by May 31, 2024, 11:59:59 PM ET..."; `outcomePrices` `["1","0"]` (Yes); `umaResolutionStatus: resolved`; `closed: true`; closedTime/umaEndDate 2024-05-24T00:14:40Z; volume ~$13.23M. Primary source for rule text and settled outcome. [Gamma][gamma]

[^sec-order]: U.S. Securities and Exchange Commission, Release No. 34-100224, May 23, 2024, "Order Granting Accelerated Approval of Proposed Rule Changes, as Modified by Amendments Thereto, to List and Trade Shares of Ether-Based Exchange-Traded Products" (File Nos. SR-NYSEARCA-2023-70 et al.). Approves the 19b-4 listing rule changes for NYSE Arca, Nasdaq, and Cboe BZX. Title and date confirmed via Federal Register (FR-2024-05-30) and the SEC PDF. [Order PDF][sec-order] · [Federal Register][fed-reg]

[^coindesk]: Helene Braun, CoinDesk, "Ether ETFs Clear Major Hurdle, Though SEC Hasn't Cleared Them for Trading Yet," May 23, 2024. "They are not yet cleared to trade... the regulator must approve their S-1 filings before investors can buy them." [Article][coindesk]

[^mayerbrown]: Mayer Brown, "SEC Approves Listings of Spot Ether ETFs: Waiting is the Hardest Part," May 30, 2024. Confirms the SEC approved the 19b-4 rule changes but the registration statements "remain under review by the SEC... through a separate review process." [Alert][mayerbrown]

[^investopedia-july]: Investopedia, "SEC Approves Spot Ether ETFs," July 2024. Spot ether ETFs received final/effective registration and began trading July 23, 2024 — after the May 31 deadline. [Article][investopedia-july]

[^dlnews]: Ryan Celaj, DL News, "Ethereum ETF approval will cause an $11m dispute on Polymarket — here's why," May 23, 2024. Pre-decision: issuers must get approval for both 19b-4 and S-1 filings; "Thursday's decision is for only the 19b-4 filing"; warns of the largest dispute in Polymarket's history over what "approval" means. [Article][dlnews]

[^cointelegraph]: Cointelegraph, "Polymarket gets backlash over 'approved' outcome on $13M Ethereum ETF bets," May 23–24, 2024 (via TradingView). Market "closed at a Yes result on May 23... briefly disputed but ultimately resolved with the same Yes outcome." Quotes VanEck's Matthew Sigel and Bitwise's Matt Hougan on the dual 19b-4 + registration-form requirement. [Article][cointelegraph]

[gamma]: https://gamma-api.polymarket.com/events?slug=ethereum-etf-approved-by-may-31
[sec-order]: https://www.sec.gov/files/rules/sro/nysearca/2024/34-100224.pdf
[fed-reg]: https://www.govinfo.gov/content/pkg/FR-2024-05-30/html/2024-11804.htm
[coindesk]: https://www.coindesk.com/markets/2024/05/23/sec-approves-spot-ether-etf-listing-still-needs-to-approve-products
[mayerbrown]: https://www.mayerbrown.com/en/insights/publications/2024/05/sec-approves-listings-of-spot-ether-etfs-waiting-is-the-hardest-part
[investopedia-july]: https://www.investopedia.com/sec-approves-spot-ether-etfs-8678873
[dlnews]: https://www.dlnews.com/articles/web3/ethereum-etf-ok-may-prompt-11-million-row-on-polymarket/
[cointelegraph]: https://cointelegraph.com/news/polymarket-gets-backlash-over-approved-outcome-13-million-ethereum-etf-bet
