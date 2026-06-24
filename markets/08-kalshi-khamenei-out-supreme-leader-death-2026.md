# Kalshi: Ali Khamenei out as Supreme Leader (death carveout)

## Bottom line

**Finding: No failure. The governing `WLEADEROUT` contract carved death out of ordinary $1 binary settlement before Khamenei was killed, and that carveout is provable from primary sources predating the death: the May 15, 2025 CFTC product certification (contract listed May 16, 2025) and Wayback CDX records showing the terms PDF byte-identical across the February 28, 2026 death. When Khamenei was killed, Kalshi paused the market and settled on the last traded price before death under that rule — a correct application of the written contract — and reimbursed confused traders (~$2.2M). The live class action's own theory concedes the carveout existed and attacks UI disclosure and last-price methodology, not the contract. Failure-resolved: N/A. Confidence: high on the contract and its timing; medium on the pre-death UI display and the last-price methodology.**

After Khamenei was killed on February 28, 2026, traders who held "Yes" on "Ali Khamenei out as Supreme Leader?" expected $1 payouts and did not get them. Kalshi paused the market under Rule 13.1 and applied a death carveout, settling on the last traded price before death rather than as an ordinary binary "Yes."[^api-event][^terms][^reporting]

The decisive question is whether the rule excluded death from normal "Yes" treatment **and was in force before the death** — the crux given the "rule changed after the fact" allegation. Both are verified from primary sources. The `WLEADEROUT` death carveout appears verbatim in the **original CFTC product certification dated May 15, 2025**, with the contract listed May 16, 2025 — roughly nine months before the death.[^cert] And Wayback's CDX index shows the published `WLEADEROUT.pdf` was **byte-identical** (content digest `G2PYV6QVLU7P4DBNBNWWT6IQSRU55JGJ`) across snapshots from January 11 through March 19, 2026, straddling the February 28 death; the digest only changes at the May 6, 2026 snapshot.[^cdx] The carveout was not added or "clarified into existence" after the death.

That makes the short title — "Ali Khamenei out as Supreme Leader?" — insufficient to call this a failure. A title cannot repeat every carveout; the binding contract handled death, the carveout predated the death, and Kalshi's last-price settlement was a defensible application of that contract.

## Market details

- **Venue:** Kalshi
- **Series:** `KXKHAMENEIOUT` ("Ali Khamenei out?"), governed by the `WLEADEROUT` rulebook.[^api-series]
- **Event shown on page:** `KXKHAMENEIOUT-AKHA`, "Ali Khamenei out as Supreme Leader?", sub-title "Before 2027." Dated strikes at issue included "Before March 1, 2026" and "Before April 1, 2026."[^api-event][^complaint]
- **Governing contract:** the `WLEADEROUT` terms, CFTC-certified **May 15, 2025**, listed **May 16, 2025** — predating the February 28, 2026 death.[^cert]
- **Payout Criterion:** Yes if the leader "has resigned or otherwise left their specified position" (or announces leaving within the year), with a separate death carveout (below).[^terms][^cert]
- **Death:** Khamenei killed February 28, 2026 in U.S./Israeli strikes.[^reporting][^complaint]
- **Settlement:** market paused under Rule 13.1; long/short payouts based on last traded price prior to death, with Outcome Review Committee fair-value backstop.[^api-event][^terms]
- **Reimbursement:** ~$2.2 million in refunded fees and net losses.[^reporting]

## The rule

The `WLEADEROUT` Payout Criterion is leaving office by resignation or otherwise. A separate clause carves out death. The original May 15, 2025 certification (Appendix A, as-listed terms) states:[^cert]

> "If `<leader>` leaves solely because they have died, the associated market will resolve and the Exchange will determine the payouts to the holders of long and short positions based upon the last traded price (prior to the death). If a last traded price is not available or is not logically consistent, or if the Exchange determines at its sole discretion that the last traded prices prior to death do not represent a fair settlement value, the Outcome Review Committee will be responsible for making a binding determination of fair allocation. For the avoidance of doubt, the Exchange will distribute $1.00 for each Contract."

The currently published `WLEADEROUT` terms carry an expanded version of the same carveout — adding that if "trading activity was materially affected by the circumstances giving rise to the death," Kalshi may instead use the last traded price before those circumstances became "known or reasonably anticipated," plus an explicit halt/pause right and a finality clause.[^terms] The core mechanism — death triggers last-price / ORC fair-value settlement rather than an ordinary "Yes" — is present in both the original certification and the current terms.

That rule does not make death a normal "Yes" event. It makes death a special settlement event.

## What happened

Khamenei was killed February 28, 2026. Kalshi did not pay "Yes" at $1. It paused the market under Rule 13.1 and announced it would settle on the last traded price before death; if that price was unclear, the Outcome Review Committee would set fair value.[^api-event] Kalshi's position, reported contemporaneously, is that the policy exists to avoid markets settling directly on death, and that it refunded fees and reimbursed post-death purchases.[^reporting]

