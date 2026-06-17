# Kalshi: Miami high temperature and corrected NWS report

## Bottom line

**Finding: This was a real corrected-data dispute, but Kalshi appears to have had a strong written-rule defense. Confidence: low-medium.**

A Reddit thread alleges that Kalshi resolved a November 27, 2024 "Miami High" temperature market using an initial NWS report showing 84 degrees Fahrenheit, even though NWS later corrected the maximum temperature to 81 degrees.[^reddit]

The same thread contains the core defense: a commenter states that the contract expressly said subsequent corrections would not be taken into account.[^reddit] If that rule is accurate, Kalshi likely followed the contract even though the settlement may have reflected a bad initial data point.

## Market details

- **Venue:** Kalshi
- **Market:** Miami daily high temperature for November 27, 2024.
- **Alleged initial NWS value:** 84°F.
- **Alleged corrected value:** 81°F.
- **Alleged issue:** Kalshi used the initial erroneous report rather than the later correction.
- **Rule defense alleged in thread:** later corrections excluded.[^reddit]

## What happened

The Reddit poster claimed Kalshi resolved the Miami High market using an incorrect NWS report of 84°F rather than a corrected maximum of 81°F.[^reddit]

In comments, the same poster described the 84°F value as an obvious reporting error because it allegedly placed the high at 4:18 AM and the low at 6:50 AM, and said NWS corrected it about an hour after the report.[^reddit]

Another commenter responded that the contract "literally" said subsequent corrections would not be taken into account.[^reddit]

## The allegation against Kalshi

The allegation is that the market paid based on a physically erroneous initial source value, even after the source corrected it.

This is structurally similar to other "initial data vs final data" cases: administrative finality makes settlement fast and predictable, but it can pay the side that is wrong under the later corrected real-world record.

## Kalshi's defense

The strongest defense is the no-corrections rule described in the thread.

If the contract said subsequent corrections do not count, then Kalshi did not violate the rule by using the first NWS value. The complaint is then about rule design and user expectations, not about ignoring the contract.

## Assessment

### Did the data reportedly change from 84°F to 81°F?

**Yes, according to the Reddit thread.**[^reddit]

### Did the contract reportedly exclude later corrections?

**Yes, according to a counterparty comment in the same thread.**[^reddit]

### Is there independent verification of the NWS correction and exact Kalshi terms?

**No.** No archived NWS product or Kalshi contract was located during this pass.

### Was this a real failure for the tracker?

**Yes, but only as a low-confidence rule-design/source-finality case.**

### Overall classification

- **Initial source vs corrected source:** Alleged
- **Explicit no-corrections defense:** Strong if accurately quoted
- **Final misresolution under written rule:** Not established
- **Best public verdict:** Blocker/low-confidence case; likely rule-design problem rather than rule violation

## Precise blocker to a stronger finding

The missing evidence is the exact Kalshi contract PDF and the NWS observation/report/correction record. Without those, the case should not be presented as a proven Kalshi misresolution.

## Sources

[^reddit]: Reddit, r/Kalshi, ["Were you impacted by Kalshi's incorrect resolution of the 'Miami High' market for November 27, 2024?"][reddit], November 2024. Contains the 84°F/81°F allegation, claimed timing of the correction, and a counterargument that later corrections were excluded by the contract.

[reddit]: https://www.reddit.com/r/Kalshi/comments/1h1zjhb/were_you_impacted_by_kalshis_incorrect_resolution/
