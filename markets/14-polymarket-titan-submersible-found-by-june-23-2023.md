# Polymarket: Titan submersible found by June 23, 2023

## Bottom line

**Finding: This was a real resolution controversy and likely a written-rule failure. Confidence: medium-high.**

Polymarket asked whether the missing OceanGate vessel exploring the Titanic wreck would be found by June 23, 2023. The market resolved **Yes** after a debris field from the Titan was located and officials concluded the vessel had suffered a catastrophic implosion.[^polymarket-api][^dlnews][^axios]

The problem is that Polymarket's own rule tried to narrow what "found" meant. It said the vessel did not need to be rescued or physically recovered, but it also said that if pieces were located without the cabin containing the passengers, that would not suffice for Yes.[^polymarket-api]

The public evidence available at the time centered on debris, pieces, and catastrophic loss of the pressure chamber. DL News reported that No holders pointed to the fine print, while UMA voters resolved Yes. UMA founder Hart Lambur defended the outcome on the ground that ordinary people would say the sub had been found.[^dlnews]

This belongs in the tracker as a **literal written-rule versus perceived-spirit failure**. The Yes outcome was understandable in ordinary language, but the strongest available evidence indicates that the resolution discounted or softened the explicit pieces/cabin limitation.

## Market details

- **Venue:** Polymarket
- **Question:** `Will the missing submarine be found by June 23?`
- **Market rule:** Yes if the OceanGate vessel was found by Friday, June 23, 2023, 11:59:59 PM ET.
- **Key caveat:** The vessel did not need to be rescued or physically recovered, but pieces alone would not suffice if the cabin containing the passengers was not located.
- **Resolution source:** Official statement from OceanGate, the U.S. Coast Guard, or another credible government agency; if none, credible-reporting consensus.
- **Archived volume:** about $2.25 million in Polymarket's public event API.
- **Final result:** Yes.[^polymarket-api]

Polymarket's archived description also records that the market was sent to UMA dispute resolution.[^polymarket-api]

## What happened in the real world

The Titan submersible lost contact during a dive to the Titanic wreck on June 18, 2023. On June 22, searchers found a debris field near the Titanic. Reporting based on U.S. Coast Guard statements described debris from the submersible and a catastrophic implosion.[^axios][^wired]

Axios reported that OceanGate believed all five passengers had died and that the Coast Guard confirmed debris near the Titanic wreck site indicated catastrophic loss of the vessel's pressure chamber.[^axios]

Wired similarly reported that Coast Guard officials found debris from the submersible about 1,600 feet from the Titanic's bow and that the debris included the nose cone and parts of the pressure hull.[^wired]

Those facts strongly established that the missing vessel's fate and location had been determined. They did not cleanly establish that the "cabin which contains the vessel's passengers," in the sense used by Polymarket's caveat, had been found before the deadline.

## What happened on Polymarket

Polymarket resolved the market Yes after UMA dispute resolution.[^polymarket-api][^dlnews]

DL News reported that Yes holders won after the Coast Guard announcement that pieces of the submersible had been found on the ocean floor. No holders objected by pointing to Polymarket's fine print: pieces alone would not suffice unless the cabin containing the passengers was found.[^dlnews]

The controversy then became a dispute over whether the "spirit" of the question should control over the stricter caveat. DL News interviewed UMA founder Hart Lambur, who rejected collusion claims and defended the Yes outcome by saying ordinary people would likely say the sub had been found.[^dlnews]

## The allegation against Polymarket

### 1. The explicit caveat appears to favor No

The market did not merely ask whether searchers learned what happened to Titan. It added a caveat: pieces located without the passenger cabin would not suffice.[^polymarket-api]

The public facts cited by DL News, Axios, and Wired were debris, pieces, and pressure-hull or pressure-chamber loss.[^dlnews][^axios][^wired]

On a literal reading, that is exactly the scenario the caveat was designed to handle. Finding pieces of a destroyed vessel is not the same as finding the passenger cabin.

### 2. The resolution rewarded ordinary-language "found" despite narrower drafting

There was a strong ordinary-language reason for Yes. The search had located Titan's debris field, identified the vessel's fate, and ended the search-and-rescue uncertainty. But Polymarket's caveat made the market more specific than the title.

If the resolver wanted to follow ordinary language, the caveat should not have been written so narrowly. Once it was written, traders could reasonably expect it to control.

### 3. The market invited a title/rules conflict