Kalshi's own on-platform clarification acknowledges one earlier version was "grammatically ambiguous" and commits to reimburse lost value on trades made between the clarifications.[^api-event] Reporting puts total remediation at about **$2.2 million** in refunded fees and net losses.[^reporting]

Separately, on **March 2, 2026**, Kalshi filed a CFTC rulebook amendment (effective March 17, 2026) adding general **Rule 6.3(e)** for the death of a natural person central to a contract. The filing states the amendment "further codifies and memorializes the exchange's practice" — i.e., it frames the rule as memorializing a pre-existing practice, not creating a new one.[^cftc-amendment]

## The allegation against Kalshi

A class action — **Risch v. KalshiEX LLC** (C.D. Cal., filed March 5, 2026) — alleges Kalshi should have paid "Yes." Notably, its theory is **disclosure and methodology, not absence of the rule**:[^complaint]

- The page's rules summary stated "if Ali Khamenei leaves office before March 1, 2026, then the market resolves Yes," and the death carveout — "to the extent any version of the death carveout appeared" — was allegedly not in the **user-facing rules summary** consumers relied on, and not presented to inform a reasonable consumer of its existence.
- Kalshi itself called a prior disclosure "grammatically ambiguous."
- The "last traded price (prior to the death)" is alleged to be **undefined** in any user-facing material; the precise timestamp, selection criteria, and whether the same methodology applied uniformly across expirations are "opaque."

The complaint quotes the `WLEADEROUT` death carveout verbatim and concedes a version of it appeared in the contract's formal terms. Its grievance is that the carveout was not surfaced in the product UI and that the last-price calculation was not transparent.[^complaint]

## Kalshi's defense

Kalshi's defense is strong on the verified record:

1. The `WLEADEROUT` terms contain a death carveout triggering last-price / ORC fair-value settlement rather than ordinary "Yes."[^terms][^cert]
2. That carveout predated the death: it is in the **May 15, 2025 certification** (listed May 16, 2025), and the published terms PDF was byte-identical across the February 28, 2026 death per Wayback CDX (digest `G2PYV6QVLU7P4DBNBNWWT6IQSRU55JGJ`, January 11–March 19, 2026).[^cert][^cdx]
3. Kalshi paused under Rule 13.1 and settled on the last traded price before death — the mechanism the contract specifies.[^api-event][^terms]
4. Kalshi reimbursed fees, post-death purchases, and ambiguity-window losses (~$2.2M).[^api-event][^reporting]
5. The March 2, 2026 CFTC Rule 6.3(e) amendment "memorializes" the practice, consistent with the carveout already being in `WLEADEROUT`.[^cftc-amendment]

A title shorter than the rule is not a serious rebuttal. Prediction-market titles are summaries; the contract defines edge cases.

## Assessment

### Did Khamenei leaving office by death satisfy the title in ordinary language?

**Yes.** A dead leader is plainly out of office in ordinary language.

### Did Kalshi's written rules make death a normal $1 "Yes" event?

**No.** The `WLEADEROUT` terms carve death out, settling on last traded price with an ORC fair-value backstop.[^terms][^cert]

### Did the death carveout predate the February 28, 2026 death?

**Yes — verified.** It appears in the May 15, 2025 certification (contract listed May 16, 2025), and Wayback CDX shows the terms PDF byte-identical (digest `G2PYV6QVLU7P4DBNBNWWT6IQSRU55JGJ`) from January 11 through March 19, 2026, across the death.[^cert][^cdx] The "rule added after the fact" allegation fails at the contract level.

### Does the title/rule difference itself prove a failure?

**No.** A short title cannot include every condition. With the carveout in the governing contract before the event, it is not a platform failure that the title did not repeat it.

### Did Kalshi violate the contract?

**Not on the verified record.** The contract specified last-price / ORC settlement on death; Kalshi paused and settled that way and reimbursed confused traders. The live disputes are about UI disclosure and the opacity of the specific last-price methodology — transparency and consumer-disclosure questions — not a misapplication of the written settlement rule.

### Overall classification

- **Settlement consistent with the governing written rule:** Yes
- **Carveout predated the death:** Yes — verified from the dated certification and Wayback CDX
- **Misapplication of the rules:** Not established
- **User confusion / UI disclosure:** Real, and the basis of live litigation, but not a contract misresolution
- **Last-price methodology transparency:** A genuine open dispute, not a settled rule violation
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

The prior blocker — needing a timestamped pre-death archive to rebut the "rule changed after the death" allegation — is **resolved**. The May 15, 2025 CFTC certification places the carveout in the as-listed terms nine months before the death, and the Wayback CDX hash-identity (`G2PYV6QVLU7P4DBNBNWWT6IQSRU55JGJ`, January 11–March 19, 2026) shows the published terms PDF was byte-identical across the death.[^cert][^cdx]

