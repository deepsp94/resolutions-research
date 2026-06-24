# Kalshi: 2025 government shutdown duration

## Bottom line

**Finding: No failure. Kalshi resolved its 2025 government-shutdown-duration market to 43 days, matching the universal historical record, under a governing contract whose times are entirely Eastern Time — so the original "UTC-vs-ET cutoff error" allegation is built on a convention that does not exist in the rules. Confidence: High.**

The market in question is Kalshi's `KXGOVSHUTLENGTH` series, governed by the **SHUTLENGTH** contract (CFTC self-certified Jan 19, 2023), which uses the U.S. Office of Personnel Management (OPM) as its sole Source Agency, checks shutdown status daily at 10:00 AM ET, and specifies every time in Eastern Time with no UTC convention anywhere.[^terms][^series][^cert] The 2025 shutdown ran Oct 1 – Nov 12, 2025 and was reported essentially everywhere as 43 days, the longest in U.S. history; Kalshi's "above 43 days" rung resolved No and shorter rungs resolved Yes, matching that consensus.[^wiki][^settle]

The strongest contrary argument — that OPM's status web page may not have flipped to "Open" until ~11:25 AM ET on Nov 13, after the 10:00 AM ET checkpoint, arguably implying a 44th day — is speculative and immaterial: the funding bill was signed the night of Nov 12 and OPM published "normal operating procedures are in effect" for Nov 13, satisfying the contract's "operating normally" expiration trigger. Counting a 44th day would contradict every primary record.[^opm][^wiki]

## Market details

- **Venue:** Kalshi
- **Series / event:** `KXGOVSHUTLENGTH`, event `KXGOVSHUTLENGTH-26JAN01`, "How long will the government shutdown last?"[^series]
- **Governing contract:** SHUTLENGTH, CFTC self-certified Jan 19, 2023; all times Eastern Time, no UTC convention.[^terms][^cert]
- **Source Agency:** U.S. Office of Personnel Management (OPM); current status checked daily at 10:00 AM ET.[^terms][^series]
- **Real-world facts:** Shutdown Oct 1 – Nov 12, 2025; funding bill (P.L. 119-37) signed ~10:24 PM ET Nov 12, 2025; reported as 43 days, the longest in U.S. history; OPM posted "normal operating procedures are in effect" for Nov 13.[^wiki][^opm]
- **Settled outcome:** Final length 43 days. "Above 43 days" resolved No; "above 42" and shorter resolved Yes — matching consensus.[^settle][^wiki]

## What happened

The 2025 federal government shutdown began Oct 1, 2025 and ended when President Trump signed the funding bill (P.L. 119-37) at roughly 10:24 PM ET on Nov 12, 2025. It lasted 43 days and was the longest shutdown in U.S. history.[^wiki] OPM published that "normal operating procedures are in effect" for federal agencies on Thursday, Nov 13, 2025.[^opm]

Kalshi's `KXGOVSHUTLENGTH` market asked how long the shutdown would last, with rungs for various day counts. It settled at a final length of 43 days: the "more than 43 days" / "above 43" rung resolved No, while "above 42 days" and shorter rungs resolved Yes.[^settle] That outcome matches the consensus that the shutdown lasted exactly 43 days.[^wiki]

## The allegation against Kalshi

The original allegation, framed on Reddit, asserted that Kalshi applied a UTC-vs-ET cutoff error to the shutdown-duration market — i.e., that the day-counting checkpoint was evaluated in UTC instead of Eastern Time, producing a length one day off from a correct ET count.

A refined, stronger version of the dispute drops the UTC framing and instead argues that OPM's current-status web page reportedly did not flip to "Open" until ~11:25 AM ET on Nov 13 — after the contract's 10:00 AM ET checkpoint — which on a literal reading of the daily-status check could imply Nov 13 was still a "shutdown day," making the total 44 days rather than 43.

## Kalshi's defense

The governing SHUTLENGTH contract specifies every time in Eastern Time and contains no UTC convention at all, so there is no UTC cutoff to have applied incorrectly.[^terms] The Source Agency is OPM, and the Payout Criterion counts a day when the government is "at least partially shut down... due to a lapse in appropriations," checked at 10:00 AM ET.[^terms] The Expiration Date is the sooner of the first 10:00 AM ET following a Payout-Criterion event, the first 10:00 AM ET following a shutdown where "the government is operating normally," or one day after the listed date — and OPM's published "normal operating procedures are in effect" for Nov 13 satisfies the "operating normally" trigger.[^terms][^opm]

