# Kalshi: Trump sues The Wall Street Journal

## Bottom line

**Finding: No failure. The binding contract resolves Yes once Trump files a lawsuit against the Wall Street Journal, the actual complaint explicitly names "Dow Jones & Company, Inc. d/b/a The Wall Street Journal" as the lead defendant, and the contract's source list includes the federal court record (PACER) where that complaint is filed. The Yes settlement was a correct application of the rule. Confidence: high.**

Kalshi's `KXDJTWSJ` market — "Will Trump sue WSJ before September?" — resolved **Yes** and is marked Determined.[^market] A trader objected that the Wall Street Journal "was never named explicitly," since the suit also named Dow Jones, News Corp, Rupert Murdoch, Robert Thomson, and two reporters.[^reddit] That objection is refuted by the complaint itself: Trump's July 18, 2025 lawsuit is captioned **"Dow Jones & Company, Inc. d/b/a The Wall Street Journal, a Delaware corporation, News Corporation..."** and its opening line says Trump "sues Defendants, Dow Jones & Company, Inc. d/b/a The Wall Street Journal."[^complaint][^docket] "The Wall Street Journal" is named — as the registered "doing-business-as" name of its publisher.

The contract's standard is not a loose "consensus of credible reporting" test, either. It resolves on "reporting from the Source Agencies," an enumerated list that includes **PACER** (the federal courts' records system) alongside the parties and major outlets.[^terms] The filed complaint is therefore admissible primary evidence, and every listed outlet reported the filing. This is a clean **No failure**.

## Market details

- **Venue:** Kalshi
- **Market:** `KXDJTWSJ`, "Will Trump sue WSJ before September?" — `entity_1` = Donald J. Trump, `entity_2` = Wall Street Journal, deadline September 1, 2025.[^market]
- **Governing contract:** the `SUE` terms, CFTC-certified February 7, 2025 and listed February 8, 2025 — predating the July 2025 lawsuit.[^cert]
- **Payout Criterion:** Yes if `entity_1` "has filed a lawsuit or some other formal adversarial legal process (such as pre-complaint discovery or an arbitration claim) against `entity_2` after Issuance and before `<date>`."[^terms]
- **Source standard:** "reporting from the Source Agencies" — an enumerated list (PACER, the parties, NYT, AP, Bloomberg, Reuters, Axios, Politico, Semafor, The Information, The Washington Post, The Wall Street Journal, ABC, CBS, CNN, Fox News, MSNBC, NBC).[^terms]
- **Outcome:** Yes; Determined.[^market]

## What happened

On July 18, 2025, Donald Trump filed a defamation suit in the U.S. District Court for the Southern District of Florida (`1:25-cv-23232`, *Trump v. Murdoch*) over the Journal's reporting on a birthday letter tied to Jeffrey Epstein.[^complaint][^docket][^ap] The named defendants are **Dow Jones & Company, Inc. d/b/a The Wall Street Journal**, News Corporation, Keith Rupert Murdoch, Robert Thomson, and reporters Khadeeja Safdar and Joseph Palazzolo.[^complaint] Major outlets on the contract's source list — including the Associated Press — reported it as Trump suing the Wall Street Journal.[^ap]

The filing occurred after the contract's February 2025 issuance and before the September 1, 2025 deadline, satisfying the Payout Criterion. Kalshi resolved the market Yes.[^market]

## The allegation against Kalshi

The objection is a strict legal-entity reading: that "The Wall Street Journal" was not itself a captioned defendant — only Dow Jones (its publisher), News Corp (its parent), executives, and reporters were — so a market specifically about suing "the Wall Street Journal" should not resolve Yes.[^reddit]

The objection would have force if the WSJ were absent from the caption. It is not.

## Kalshi's basis for Yes

Two independent grounds support the Yes resolution, both verifiable from primary sources:

1. **The WSJ is named in the complaint.** The lead defendant is "Dow Jones & Company, Inc. d/b/a The Wall Street Journal."[^complaint] A "d/b/a" designation is the legal mechanism by which the Wall Street Journal — which is not a separately incorporated entity but a publication of Dow Jones — is named as a party. Suing "Dow Jones d/b/a The Wall Street Journal" is suing the Wall Street Journal.

2. **The contract's source standard captures it.** The rule resolves on "reporting from the Source Agencies," which include PACER and the WSJ itself, not a subjective consensus threshold.[^terms] The filed complaint (on PACER) and the contemporaneous reporting by listed outlets both document that Trump filed suit against the Wall Street Journal.[^complaint][^ap]