Two honest residuals remain, but neither is a contract misresolution: (1) the exact **pre-death market-page rules-summary text** shown in the product UI is not independently archived here, and the complaint alleges the carveout was not surfaced there; and (2) the **last-traded-price methodology** (precise timestamp, selection criteria, uniformity across expirations) is undisclosed and is the strongest live dispute. Both are disclosure/transparency issues now being litigated in *Risch v. Kalshi*, not evidence that Kalshi misresolved the written contract.[^complaint]

## Sources

### Platform / primary

[^api-series]: Kalshi trade API, `series/KXKHAMENEIOUT` ("Ali Khamenei out?"). Lists `WLEADEROUT` as the contract rulebook and links the contract-terms and product-certification PDFs. [API][api-series]

[^api-event]: Kalshi trade API, `events/KXKHAMENEIOUT-AKHA` ("Ali Khamenei out as Supreme Leader?", "Before 2027"). Carries the death clarification ("if Ali Khamenei dies, the market will resolve... based on the last traded price prior to death... the Outcome Review Committee will determine a fair market value"), the grammatically-ambiguous-clarification reimbursement note, and the Rule 13.1 pause notice. [API][api-event]

[^terms]: Kalshi, `WLEADEROUT` contract terms (current). Payout Criterion is the leader resigning or otherwise leaving office; a separate clause settles death at the last traded price prior to death (or before death-related circumstances became known/reasonably anticipated if trading was materially affected), with Outcome Review Committee fair-value backstop and a halt/pause right. [PDF][terms]

[^cert]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification for the "Will `<leader>` leave office before `<date>`?" (`WLEADEROUT`) contract, dated **May 15, 2025**; contract "initially listed May 16, 2025" (signed Xavier Sottile, Head of Markets). Appendix A (as-listed terms) already contains the verbatim death carveout: "If `<leader>` leaves solely because they have died... based upon the last traded price (prior to the death)... the Outcome Review Committee will be responsible for making a binding determination of fair allocation. For the avoidance of doubt, the Exchange will distribute $1.00 for each Contract." [Cert][cert]

[^cdx]: Internet Archive Wayback CDX index for `kalshi-public-docs.s3.amazonaws.com/contract_terms/WLEADEROUT.pdf`. The published terms PDF shows content digest `G2PYV6QVLU7P4DBNBNWWT6IQSRU55JGJ` on snapshots 2026-01-11, 2026-01-19, 2026-01-22, 2026-03-01, and 2026-03-19 — byte-identical across the February 28, 2026 death — with the digest first changing at the 2026-05-06 snapshot. [CDX][cdx]

[^cftc-amendment]: KalshiEX LLC, CFTC rulebook amendment filed **March 2, 2026**, effective March 17, 2026, adding Rule 6.3(e) for the death of a natural person central to a Contract's Underlying or Payout Criterion. The filing states the amendment "further codifies and memorializes the exchange's practice" for such markets. [PDF][cftc-amendment]

[^complaint]: *Risch v. KalshiEX LLC*, class action complaint, U.S. District Court for the Central District of California, filed **March 5, 2026** (plaintiffs Adam Risch and Yonatan Gliksman). Alleges the page's rules summary said the market "resolves Yes if Khamenei leaves office before March 1, 2026," that the death carveout — "to the extent any version... appeared" — was not in the user-facing rules summary, and that the "last traded price (prior to the death)" was undefined and the methodology opaque. Causes of action: breach of contract / implied covenant, fraud and intentional misrepresentation, plus California UCL (§17200) and CLRA claims. Quotes the `WLEADEROUT` death carveout verbatim. [Complaint PDF][complaint]

### Reporting

[^reporting]: Contemporaneous reporting (March 2026; Fox Business, Bloomberg Law, CNN, Decrypt and others) on the Khamenei market: Khamenei killed February 28, 2026; Kalshi invoked the death carveout and settled on last traded price rather than paying "Yes"; Kalshi said its policy avoids markets settling directly on death; and Kalshi refunded fees and net losses, reported at roughly $2.2 million, on the "Ali Khamenei out as Supreme Leader?" market. [Fox Business][reporting-fox]

[api-series]: https://api.elections.kalshi.com/trade-api/v2/series/KXKHAMENEIOUT
[api-event]: https://api.elections.kalshi.com/trade-api/v2/events/KXKHAMENEIOUT-AKHA?with_nested_markets=true
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/WLEADEROUT.pdf
[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/WLEADEROUT.pdf
[cdx]: http://web.archive.org/cdx/search/cdx?url=kalshi-public-docs.s3.amazonaws.com/contract_terms/WLEADEROUT.pdf&output=json
[cftc-amendment]: https://www.cftc.gov/sites/default/files/filings/orgrules/26/03/rules03022640155.pdf
[complaint]: https://storage.courtlistener.com/recap/gov.uscourts.cacd.1009602/gov.uscourts.cacd.1009602.1.0.pdf
[reporting-fox]: https://www.foxbusiness.com/technology/prediction-market-kalshi-sued-54m-iran-leader-bets-death-carveout-invoked
