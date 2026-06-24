# Kalshi: Miami high temperature and a corrected-away NWS reading

## Bottom line

**Finding: No failure. Kalshi settled the November 27, 2024 Miami high-temperature market on the value the NWS had documented at the contract's morning expiration (84°F). That figure was later corrected to 81°F, but the contract in force at the time froze the value at expiration and excluded post-expiration revisions, with no delay-for-corrections mechanism. Kalshi applied the governing written rule. Confidence: medium-high.**

This case looks at first like a clean misresolution: the official Miami high for November 27, 2024 is **81°F**, yet Kalshi's settled market resolved **"84° or above" Yes**.[^climia-final][^ncei][^kalshi-market] The 84°F was a transient NWS error, issued at 4:32 AM ET and corrected back to 81°F at 8:56 AM ET.[^climia-84][^climia-final]

The decisive question is *which contract governed*. The current `MIAHIGH` terms contain a clause delaying determination to 11AM ET when a high is inconsistent with METAR or "the Final report high is lower than earlier report(s)" — which would have caught this correction.[^terms-current] But **that clause was not in the contract in November 2024.** The May 2023 CFTC certification of the Miami contract, and the October 18, 2024 CFTC certification of the structurally identical Los Angeles high-temperature contract (filed about six weeks before this incident), both set expiration at "the first 7:00 or 8:00 AM ET following the release of the data" with **no delay clause at all**.[^cert-mia-2023][^cert-la-2024] Kalshi added the delay mechanism only later.

Under the rule that actually governed, the NWS-documented value at the ~7–8 AM expiration was 84°F, and the 8:56 AM correction to 81°F was a post-expiration revision the contract excluded. Settling at 84°F was therefore a correct application of the written rule, not a resolution failure. The episode exposed a weak contract design — a settlement with no safeguard against transient sensor errors — which Kalshi appears to have fixed afterward, but applying a written rule as drafted is not a failure.

## Market details

- **Venue:** Kalshi
- **Market:** "Highest temperature in Miami on Nov 27, 2024?" — event `KXHIGHMIA-24NOV27`, governed by the Miami high-temperature contract.[^kalshi-market]
- **Outcome buckets:** ≤75°, 76–77°, 78–79°, 80–81°, 82–83°, 84° or above.[^kalshi-market]
- **Binding source:** the NWS Daily Climate Report (CLI) for Miami, FL.[^cert-mia-2023]
- **Governing rule (Nov 2024):** expiration at the first 7:00/8:00 AM ET after data release; "Revisions to the Underlying made after Expiration will not be accounted for"; **no** 11AM-ET delay clause.[^cert-mia-2023][^cert-la-2024]
- **NWS-documented value at expiration:** 84°F (4:32 AM ET report).[^climia-84]
- **Final corrected value:** 81°F (8:56 AM ET correction; NCEI daily summary).[^climia-final][^ncei]
- **Kalshi settlement:** "84° or above" = Yes.[^kalshi-market]

## What happened

The contract's Underlying is the maximum temperature in the NWS Daily Climate Report for Miami. The relevant NWS product (CLIMIA) issued the following for the November 27, 2024 summary (timestamps from the NWS product archive):

| Issued (ET) | Reported maximum |
|---|---|
| Nov 27, 4:25 PM | 81°F (at 3:15 PM)[^climia-pm] |
| Nov 28, 4:32 AM | **84°F (logged as a 4:18 AM "high")**[^climia-84] |
| Nov 28, 8:56 AM | 81°F (at 3:15 PM) — corrected[^climia-final] |

The 84°F reading is physically implausible — a 4:18 AM maximum of 84°F in late-November Miami — and the corrected report restored the real 3:15 PM afternoon peak of 81°F, which the independent NCEI daily summary also records.[^climia-84][^climia-final][^ncei] Kalshi's settled market resolved "84° or above" Yes and the correct "80–81°" bucket No.[^kalshi-market]

## The allegation against Kalshi

Traders alleged Kalshi settled on the initial 84°F even though NWS corrected it to 81°F, paying an impossible outcome and grading the true "80–81°" holders as losers.[^reddit] The factual premise is correct — Kalshi did settle "84° or above" Yes.[^kalshi-market] The question is whether that violated the governing contract.

## Kalshi's defense

The defense is that the contract froze the value at expiration and excluded later corrections.

The Miami contract (May 2023 certification) and the identical-template Los Angeles contract (October 2024 certification) both provide: Expiration Date is "the sooner of the first 7:00 or 8:00 AM ET following the release of the data," Expiration Value is "the value of the Underlying as documented by the Source Agency on the Expiration Date at the Expiration time," and "Revisions to the Underlying made after Expiration will not be accounted for in determining the Expiration Value."[^cert-mia-2023][^cert-la-2024] Neither version contains the 11AM-ET delay clause present in the current terms.[^terms-current]

The data for November 27 was released in the 4:32 AM ET report showing 84°F; the first 7:00/8:00 AM ET expiration therefore documented 84°F; and the 8:56 AM ET correction to 81°F arrived after expiration and was excluded. On the governing contract, 84°F was the Expiration Value.

## Assessment

### Did the delay clause govern in November 2024?

**No.** It is absent from the May 2023 Miami certification and from the October 18, 2024 Los Angeles certification of the same weather-contract template, the latter filed roughly six weeks before this market settled.[^cert-mia-2023][^cert-la-2024] No archived copy of the contract from 2024 contains it; the clause appears only in later versions.[^terms-current] The earlier draft of this case file wrongly relied on the current clause; the dated certifications correct that.

