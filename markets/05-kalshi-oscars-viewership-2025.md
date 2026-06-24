# Kalshi: 2025 Oscars viewership and a next-day upward revision

## Bottom line

**Finding: No failure. Kalshi settled its 2025 Oscars viewership market on the viewer count documented by the source agencies at the contract's expiration — an initial ~18.07 million figure that put the audience below the 19.5-million strike, so that strike resolved No. Nielsen/ABC revised the count up to ~19.69 million the next day, which would have made the strike Yes, but the governing contract expressly excluded revisions made after expiration. Kalshi applied the written rule. Confidence: high. Failure-resolved: N/A.**

This looks at first like a clean misresolution: the figure now reported for the 2025 Oscars is **~19.7 million**, above Kalshi's **19.5-million** strike, yet that strike settled **No**.[^thewrap][^variety] The settlement instead used the **initial ~18.07 million** count.[^guardian][^thewrap]

The decisive question is *which value the contract bound to*. The governing rules — certified to the CFTC on **February 28, 2025** (listed March 1, 2025), days before the March 2 ceremony — define the Underlying as the reported viewer count and state verbatim that "**Revisions to the Underlying made after Expiration will not be accounted for in determining the Expiration Value**," with the Expiration Value taken "as documented by the Source Agency on the Expiration Date at the Expiration time" of **10:00 AM ET**.[^cert] The initial report (~18.07M, March 3) was below 19.5M; the ~19.69M figure was a March 4 upward revision adding digital viewing.[^thewrap][^variety] Under the rule that governed, the post-expiration revision was excluded, and No was the correct application of the written terms.

The episode is a genuine user-facing controversy and a weak product design — a "viewership" market that locks in an early count and excludes a same-week fuller measure can pay an answer that looks false to ordinary users — but applying a written post-expiration-exclusion rule as drafted is not a settlement error.

## Market details

- **Venue:** Kalshi
- **Market:** "How many people will watch the Oscars?" (In 2025) — series `KXOSCARSVIEWER`, event `KXOSCARSVIEWER-25`.[^series]
- **Relevant strike:** above 19.5 million viewers.[^predictionnews-resolutions]
- **Event:** 97th Academy Awards, March 2, 2025.
- **Governing contract:** the Oscars-viewership terms, CFTC-certified February 28, 2025 (listed March 1, 2025).[^cert]
- **Binding sources (priority order):** The New York Times, Deadline, Variety, CBS News, The Guardian, the Associated Press, The Washington Post, the Hollywood Reporter, Nielsen.[^cert]
- **Governing rule:** Expiration Value "as documented by the Source Agency on the Expiration Date at the Expiration time"; Expiration time 10:00 AM ET; "Revisions to the Underlying made after Expiration will not be accounted for."[^cert]
- **Value used at settlement:** initial ~18.07 million (below 19.5M).[^guardian][^thewrap]
- **Later revised value:** ~19.69 million (≈19.7M).[^thewrap][^variety]
- **Result for the 19.5-million strike:** No.[^predictionnews-resolutions]

I could not recover the live 2025 strike grid or per-strike settled results from Kalshi's public API: the `KXOSCARSVIEWER-25` event still resolves but its markets have been pruned from the markets endpoint, and the only Wayback snapshot of the live market page is a client-rendered shell with no embedded data.[^series] The strike (above 19.5M) and the No outcome are documented by PredictionNews.[^predictionnews-resolutions]

## What happened

The contract's Underlying is the reported number of viewers the Academy Awards telecast drew, with the Expiration Value taken at 10:00 AM ET on the Expiration Date and post-expiration revisions excluded.[^cert] The reported figure moved as follows:

| Reported | Viewer count | Basis |
|---|---|---|
| March 3, 2025 | **~18.07 million** (ABC + Hulu) | Initial Nielsen Fast Nationals; The Guardian: "just over 18m," down 7%[^guardian][^thewrap] |
| March 4, 2025 | **~19.69 million** (≈19.7M) | Updated Nielsen figures adding digital viewing on mobile, PCs, tablets — a gain of ~1.645 million[^thewrap][^variety] |

The ~1.645-million upward revision came from counting digital-device viewing not in the first release — a category that mattered in 2025 because the ceremony was livestreamed on Hulu — and made the 2025 audience the biggest in five years.[^thewrap][^variety] The 19.5-million strike, settled on the initial ~18.07M figure, resolved No.[^predictionnews-resolutions]

## The allegation against Kalshi

Traders alleged the settlement no longer matched the commonly reported event fact: the ordinary answer to "how many watched the 2025 Oscars?" became ~19.7 million, above the 19.5-million strike, yet the strike stayed No.[^predictionnews-resolutions] The factual premise is correct — the strike did settle No on the ~18M figure while the later best-known count exceeded 19.5M. The question is whether that violated the governing contract.

## Kalshi's defense

The defense is that the contract froze the value at expiration and excluded later revisions.

The governing terms, certified to the CFTC on February 28, 2025, provide: the Expiration Value is "the value of the Underlying as documented by the Source Agency on the Expiration Date at the Expiration time," the Expiration time is 10:00 AM ET, and "Revisions to the Underlying made after Expiration will not be accounted for in determining the Expiration Value."[^cert] PredictionNews reports that Kalshi did not change the resolution because the rules stated the initial release would count and future revisions would not, and quotes a Kalshi operations-team member saying the market was "determined correctly" while acknowledging it was unfortunate the market did not account for data revisions.[^predictionnews-resolutions]

