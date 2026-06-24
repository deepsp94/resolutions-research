# Polymarket: Israel invades Lebanon in September 2024

## Bottom line

**Finding: No failure. Polymarket's market resolved Yes only if Israel "commences a military offensive intended to establish control over any portion of Lebanon" between September 17 and September 30, 2024. Israel's late-September operation was an entry of ground forces explicitly framed by the IDF and Israeli officials as limited, targeted raids not intended to occupy Lebanese territory; no official source or credible-reporting consensus confirmed the rule's intent-to-establish-control condition. The market resolved No, and that No was a correct application of the written rule. Confidence: high.**

This case looks at first like a clean misresolution: the market is titled "Will Israel invade Lebanon in September?", Israeli ground forces did cross into southern Lebanon around the deadline, and major outlets used "invasion" and "incursion" language.[^gamma][^toi][^wiki] But the binding rule did not resolve on the word "invasion" or on ground entry alone. It required a military offensive **intended to establish control over any portion of Lebanon**, with the resolution source being official confirmation by Lebanon, Israel, the United Nations, or a UN Security Council permanent member, or a consensus of credible reporting.[^gamma]

That intent-to-control condition was not established. The IDF described the operation as "limited, localized, and targeted ground raids" against Hezbollah infrastructure near the border, and two Israeli officials said the security-cabinet decision emphasized the operation was limited in time and scope and was **not intended to occupy southern Lebanon**.[^toi][^lwj][^wiki] None of the four enumerated official sources confirmed control-intent, and the credible-reporting characterization matched the limited-raids framing.

The decisive point is that the No resolution holds **independent of the timing question.** Whether or not ground entry fell inside the September 17–30 window, the binding control-intent condition failed on the official and reported record. The gamma API records the market resolved No (`outcomePrices ["0","1"]`) with `umaResolutionStatus: resolved`.[^gamma] Applying a written rule's narrowing condition as drafted is not a resolution failure.

## Market details

- **Venue:** Polymarket
- **Market:** "Will Israel invade Lebanon in September?" — gamma event/market slug `will-israel-invade-lebanon-in-september` (event id 12681, market id 507417, conditionId `0xab66…4df5`).[^gamma]
- **Date window:** September 17, 2024 through September 30, 2024, 11:59 PM ET.[^gamma]
- **Payout criterion (verbatim):** "This market will resolve to 'Yes' if Israel commences a military offensive intended to establish control over any portion of Lebanon between September 17, 2024 and September 30, 2024, 11:59 PM ET. Otherwise, this market will resolve to 'No'."[^gamma]
- **Resolution source (verbatim):** "official confirmation by Lebanon, Israel, the United Nations, or any permanent member of the UN Security Council, however a consensus of credible reporting will also be used."[^gamma]
- **Volume:** about $13.8 million.[^gamma]
- **Outcome:** No (`outcomePrices ["0","1"]`); `umaResolutionStatus: resolved`; closed/UMA-finalized October 8, 2024.[^gamma]

## What happened in the real world

Israel began ground operations into southern Lebanon around the close of the market window — the operation began the evening of September 30 / into October 1, 2024 (Israel local time, UTC+3), and the IDF publicly confirmed it in the early hours of October 1 local time, stating that "limited, localized, and targeted ground raids" against Hezbollah targets and infrastructure had begun several hours earlier.[^toi][^lwj] Wikipedia dates the cross-border raids to October 1, characterizing September 30 as the preparatory phase (the US was notified; Lebanese forces withdrew from the border).[^wiki]

On intent, the operation was consistently described as limited and targeted, not as a campaign to hold or govern Lebanese territory. Two Israeli officials told Axios the security-cabinet decision was limited in time and scope and was **not intended to occupy southern Lebanon**, and Israel publicly stated it had "no intentions for long-term occupation."[^axios][^wiki] The raids focused on Hezbollah infrastructure in border villages "only hundreds of meters across the border."[^wiki]

Those facts explain why a dispute existed — ground troops crossed and outlets used invasion language — but they do not satisfy the market's stated intent-to-establish-control requirement.

## The allegation against Polymarket

The user-facing complaint was understandable: Israeli troops entered Lebanon and many outlets used invasion/incursion language, so a trader reading only the short title could have expected Yes.[^toi][^wiki] But the detailed rule controlled, and it required a military offensive intended to establish control over part of Lebanon. Titles are short labels; they do not repeat every condition in the rules.[^gamma]

The strongest Yes argument would need to show that one of the specified official sources — or a credible-reporting consensus — confirmed that Israel intended to establish control over part of Lebanon within the window. The reviewed record does not show that.

## Polymarket's basis for No

The defense is the written rule and the source record:

1. **The rule required intent to establish control, not mere entry.** Yes resolution was conditioned on Israel commencing "a military offensive intended to establish control over any portion of Lebanon," not on ground troops crossing the border.[^gamma]

2. **Official Israeli framing was the opposite of control-intent.** The IDF framed the operation as limited, localized, targeted raids against Hezbollah targets near the border, and Israeli officials said it was not intended to occupy southern Lebanon and had no intention of long-term occupation.[^toi][^axios][^wiki][^lwj] None of the four enumerated official sources confirmed an intent to establish control, and the credible-reporting characterization matched the limited-raids framing.