### Under the governing rule, was 84°F the right Expiration Value?

**Yes.** Expiration fell at the first 7:00/8:00 AM ET after the data release, when NWS had documented 84°F; the 81°F correction came at 8:56 AM ET, after expiration, and the contract excluded post-expiration revisions.[^cert-mia-2023][^climia-84][^climia-final]

### So was this a resolution failure?

**No — it was a rule applied as written.** This mirrors the Oscars viewership case, where Kalshi settled on the value documented at expiration and excluded later upward revisions; following a written post-expiration-exclusion rule is not a settlement error even when a later correction would change the number.

### Is there a fair criticism of Kalshi?

**Yes, but it is a design criticism, not a failure.** A weather contract whose settlement can lock in a transient, physically impossible sensor reading — with no consistency check or short delay — is poorly designed. Kalshi's later addition of the 11AM-ET delay clause (which keys on METAR inconsistency and downward revisions) is effectively an acknowledgment of that gap. That improvement does not retroactively make the November 2024 settlement a rule violation.

### Overall classification

- **Settlement consistent with the governing written rule:** Yes
- **Misapplication of the rules:** No
- **Semantic ambiguity:** No
- **Weak contract design (since amended):** Yes
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

None material. The decisive facts are verified from primary sources: the dated CFTC certifications showing the governing rule had no delay clause, the timestamped NWS CLIMIA issuances showing the 84°F documented at the morning expiration and the later 81°F correction, the NCEI final value, and Kalshi's settled market page. The only minor residual is that no archived copy of the exact Miami contract page from November 27, 2024 survives independently of the CFTC certifications; the two dated certifications bracketing the incident make that immaterial.

## Sources

[^cert-mia-2023]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification, "Will the high temperature in Miami be <greater than/less than/between> <degrees>?", dated May 8, 2023. Sets expiration at the first 7:00/8:00 AM ET after data release and excludes post-expiration revisions; contains no 11AM-ET delay clause. (Also Kalshi's current `MIAHIGH` product-certification PDF.) [Cert][cert-mia-2023]

[^cert-la-2024]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification, "Will the high temperature in Los Angeles be <greater than/less than/between> <degrees>?", dated October 18, 2024 — the same weather-contract template, certified ~6 weeks before the Miami incident, with the identical expiration mechanics and **no** delay clause. [Cert][cert-la-2024]

[^terms-current]: Kalshi, current `MIAHIGH` contract terms. Adds the later language: "Determination will be delayed until 11AM ET in the case of either (1) High temperature is not consistent with 6-hr or 24-hr highs reported by METAR or (2) the Final report high is lower than earlier report(s)." [PDF][terms-current]

[^kalshi-market]: Kalshi, settled market page, "Highest temperature in Miami on Nov 27, 2024?" (`KXHIGHMIA-24NOV27`), marked Determined. Shows "84° or above" resolved Yes and "80° to 81°" resolved No. [Market][kalshi-market]

[^climia-pm]: NWS Miami Climate Summary for November 27, 2024, issued Nov 27 4:25 PM ET (`202411272125-KMFL-CDUS42-CLIMIA`). Maximum 81°F at 3:15 PM. [Product][climia-pm]

[^climia-84]: NWS Miami Climate Summary for November 27, 2024, issued Nov 28 4:32 AM ET (`202411280932-KMFL-CDUS42-CLIMIA`). Maximum erroneously shown as 84°F, logged at "4:18 AM." [Product][climia-84]

[^climia-final]: NWS Miami Climate Summary for November 27, 2024, corrected issuance Nov 28 8:56 AM ET (`202411281356-KMFL-CDUS42-CLIMIA`). Maximum restored to 81°F at 3:15 PM. [Product][climia-final]

[^ncei]: NOAA NCEI daily-summaries, station USW00012839 (Miami International), 2024-11-27. TMAX = 81°F. [Query][ncei]

[^reddit]: Reddit, r/Kalshi, "Were you impacted by Kalshi's incorrect resolution…" (late November 2024). Traders report the market settled on 84°F despite the NWS correction. Thread no longer reliably crawlable. [Thread][reddit]

[cert-mia-2023]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/MIAHIGH.pdf
[cert-la-2024]: https://www.cftc.gov/sites/default/files/filings/ptc/24/10/ptc1018247244.pdf
[terms-current]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/MIAHIGH.pdf
[kalshi-market]: https://kalshi.com/markets/kxhighmia/highest-temperature-in-miami/kxhighmia-24nov27
[climia-pm]: https://mesonet.agron.iastate.edu/api/1/nwstext/202411272125-KMFL-CDUS42-CLIMIA
[climia-84]: https://mesonet.agron.iastate.edu/api/1/nwstext/202411280932-KMFL-CDUS42-CLIMIA
[climia-final]: https://mesonet.agron.iastate.edu/api/1/nwstext/202411281356-KMFL-CDUS42-CLIMIA
[ncei]: https://www.ncei.noaa.gov/access/services/data/v1?dataset=daily-summaries&dataTypes=TMAX,TMIN&stations=USW00012839&startDate=2024-11-27&endDate=2024-11-27&units=standard&format=json
[reddit]: https://www.reddit.com/r/Kalshi/comments/1h1zjhb/were_you_impacted_by_kalshis_incorrect_resolution/