The title asked a simple question: was the submarine found? The fine print asked a more technical one: were the right parts found?

That mismatch created the failure. Traders who priced the title and news outcome saw Yes; traders who priced the caveat saw No.

## Polymarket/UMA's defense

I did not find a separate detailed Polymarket statement defending the final result. The strongest defense is the UMA-side rationale reported by DL News.

That defense is:

- The Coast Guard and credible reporting established that the debris field was Titan and that the vessel had catastrophically imploded.[^axios][^wired]
- The market did not require rescue or physical recovery.[^polymarket-api]
- In common usage, a missing vessel can be considered "found" once its wreckage is located and identified.
- Lambur argued that most ordinary people asked whether the sub was found would likely answer yes.[^dlnews]

Under that view, the Yes resolution captured the practical information the market was meant to forecast: whether the missing vessel would be located before the deadline.

## Assessment

### Was Titan's debris field located before the deadline?

**Yes.**

Contemporaneous reporting based on Coast Guard statements says a debris field from Titan was found on June 22, before the June 23 deadline.[^axios][^wired]

### Was the vessel rescued or physically recovered before the deadline?

**No, and the market did not require that.**

The rule explicitly said rescue or physical recovery was not necessary.[^polymarket-api]

### Were only pieces located, without clear evidence that the passenger cabin was found?

**That is the strongest reading of the public record reviewed here.**

The reviewed sources describe debris, pieces, nose cone, and pressure-hull/pressure-chamber components.[^dlnews][^axios][^wired] They do not establish that the passenger cabin, as such, was located before the deadline.

### Was the Yes resolution clearly understandable?

**Yes.**

In ordinary language and in the practical search-and-rescue sense, the missing sub had been found: officials had located the wreckage and identified the disaster.

### Was the Yes resolution consistent with the literal caveat?

**Probably not.**

The caveat appears to exclude a Yes outcome based only on pieces unless the cabin containing passengers was located. The strongest available public evidence points to pieces/debris, not a located passenger cabin.

### Was this a real failure for the tracker?

**Yes.**

This is a good example of a market where the visible title, public news reality, and detailed resolution caveat pointed in different directions. The platform's resolution process appears to have favored the broad spirit of the question over the literal limiting language.

### Overall classification

- **Operational settlement error:** Not established
- **Semantic ambiguity:** Yes
- **Title/rules mismatch:** Yes
- **Likely written-rule mismatch:** Yes
- **Best public verdict:** Yes was understandable as ordinary truth; No was stronger under the specific pieces/cabin caveat

## Precise blocker to a stronger finding

The missing evidence is the full UMA vote record and any contemporaneous resolver rationale explaining why the caveat was satisfied. If UMA voters had evidence that the passenger cabin, as described in the market rule, was found before the deadline, the literal-rule critique would weaken. The reviewed sources do not show that.

## Sources

[^polymarket-api]: Polymarket Gamma API, [`will-the-missing-submarine-be-found-by-june-23` event][polymarket-api]. Archives the market question, detailed caveat, source language, UMA-dispute note, volume, and Yes outcome.

[^dlnews]: Aleks Gilbert, DL News, ["Crypto bettors' uproar over Titan submarine puts spotlight on 'decentralised truth'"][dlnews], July 1, 2023. Reports the fine-print dispute, UMA's Yes resolution, complaints about whale voting, and Hart Lambur's defense of the ordinary-language Yes outcome.

[^axios]: Axios, ["Titan submersible passengers believed to be dead, company says"][axios], June 22, 2023. Reports OceanGate's statement, Coast Guard confirmation, debris near the Titanic wreck site, and catastrophic loss of the pressure chamber.

[^wired]: Wired, ["Missing Sub Passengers Believed Dead After Debris Found From Likely Implosion"][wired], June 22, 2023. Reports that Coast Guard officials found Titan debris, including nose cone and pressure-hull parts, and concluded the passengers were believed dead after a catastrophic implosion.

[polymarket-api]: https://gamma-api.polymarket.com/events?slug=will-the-missing-submarine-be-found-by-june-23
[dlnews]: https://www.dlnews.com/articles/markets/crypto-bets-on-titan-sub-cause-uproar-at-uma-polymarket/
[axios]: https://www.axios.com/2023/06/22/titanic-tourist-submarine-missing-north-atlantic-air-supply
[wired]: https://www.wired.com/story/titan-sub-debris-found