The value documented at the 10:00 AM ET expiration was the initial ~18.07-million count, below 19.5 million; the ~19.69-million figure was a March 4 upward revision arriving after expiration and was excluded. On the governing contract, the sub-19.5M value was the Expiration Value.

## Assessment

### Which contract version governed in March 2025?

**The February 28, 2025 certification.** It was self-certified to the CFTC days before the March 2 ceremony (signed by Kalshi's Head of Markets and listed March 1, 2025), and its Appendix A terms match the current public terms PDF in substance — same Underlying definition, same post-expiration-revision exclusion, same 10:00 AM ET Expiration time, and the same nine-agency priority list.[^cert][^series] This is not a today's-version proxy: the dated certification is the version in force at the event.

### Under the governing rule, was the sub-19.5M figure the right Expiration Value?

**Yes.** The Expiration Value was the count documented by the source agencies at the 10:00 AM ET expiration, which was the initial ~18.07-million figure; the ~19.69-million figure was a next-day upward revision the contract excluded.[^cert][^guardian][^thewrap] The 19.5-million strike therefore resolved No.

### So was this a resolution failure?

**No — it was a rule applied as written.** This mirrors the Miami high-temperature case, where Kalshi settled on the value documented at expiration and excluded a later correction; following a written post-expiration-exclusion rule is not a settlement error even when a later revision would change the number.

### Is there a fair criticism of Kalshi?

**Yes, but it is a design and communication criticism, not a failure.** A "viewership" market that locks in an early reported count and mechanically excludes a same-week, fuller release — newly material in 2025 because Hulu streaming and digital-device viewing shifted ~1.645 million viewers into the revised total — pays an answer that looks false to users who treated the market as final Oscars viewership.[^thewrap][^variety] Kalshi could have avoided the controversy by framing the contract as the initial reported figure or by keying settlement to a fuller release. That weakness does not make the settlement a violation of the written rule.

### Overall classification

- **Settlement consistent with the governing written rule:** Yes
- **Misapplication of the rules:** No
- **Final-real-world mismatch:** Yes (later best-known count exceeded the strike)
- **Weak contract design / user-expectation problem:** Yes
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

None material to the verdict. The decisive facts are verified from primary sources: the dated February 28, 2025 CFTC certification showing the governing post-expiration-exclusion rule and the 10:00 AM ET expiration, the correct series ticker (`KXOSCARSVIEWER`), the initial ~18.07-million count, and the ~19.69-million March 4 revision. The only residual is that the live 2025 strike grid and per-strike settled results could not be pulled from Kalshi's API (the event's markets are pruned) or from the archived live page (a client-rendered shell); the strike and No outcome rest on PredictionNews. An archived rendered market page would complete the market-details section but does not change the classification.

## Sources

[^cert]: KalshiEX LLC, CFTC Regulation 40.2(a) product certification, "Will <above/below/between/exactly/at least> <count> persons watch the <year> Academy Awards?", signed by the Head of Markets and dated February 28, 2025 (listed March 1, 2025). Appendix A defines the Underlying as the reported viewer count; states "Revisions to the Underlying made after Expiration will not be accounted for in determining the Expiration Value"; sets the Expiration Value "as documented by the Source Agency on the Expiration Date at the Expiration time"; sets the Expiration time at 10:00 AM ET; and lists the Source Agencies in priority order (The New York Times, Deadline, Variety, CBS News, The Guardian, the Associated Press, The Washington Post, the Hollywood Reporter, Nielsen). [Cert][cert] (Substantively identical current terms PDF: [Terms][terms].)

[^series]: Kalshi trade API, series `KXOSCARSVIEWER` and event `KXOSCARSVIEWER-25`, "How many people will watch the Oscars?" / "In 2025." The event resolves but its markets are pruned from the public markets endpoint; the contract-terms and certification URLs are provided in the series metadata. [API][series]

[^guardian]: The Guardian, "Oscars telecast ratings fall 7% to 18m viewers," March 4, 2025. Reports the initial Nielsen figure as "just over 18m" across ABC and Hulu, down 7%. [Article][guardian]

[^thewrap]: TheWrap, "2025 Oscar Ratings Tick Up to 19.7 Million Viewers, Biggest in 5 Years." Reports the initial 18.07-million count (March 3) and the revised 19.69-million total (March 4), a gain of 1.645 million from adding digital viewing on mobile, PCs, and tablets. [Article][thewrap]

[^variety]: Variety, "Oscars Ratings 2025: 19.7 Million Viewers." Reports the revised ~19.69-million total as the biggest Oscars audience in five years. [Article][variety]

[^predictionnews-resolutions]: PredictionNews, "Prediction Market Resolutions: The Good, Bad, and Ugly." Describes the Kalshi Oscars controversy: the above-19.5-million strike resolving No on the initial figure, the later ~19.7-million revision, the rule excluding post-expiration revisions, and Kalshi's stated rationale that it determined the market correctly. [Article][predictionnews-resolutions]

[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/OSCARSVIEWER.pdf
[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/OSCARSVIEWER.pdf
[series]: https://api.elections.kalshi.com/trade-api/v2/series/KXOSCARSVIEWER
[guardian]: https://www.theguardian.com/film/2025/mar/04/oscars-telecast-ratings-fall-7-to-18m-viewers
[thewrap]: https://www.thewrap.com/2025-oscars-ratings-viewership-abc-hulu/
[variety]: https://variety.com/2025/tv/news/oscars-ratings-2025-viewers-1236326364/
[predictionnews-resolutions]: https://predictionnews.com/learn/resolutions/
