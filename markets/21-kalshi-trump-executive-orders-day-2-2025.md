# Kalshi: Trump executive orders on Day 2

## Bottom line

**Finding: No failure. Kalshi's resolution was correct under the binding contract, which counts executive orders by signing date as recorded in the Federal Register. Confidence: high.**

The seed allegation came from a single Reddit thread about a Kalshi market on how many executive orders Donald Trump signed on his second day in office (January 21, 2025). The poster alleged that WhiteHouse.gov showed zero executive orders for that day, while Kalshi resolved the count in the `1-5` bucket.[^reddit]

That allegation relied on the wrong source. The binding contract (Kalshi's `EOPERIOD` terms) names the **Federal Register** as the sole Source Agency and counts an executive order by its **signing date**.[^terms] The Federal Register records exactly **two** numbered executive orders signed January 21, 2025: EO 14173 ("Ending Illegal Discrimination and Restoring Merit-Based Opportunity") and EO 14174 ("Revocation of Certain Executive Orders"), both published January 31, 2025.[^fr-api][^fr-index] Two falls inside the `1-5` bucket, so Kalshi resolved correctly.

This should be marked **No failure**.

## Market details

- **Venue:** Kalshi
- **Market:** "Executive Orders - Day 2," part of Kalshi's daily executive-order count series (`KXEOCOUNT…`), governed by the `EOPERIOD` contract terms.[^terms]
- **Period:** Trump's second day in office, January 21, 2025 (Inauguration Day, January 20, was Day 1).
- **Binding source:** the Federal Register (`federalregister.gov`), per the contract.[^terms]
- **Source alleged by the trader:** WhiteHouse.gov.[^reddit]
- **Actual result:** two executive orders signed January 21, 2025 (EO 14173, EO 14174); the `1-5` resolution was correct.[^fr-api]

## What happened

A Reddit poster alleged that the official source showed zero executive orders for January 21, 2025, but that Kalshi counted `1-5`, and asked how to dispute the outcome.[^reddit] Other commenters in the same thread pushed back, noting that a qualifying White House action existed and that the rules counted the revocation of an executive order as itself an executive order; a Kalshi-tagged comment said the outcome had already been explained through Kalshi Ideas and support.[^reddit]

The binding contract resolves the disagreement. Under `EOPERIOD`, an "Executive Order" is a numbered presidential directive formally titled "Executive Order," signed by the President, and published in the Federal Register; the count is determined by **signing date as recorded in the Federal Register**, and orders "that are later revoked or amended still count for the period they were signed."[^terms] Presidential memoranda, proclamations, and determinations explicitly do **not** count.[^terms]

The Federal Register lists two executive orders with a signing date of January 21, 2025 — EO 14173 and EO 14174 — each published January 31, 2025.[^fr-api][^fr-index] EO 14174 is itself a revocation of prior executive orders, which is exactly the case the contract says still counts as a numbered executive order.[^terms]

## The allegation against Kalshi

The allegation is that Kalshi counted executive orders that did not appear on the named White House source for that day, i.e., that it used a broader or different source than the one users were trading against.[^reddit]

If the binding source had been WhiteHouse.gov and that page had shown zero, this would be a source-rule failure. Neither premise holds.

## Kalshi's defense

The defense is the contract text, and it is decisive rather than merely plausible.

The `EOPERIOD` terms name the Federal Register — not WhiteHouse.gov — as the Source Agency, count by signing date, and expressly include later-revoked or amended orders for the period they were signed.[^terms] The Federal Register shows two qualifying orders signed January 21, 2025.[^fr-api] The trader's "zero" figure came from the wrong source and likely also reflected the publication lag: both orders were signed January 21 but not published until January 31, so anyone checking by publication date — or a live WhiteHouse.gov list — could see nothing for January 21 even though two orders had been signed.[^fr-api]

## Assessment

### Is the market identified, with its binding rules?

**Yes.** It is Kalshi's daily executive-order count series under the `EOPERIOD` terms, which name the Federal Register as the source and count by signing date.[^terms]

### Does the binding source support the resolution?

**Yes.** The Federal Register records two executive orders signed January 21, 2025 (EO 14173, EO 14174), and `1-5` is the correct bucket.[^fr-api][^fr-index]

### Was the trader's premise correct?

**No.** The "zero" count relied on WhiteHouse.gov rather than the contract's Federal Register source, and did not account for the signing-date rule or the ten-day publication lag.[^terms][^fr-api]

### Was there any broader controversy?

**No.** The dispute appears only in one self-rebutting r/Kalshi thread. No prediction-market media covered it, and no Kalshi statement, refund, correction, CFTC complaint, or lawsuit is tied to it — unlike Kalshi's genuinely contested markets (e.g., the Khamenei death market and NFL futures).[^reddit]

### Overall classification

- **Source/count dispute:** Raised, but unfounded
- **Binding source:** Federal Register, which supports the resolution
- **Platform rule violation:** None
- **Best public verdict:** No failure

## Precise blocker to a stronger finding

None material. The original Reddit thread is no longer reliably crawlable, so its full comment record cannot be re-derived, but the verdict does not depend on it: the binding contract terms and the Federal Register record are both primary, public, and independently verifiable, and both support Kalshi's resolution.

## Sources

[^terms]: Kalshi, `EOPERIOD` contract terms (binding rules). Names the Federal Register as the sole Source Agency, defines a countable "Executive Order" as a numbered directive published in the Federal Register, counts by signing date ("The signing date as recorded in the Federal Register determines which period an Executive Order belongs to"), includes later-revoked/amended orders for the period signed, and excludes memoranda, proclamations, and determinations. [PDF][terms]

[^fr-api]: Federal Register API, query for presidential documents of type "executive_order" with signing date January 21, 2025. Returns a count of 2: EO 14173 ("Ending Illegal Discrimination and Restoring Merit-Based Opportunity") and EO 14174 ("Revocation of Certain Executive Orders"), both signed 2025-01-21 and published 2025-01-31. [Query][fr-api]

[^fr-index]: Federal Register, Trump 2025 executive-orders index. Lists the numbered executive orders and their signing/publication dates. [Index][fr-index]

[^reddit]: Reddit, r/Kalshi, "How does one dispute a Kalshi outcome? Anyone else affected by the incorrect count of Executive Orders - Day 2?" January 2025. Contains the allegation, in-thread counterarguments, and references to Kalshi support/Kalshi Ideas explanations. [Thread][reddit]

[terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/EOPERIOD.pdf
[fr-api]: https://www.federalregister.gov/api/v1/documents.json?conditions%5Bpresidential_document_type%5D%5B%5D=executive_order&conditions%5Bsigning_date%5D%5Bgte%5D=2025-01-21&conditions%5Bsigning_date%5D%5Blte%5D=2025-01-21
[fr-index]: https://www.federalregister.gov/presidential-documents/executive-orders/donald-trump/2025
[reddit]: https://www.reddit.com/r/Kalshi/comments/1i7d8d4/how_does_one_dispute_a_kalshi_outcome_anyone_else/