A separate, later contract — **GOVTSHUTLENGTH**, CFTC-certified Feb 5, 2026 — adds OMB+OPM and multi-outlet sources plus more detailed day-counting language. But it postdates this event by roughly three months and did not govern this market.[^govtcert] Any analysis built on `GOVTSHUTLENGTH.pdf` is reading the wrong (later) contract.

## Assessment

### Did the governing contract use a UTC cutoff?

**No.** SHUTLENGTH specifies all times in Eastern Time; there is no UTC convention anywhere in the contract, so the original UTC-vs-ET allegation has no basis in the rules.[^terms][^series]

### Was the correct contract identified?

**Yes — and it is easy to get wrong.** The market is governed by SHUTLENGTH (self-certified Jan 19, 2023), not by the later GOVTSHUTLENGTH (certified Feb 5, 2026), which postdates the event by ~3 months and never governed this market.[^cert][^govtcert]

### Did the 43-day settlement match reality?

**Yes.** The shutdown ran Oct 1 – Nov 12, 2025 and was universally reported as 43 days, the longest in U.S. history; Kalshi's rungs resolved accordingly.[^wiki][^settle]

### Does the OPM-page-timing argument change the outcome?

**No.** Even if OPM's status page didn't flip to "Open" until ~11:25 AM ET Nov 13, the funding bill was signed the night of Nov 12 and OPM published "normal operating procedures are in effect" for Nov 13, satisfying the contract's "operating normally" expiration trigger. Counting a 44th day would contradict every primary record.[^opm][^wiki][^terms]

### Overall classification

- **UTC/ET cutoff allegation:** Unfounded — contract is entirely ET.
- **Wrong-contract risk (GOVTSHUTLENGTH):** Real, but the analysis here uses the correct governing contract (SHUTLENGTH).
- **Settlement vs. consensus:** Matches (43 days).
- **Strongest pro-dispute argument (OPM page timing):** Speculative and immaterial.
- **Best public verdict:** No failure.

## Precise blocker to a stronger finding

None is material. The governing contract (SHUTLENGTH and its OPM source agency), the 43-day consensus, and the OPM "operating normally" Nov 13 status are all sourced.[^terms][^series][^wiki][^opm] The only missing artifacts are an archived screenshot of the settled rung ladder and the exact timestamp on the OPM current-status page; neither would change the outcome, since the shutdown was legally and operationally over by the Nov 13 checkpoint and the 43-day count is the universal record.

## Sources

[^terms]: Kalshi SHUTLENGTH governing contract terms — Source Agency = "the Office of Personnel Management"; daily 10:00 AM ET status check; Expiration Date triggers including "the government is operating normally"; all times Eastern Time. [SHUTLENGTH.pdf][terms]

[^series]: Kalshi series API for `KXGOVSHUTLENGTH`, pointing to SHUTLENGTH contract terms with OPM as the settlement source agency. [series API][series]

[^cert]: Kalshi SHUTLENGTH product certification, CFTC self-certified Jan 19, 2023. [SHUTLENGTH cert][cert]

[^govtcert]: Kalshi GOVTSHUTLENGTH product certification, CFTC-certified Feb 5, 2026 — postdates this event by ~3 months and did not govern. [GOVTSHUTLENGTH cert][govtcert]

[^wiki]: 2025 United States federal government shutdown — Oct 1 to Nov 12, 2025; funding bill signed ~10:24 PM ET Nov 12; 43 days, longest in U.S. history. [Wikipedia][wiki]

[^settle]: Settlement recap — final length 43 days; "above 43 days" rung resolved No; 10:00 AM ET Nov 13 checkpoint. [SportsHandle][settle]

[^opm]: OPM statement that federal agencies' "normal operating procedures are in effect" Thursday, Nov 13, 2025, as the shutdown ended. [NBC Washington][opm]

[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/SHUTLENGTH.pdf
[series]: https://api.elections.kalshi.com/trade-api/v2/series/KXGOVSHUTLENGTH
[cert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/SHUTLENGTH.pdf
[govtcert]: https://kalshi-public-docs.s3.us-east-1.amazonaws.com/regulatory/product-certifications/GOVTSHUTLENGTH.pdf
[wiki]: https://en.wikipedia.org/wiki/2025_United_States_federal_government_shutdown
[settle]: https://sportshandle.com/kalshi/government-shutdown-prediction-markets/
[opm]: https://www.nbcwashington.com/news/local/government-shutdown/opm-says-federal-agencies-are-open-thursday-as-shutdown-ends/