## Assessment

### Did Trump file a qualifying lawsuit before the deadline?

**Yes.** A defamation complaint was filed July 18, 2025 — a "lawsuit... formal adversarial legal process" under the Payout Criterion — well before September 1.[^complaint][^terms]

### Was the Wall Street Journal a named defendant?

**Yes.** The caption and first sentence name "Dow Jones & Company, Inc. d/b/a The Wall Street Journal."[^complaint][^docket] The trader claim that "WSJ was never named explicitly" is factually incorrect.

### Did the contract rely on a vague "consensus of credible reporting" standard?

**No.** It relies on "reporting from the Source Agencies," a fixed enumerated list that includes the federal court record (PACER) and the WSJ itself.[^terms] That is more objective than a consensus test and is independently satisfied by the filed complaint.

### Was the resolution correct, not merely defensible?

**Correct.** Earlier framing treated this as an ambiguous edge case salvaged by ordinary-language reporting. With the binding contract and the complaint in hand, the Yes resolution is a direct, correct application of the rule: a lawsuit was filed against the named entity before the deadline, documented by admissible sources.

### Overall classification

- **Final misresolution:** None
- **Legal-entity ambiguity:** Not material — the WSJ is a named defendant via its publisher's d/b/a
- **Source-rule ambiguity:** None — enumerated Source Agencies, including PACER
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

None. The decisive facts are verified from primary sources: the `SUE` contract terms and February 2025 certification, the Kalshi market page showing the rule and the Yes/Determined outcome, and the filed complaint naming "Dow Jones & Company, Inc. d/b/a The Wall Street Journal." The prior blocker (missing contract and source language) is resolved.

## Sources

[^terms]: Kalshi, `SUE` contract terms (binding rules). Payout Criterion: Yes if `entity_1` "has filed a lawsuit or some other formal adversarial legal process... against `entity_2` after Issuance and before `<date>`." Underlying is "reporting from the Source Agencies"; the Source Agencies are an enumerated list including PACER, the parties, and named major outlets. [PDF][terms]

[^cert]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification for the `SUE` contract, dated February 7, 2025 (listed February 8, 2025) — predating the July 2025 lawsuit. [Cert][cert]

[^market]: Kalshi, market page `KXDJTWSJ-25`, "Will Trump sue WSJ before September?" Rule: "Resolves Yes if Donald J. Trump sues Wall Street Journal before Sep 1, 2025"; a lawsuit or formal adversarial process qualifies. Outcome: Yes, Determined. [Market][market]

[^complaint]: *Trump v. Murdoch*, complaint filed July 18, 2025, U.S. District Court, S.D. Fla. Caption and opening line name "Dow Jones & Company, Inc. d/b/a The Wall Street Journal," News Corporation, Keith Rupert Murdoch, Robert Thomson, Khadeeja Safdar, and Joseph Palazzolo. [Complaint PDF][complaint]

[^docket]: CourtListener docket, *Trump v. Murdoch*, No. 1:25-cv-23232 (S.D. Fla.), filed July 18, 2025. [Docket][docket]

[^ap]: Associated Press, "Trump sues Wall Street Journal and media mogul Rupert Murdoch over reporting on Epstein ties," July 18, 2025. A listed Source Agency reporting the filing as Trump suing the Wall Street Journal. [AP][ap]

[^reddit]: Reddit, r/Kalshi, "Can someone help me understand Kalshi's resolution of the Trump vs WSJ lawsuit market?" July 2025. States the Yes resolution and the legal-entity objection. [Thread][reddit]

[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/SUE.pdf
[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/SUE.pdf
[market]: https://kalshi.com/markets/kxdjtwsj/djt-wsj-suit/kxdjtwsj-25
[complaint]: https://storage.courtlistener.com/recap/gov.uscourts.flsd.693830/gov.uscourts.flsd.693830.1.0.pdf
[docket]: https://www.courtlistener.com/docket/70843413/trump-v-murdoch/
[ap]: https://apnews.com/article/trump-jeffrey-epstein-grand-jury-justice-department-ece8a837f9bd179771f801a765e242e4
[reddit]: https://www.reddit.com/r/Kalshi/comments/1m6t4qr/can_someone_help_me_understand_kalshis_resolution/
