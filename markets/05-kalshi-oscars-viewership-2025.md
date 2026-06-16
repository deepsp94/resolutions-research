# Kalshi: 2025 Oscars viewership

## Bottom line

**Finding: This was a real customer-facing resolution controversy and a weak market-design choice, but not a proven Kalshi settlement error. Confidence: high.**

Kalshi offered contracts on 2025 Oscars viewership, including whether the audience would exceed **19.5 million** viewers. The contracts resolved using the initially reported figure of roughly **18.1 million**, so the 19.5-million threshold resolved **No**.[^predictionnews-ufc][^predictionnews-resolutions]

Later reporting put the audience at about **19.7 million** after Nielsen/ABC included additional viewing on phones, tablets, and computers. That later figure would have made the 19.5-million threshold **Yes**.[^washington-post][^ap]

The apparent contradiction is real: a user asking "how many people watched the Oscars?" would now usually see the 19.7-million figure, while Kalshi paid the contract using the lower initial figure. But Kalshi's written contract terms expressly said that revisions to the underlying made after expiration would not count, and PredictionNews reports that Kalshi defended the settlement on that basis.[^contract-terms][^predictionnews-resolutions]

The best classification is therefore:

- **Wrong final-real-world proxy:** yes, if the market is understood as final Oscars viewership.
- **Wrong settlement under the written rule:** not established.
- **Platform mistake:** yes, but mainly in product design and user communication, not in ignoring its own rule.

## Market details

- **Venue:** Kalshi
- **Market family:** 2025 Oscars viewership contracts
- **Relevant threshold:** above 19.5 million viewers
- **Event:** 97th Academy Awards, held March 2, 2025
- **Initial figure used for settlement:** approximately 18.1 million / "just over 18m"
- **Later expanded figure:** approximately 19.7 million / 19.69 million
- **Result for 19.5-million threshold:** No
- **Primary contract terms:** [Kalshi `OSCARVIEWER` contract terms][contract-terms]

I was not able to recover the live Kalshi market page or ticker from Kalshi's current public markets API. The full contract-terms PDF is available from Kalshi's public document store, and PredictionNews preserves the relevant threshold, result, and Kalshi's stated rationale.[^contract-terms][^predictionnews-resolutions]

## The rule

The Kalshi contract terms defined the underlying as the reported viewer count for the Academy Awards telecast in the specified year.

The decisive sentence was:

> Revisions to the Underlying made after Expiration will not be accounted for in determining the Expiration Value.

The source agencies were listed in priority order: The New York Times, Deadline, Variety, CBS News, The Guardian, the Associated Press, The Washington Post, the Hollywood Reporter, and Nielsen.[^contract-terms]

The Expiration Value was the underlying value documented by the source agency on the expiration date at the expiration time.[^contract-terms]

That rule did **not** ask for the final, most complete Nielsen number. It asked for a reported number at a specified time and excluded later revisions.

## What happened

### Initial reporting showed about 18.1 million

Early Nielsen "Fast Nationals" reported about **18.1 million** viewers. The Guardian, relying on Nielsen figures, reported that viewership had slipped to "just over 18m" across ABC and Hulu.[^guardian]

PredictionNews reports that The New York Times initially reported about **18 million** viewers and that Kalshi's contracts above **19.5 million** resolved **No**.[^predictionnews-resolutions][^predictionnews-ufc]

### Later reporting showed about 19.7 million

The Washington Post later reported that Nielsen's first numbers counted only viewers watching the ABC telecast or Hulu livestream on televisions, while the final total included viewers watching on phones, tablets, and computers. The updated figure was around **19.7 million**.[^washington-post]

The Associated Press likewise reported that ABC's Tuesday figures showed an estimated **19.7 million** viewers, the biggest Oscars audience in five years.[^ap]

For a contract asking simply whether Oscars viewership exceeded 19.5 million, that later number looks like a Yes.

## The allegation against Kalshi

### 1. The settlement no longer matches the commonly reported event fact

After the updated Nielsen/ABC figure, the ordinary answer to "how many people watched the 2025 Oscars?" became about **19.7 million**. Kalshi's 19.5-million threshold remained settled **No**.

This is the core user-facing problem. The market's settled answer became misleading as a reference for final Oscars viewership.

### 2. The initial figure was not just a normal final revision

The gap was not a trivial rounding change. The initial number excluded categories of streaming viewers that mattered in 2025 because the Oscars were streamed live on Hulu for the first time. The Washington Post specifically attributed the difference to the first report counting television viewing only, while the later total included mobile and computer streams.[^washington-post]

That means the contract selected a narrower early measurement of the audience rather than the eventual fuller measure of the same event.

### 3. The product framing invited a broader interpretation than the rule

The market was understood publicly as an Oscars viewership market. In ordinary media usage, the 19.7-million figure became the reported viewership for the 2025 Oscars.

Kalshi's detailed rule, however, effectively made the contract about the first qualifying published viewership number by the expiration time. That is a legitimate settlement design, but it is not the same informational product as final viewership.

## Kalshi's defense

### Explicit / reported defense