## Assessment

### Did Israeli ground forces enter Lebanon around the market deadline?

**Yes.** Israel began ground operations into southern Lebanon the evening of September 30 / into October 1, 2024, confirmed by the IDF on October 1 local time.[^toi][^lwj][^wiki]

### Did credible reporting use invasion/incursion language?

**Yes.** Major outlets described the operation as a ground invasion or incursion.[^toi][^wiki]

### Did the written rule require more than entry?

**Yes.** The binding rule required a military offensive **intended to establish control** over any portion of Lebanon.[^gamma]

### Was the control-intent condition satisfied on the official or credible-reporting record?

**No.** The IDF and Israeli officials described the operation as limited and targeted and explicitly not intended to occupy southern Lebanon; no enumerated official source confirmed intent to establish control.[^toi][^axios][^wiki][^lwj]

### Does the No resolution depend on the timing question?

**No — and this is decisive.** Even if the ground entry fell inside the September 17–30, 11:59 PM ET window, the binding intent-to-establish-control condition failed on the official and reported record. The No holds independent of whether entry was inside or outside the window.

### So was this a resolution failure?

**No — it was a rule applied as written.** The intent-to-control condition was a clear, outcome-determinative narrowing of the title, and it was not met. The gamma record confirms the market resolved No with UMA status resolved.[^gamma]

### Overall classification

- **Settlement consistent with the governing written rule:** Yes
- **Misapplication of the rules:** No
- **Title-vs-rule ambiguity:** Low to moderate — the title alone could mislead, but the detailed rule is clear and was applied
- **Ground entry:** Yes
- **Intent to establish control:** Not established
- **Best public verdict:** No failure

## Precise blocker to a stronger contrary finding

To prove a resolution error, the evidence would need to show that one of the enumerated official sources — or a credible-reporting consensus — confirmed Israel's September 2024 operation was intended to establish control over part of Lebanon within the market window, despite official and reported statements that it was limited and not intended as an occupation. The reviewed primary record does not establish that. A secondary residual: the multi-round propose/dispute history (Yes proposed and disputed, No proposed and disputed) is sourced to the archived Polymarket page and contemporaneous reporting; gamma's current snapshot shows only the final resolved-No state with an empty `umaResolutionStatuses` array, so that propose/dispute sequence is not independently re-confirmed on-chain here.

## Sources

[^gamma]: Polymarket Gamma API, event/market `will-israel-invade-lebanon-in-september` (event id 12681; market id 507417; conditionId `0xab66a7d5…e4df5`). Description (binding rule): "This market will resolve to 'Yes' if Israel commences a military offensive intended to establish control over any portion of Lebanon between September 17, 2024 and September 30, 2024, 11:59 PM ET. Otherwise… 'No'." Resolution source: official confirmation by Lebanon, Israel, the UN, or a UNSC permanent member, or a consensus of credible reporting. `outcomePrices` `["0","1"]` (No), `umaResolutionStatus` `resolved`, `umaResolutionStatuses` `[]`, volume ~$13.8M, closed/UMA-finalized 2024-10-08. [Gamma][gamma]

[^toi]: The Times of Israel, "IDF announces launch of limited ground raids of Hezbollah sites across Lebanon border," October 1, 2024. IDF confirmed in the early hours of October 1 (Israel time) that "limited, localized, and targeted ground raids" against Hezbollah targets and infrastructure had begun several hours earlier; outlets described the operation as an invasion/incursion. [Article][toi]

[^axios]: Barak Ravid, Axios, "Israel begins ground operation in southern Lebanon," updated September 30, 2024. Reports the IDF's limited-raids framing and that two Israeli officials said the security-cabinet decision emphasized the operation was limited in time and scope and was not intended to occupy southern Lebanon. (Direct fetch returned 403/451; substance corroborated by Times of Israel, Long War Journal, and Wikipedia.) [Article][axios]

[^lwj]: FDD's Long War Journal, "IDF begins Lebanon ground operation, Iran launches 180 ballistic missiles at Israel," October 1, 2024. Operation began the evening of September 30 into October 1; IDF described "localized and targeted ground raids based on precise intelligence against Hezbollah… targets and infrastructure in southern Lebanon," confirmed via Telegram on October 1. [Article][lwj]

[^wiki]: Wikipedia, "2024 Israeli invasion of Lebanon." Dates the cross-border raids to October 1, 2024 (September 30 = preparatory phase); records Israel "preparing for a limited ground operation, with no intentions for long-term occupation," with troops operating in border villages "only hundreds of meters across the border." [Article][wiki]

[gamma]: https://gamma-api.polymarket.com/events?slug=will-israel-invade-lebanon-in-september
[toi]: https://www.timesofisrael.com/idf-announces-launch-of-limited-ground-raids-of-hezbollah-sites-across-lebanon-border/
[axios]: https://www.axios.com/2024/09/30/israel-ground-invasion-lebanon
[lwj]: https://www.longwarjournal.org/archives/2024/10/idf-begins-lebanon-ground-operation-iran-launches-180-ballistic-missiles-at-israel.php
[wiki]: https://en.wikipedia.org/wiki/2024_Israeli_invasion_of_Lebanon