PredictionNews reports that Kalshi did not change the resolution because the market rules stated that the initial release would count and future revisions would not. It also quotes a Kalshi operations-team member as saying the market was "determined correctly" while acknowledging that it was unfortunate the market did not account for data revisions.[^predictionnews-resolutions]

That defense is strongly supported by Kalshi's contract terms. The terms expressly exclude revisions to the underlying after expiration.[^contract-terms]

### Strongest rule-based defense

Kalshi's strongest defense is straightforward:

1. The written contract selected a measurement as documented by named source agencies at expiration.
2. It expressly excluded later revisions.
3. The initial report was below 19.5 million.
4. The later 19.7-million figure was a revision or expanded release after the initial report.
5. Therefore the 19.5-million contract should remain No under the written rule.

This is not a case where the venue appears to have ignored its own source hierarchy or secretly changed the rule after trading.

### Why that defense is incomplete

The rule was clear in a narrow legal sense, but it was a poor proxy for the thing many traders likely thought they were forecasting.

The 2025 Oscars had a new distribution feature: live streaming on Hulu. The first reported number missed meaningful categories of streaming viewers, while the later number became the more complete public audience figure.[^washington-post] A market that advertises itself as viewership but mechanically excludes a same-week expanded count can pay an answer that looks false to ordinary users.

Kalshi could have avoided the controversy by stating more prominently that the contract was about the **initial reported viewership figure**, not final viewership, or by waiting for a fuller Nielsen/ABC release.

## Assessment

### Did Kalshi pay the wrong side under the contract?

**Not established.**

The available evidence indicates Kalshi followed the written rule. The rule excluded post-expiration revisions, and the lower initial figure was below 19.5 million.[^contract-terms][^predictionnews-resolutions]

### Did Kalshi's settlement contradict the later best-known viewership number?

**Yes.**

The later figure of about 19.7 million exceeded the 19.5-million threshold. That is why traders who treated the market as final Oscars viewership saw the No resolution as wrong.[^washington-post][^predictionnews-ufc]

### Was the rule badly designed?

**Yes, materially.**

Using an initial report can make sense for administrative finality. But here the initial number differed materially from the later fuller number because of how streaming viewers were counted. The contract was easy to settle but did not robustly measure final viewership.

### Was this a real failure for the tracker?

**Yes, but it should be classified carefully.**

This is not an operational misgrade like paying the wrong winner. It is a rule-design failure: Kalshi wrote and applied a rule that prioritized quick finality over the most complete eventual measurement of the event. The result was contractually defensible but publicly misleading.

### Overall classification

- **Operational settlement error:** Not established
- **Rule followed as written:** Yes, on available evidence
- **Final-real-world mismatch:** Yes
- **Rule-design weakness:** Yes
- **Transparency / user-expectation problem:** Yes
- **Best public verdict:** Contractually defensible settlement; poor market design for final viewership

## Precise blocker to a stronger finding

The remaining blocker is not the final audience number. That is well supported at roughly 19.7 million.

The missing piece is the exact live Kalshi market page or ticker showing every listed threshold, final settlement value, expiration timestamp, and user-facing title as displayed during trading. The full contract terms and PredictionNews reporting are enough to classify the incident, but the archived live page would make the market-details section more complete.

## Sources

### Primary / platform

[^contract-terms]: Kalshi, [`OSCARVIEWER` contract terms][contract-terms]. Defines the underlying, source agencies, expiration value, and exclusion of post-expiration revisions.

### Contemporaneous and industry reporting

[^guardian]: The Guardian, ["Oscars telecast ratings fall 7% to 18m viewers"][guardian], March 4, 2025. Reports the initial Nielsen figure as "just over 18m" across ABC and Hulu.

[^washington-post]: The Washington Post, ["Turns out the 2025 Oscars ratings saw some improvement"][washington-post], updated March 4, 2025. Explains the difference between the initial Fast Nationals and later 19.7-million figure.

[^ap]: Associated Press, ["The Oscars get their biggest audience in 5 years despite dominance of 'Anora' and other small films"][ap], March 4, 2025. Reports ABC's estimated 19.7-million figure.

[^predictionnews-resolutions]: PredictionNews, ["Prediction Market Resolutions: The Good, Bad, and Ugly"][predictionnews-resolutions], updated August 8, 2025. Describes the Kalshi Oscars controversy, the initial and revised figures, the rule excluding revisions, and Kalshi's reported defense.

[^predictionnews-ufc]: PredictionNews, ["Kalshi UFC Resolution Echoes 2025 Oscars Viewership Market"][predictionnews-ufc], April 13, 2026. Summarizes the Oscars viewership controversy while comparing it to another initial-result-versus-correction settlement.

[contract-terms]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/OSCARSVIEWER.pdf
[guardian]: https://www.theguardian.com/film/2025/mar/04/oscars-telecast-ratings-fall-7-to-18m-viewers
[washington-post]: https://www.washingtonpost.com/style/2025/03/04/oscars-ratings-decline-97th-academy-awards/
[ap]: https://apnews.com/article/9d82cd9ea1afa4675ca1cf797c483684
[predictionnews-resolutions]: https://predictionnews.com/learn/resolutions/
[predictionnews-ufc]: https://predictionnews.com/news/kalshi-ufc-resolution-echoes-2025-oscars-viewership-market
