# Polymarket: Titan submersible found by June 23, 2023

## Bottom line

**Finding: Failure. Polymarket's rule narrowed "found" with a caveat that pieces alone would not suffice unless "the cabin which contains the vessel's passengers" was located — yet UMA resolved Yes after only debris was found (end bells, tail cone, nose cone), with no intact cabin, no large carbon-fiber hull recovered, and human remains not recovered until June 28, after the deadline. UMA resolved on the broad ordinary-language reading, overriding its own narrower written rule. This is both a rule-drafting failure and a literal-rule-versus-resolution conflict. Confidence: high.**

Polymarket asked whether the missing OceanGate vessel exploring the Titanic wreck would be found by June 23, 2023. The market resolved **Yes** (`outcomePrices` `["1","0"]`), and the gamma record shows it was sent to UMA dispute resolution before resolving.[^gamma][^dlnews] A Titan debris field was located on June 22 and officials concluded the vessel had suffered a catastrophic implosion.[^gamma][^usni][^cbs]

The problem is that Polymarket's own rule narrowed what "found" meant in a way poorly matched to the facts. It said the vessel need not be rescued or physically recovered, but it also said that if pieces were located without "the cabin which contains the vessel's passengers," that would not suffice for Yes.[^gamma] That caveat was a bad rule for a deep-sea implosion: at Titanic depth the carbon-fiber pressure hull — the literal "cabin" — was the part most likely to be obliterated. A trader who correctly anticipated that searchers would find debris and identify the vessel's fate but would *not* find an intact passenger cabin could price the caveat as No and still lose when UMA resolved Yes on the broader ordinary-language view.

The public evidence at the deadline centered on debris, end bells, and loss of the pressure chamber — not a located cabin.[^usni][^cbs][^wiki] DL News reported that No holders pointed to the fine print while UMA voters resolved Yes, and UMA founder Hart Lambur defended the outcome on the ground that ordinary people would say the sub had been found.[^dlnews] This belongs in the tracker as a **literal written-rule versus perceived-spirit failure** layered on a **drafting failure**: the resolution discounted the explicit pieces/cabin limitation.

## Market details

- **Venue:** Polymarket
- **Market:** "Will the missing submarine be found by June 23?" — gamma event `902078`, slug `will-the-missing-submarine-be-found-by-june-23`, market id `251539`.[^gamma]
- **Governing rule:** Yes if the OceanGate vessel was found by Friday, June 23, 2023, 11:59:59 PM ET; rescue or physical recovery not required.[^gamma]
- **Cabin caveat (verbatim):** "If pieces are located, but not the cabin which contains the vessel's passengers, that will not suffice for this market to resolve to 'Yes.'"[^gamma]
- **Resolution source:** an official statement from OceanGate, the US Coast Guard, or another credible government agency; if none, a consensus of credible reporting.[^gamma]
- **Volume:** $2,253,929.[^gamma]
- **UMA status:** disputed and escalated to UMA (`umaResolutionStatus: resolved`); the description carries the UMA-dispute banner.[^gamma]
- **Outcome:** Yes (`outcomePrices` `["1","0"]`); closed June 26, 2023.[^gamma]

## What happened

The Titan lost contact during a dive to the Titanic on June 18, 2023. On June 22 — before the June 23 deadline — a remotely operated vehicle located a debris field about 1,600 feet from the Titanic's bow. The U.S. Coast Guard (Rear Admiral John Mauger) described the debris as consistent with a "catastrophic loss of the pressure chamber," i.e., an implosion, and officials concluded all five aboard had died.[^usni][^cbs]

The debris was **pieces, not an intact cabin**. The identified components were the tail cone (not part of the pressure vessel) and the forward and aft end bells (parts of the pressure vessel), located across two debris areas, along with the nose cone found first.[^wiki][^usni] No large pieces of the carbon-fiber pressure hull — the "cabin which contains the vessel's passengers" — are known to have been recovered; the hull had fragmented.[^wiki] Human remains were not recovered until **June 28, 2023**, when the *Horizon Arctic* returned them to St. John's — after the deadline.[^wiki]

Those facts established that the vessel's fate and location had been determined. They did not establish that the "cabin which contains the vessel's passengers," in the sense used by Polymarket's caveat, had been found before the deadline.

## What happened on Polymarket

Polymarket resolved the market Yes after UMA dispute resolution.[^gamma][^dlnews]

DL News reported that Yes holders won after the Coast Guard announcement that pieces of the submersible had been found on the ocean floor. No holders objected by pointing to the fine print: pieces alone would not suffice unless the cabin containing the passengers was found.[^dlnews] Disputers alleged the Yes outcome resulted from whale collusion — that a small set of recurring UMA token holders with unequal weight voted Yes — and questioned whether roughly 100 consistent voters constituted genuine decentralization.[^dlnews]

UMA founder Hart Lambur rejected the collusion claims and defended the Yes outcome on ordinary-language grounds, saying that if you "asked 100 people on the street," most would say "Yeah, it was found."[^dlnews] The controversy thus turned on whether the spirit of the question should control over the stricter caveat.

## The allegation against Polymarket

The objection is a literal reading of the contract: the market did not merely ask whether searchers learned what happened to Titan — it added a caveat that pieces located without the passenger cabin would not suffice.[^gamma] The public facts at the deadline were debris, end bells, and pressure-chamber loss — exactly the pieces-without-cabin scenario the caveat was written to exclude.[^usni][^cbs][^wiki] On that reading, finding fragments of a destroyed vessel is not finding the passenger cabin, and the market should have resolved No.

The deeper drafting problem is that the caveat made the market hinge on a condition that may have been physically unrealizable once catastrophic implosion was the event. It tried to distinguish "wreckage found" from "submarine found" but used the passenger cabin as the decisive marker, even though the carbon-fiber cabin was the part most likely to be obliterated.

## UMA's basis for Yes

There was a strong ordinary-language case for Yes, and that is the basis UMA acted on:[^dlnews]

1. **The Coast Guard satisfied the source requirement.** Credible government statements established that the debris field was Titan and that the vessel had catastrophically imploded.[^usni][^cbs]
2. **The rule did not require rescue or recovery.** "Found" did not demand physical recovery.[^gamma]
3. **Ordinary usage.** A missing vessel can be considered "found" once its wreckage is located and identified; Lambur argued most ordinary people would say the sub had been found.[^dlnews]

Under that view, the Yes outcome captured the practical information the market forecast — whether the missing vessel would be located before the deadline. But that view is the title, not the caveat: the resolution read past the explicit pieces/cabin limitation.

## Assessment

### Was Titan's debris field located before the deadline?

**Yes.** Contemporaneous Coast Guard reporting says a Titan debris field was found June 22, before the June 23 deadline.[^usni][^cbs]

### Was the vessel rescued or physically recovered before the deadline?

**No, and the rule did not require it.** The contract explicitly said rescue or physical recovery was not necessary.[^gamma]

### Was "the cabin which contains the vessel's passengers" located before the deadline?

**No.** The recovered debris was the tail cone, forward and aft end bells, and nose cone — pieces, not an intact cabin. No large carbon-fiber pressure-hull pieces are known to have been recovered, and human remains were not recovered until June 28, after the deadline.[^wiki][^usni] This is the precise scenario the caveat was written to exclude.

### Was the Yes resolution understandable in ordinary language?

**Yes.** In the practical search-and-rescue sense, the missing sub had been found: officials located the wreckage and identified the disaster.[^usni][^cbs]

### Was the Yes resolution consistent with the literal caveat?

**No.** The caveat excludes a Yes based only on pieces unless the cabin containing passengers was located. The public record points to pieces and end bells, not a located cabin — and Lambur defended the outcome on ordinary-language grounds, not on any claim the cabin had been found.[^gamma][^wiki][^dlnews]

### Was this a real failure for the tracker?

**Yes.** The visible title, the public news reality, and the detailed caveat pointed in different directions, and UMA resolved on the broad spirit over the literal limiting language. It is also a drafting failure: the pieces/cabin caveat was not a robust way to resolve a likely implosion, making the result turn on locating a passenger cabin that might no longer exist as an identifiable cabin. The rule should have specified whether a debris field or pressure-hull wreckage would count.

### Overall classification

- **Operational settlement error:** Not established
- **Semantic ambiguity:** Yes
- **Title/rules mismatch:** Yes
- **Clear rule-drafting failure:** Yes
- **Literal written-rule versus resolution mismatch:** Yes
- **Best public verdict:** Yes was understandable as ordinary truth; No was stronger under the specific pieces/cabin caveat — and UMA resolved against its own caveat

## Precise blocker to a stronger finding

The missing evidence is the full UMA per-voter vote record and any contemporaneous resolver rationale explaining why the caveat was deemed satisfied. If UMA voters had evidence that the passenger cabin, as described in the rule, was found before the deadline, the literal-rule critique would weaken. The reviewed sources do not show that — to the contrary, the debris was end bells and fragments, no large carbon-fiber hull was recovered, remains came on June 28, and Lambur's own defense rested on ordinary language rather than on a located cabin.[^gamma][^usni][^wiki][^dlnews]

## Sources

[^gamma]: Polymarket Gamma API, [`will-the-missing-submarine-be-found-by-june-23` event][gamma] (event `902078`, market `251539`). Archives the question, the verbatim cabin caveat ("If pieces are located, but not the cabin which contains the vessel's passengers, that will not suffice for this market to resolve to 'Yes.'"), the no-rescue/no-recovery language, the resolution-source language, the UMA-dispute banner, volume $2,253,929, `umaResolutionStatus: resolved`, and the Yes outcome (`outcomePrices` `["1","0"]`).

[^dlnews]: Aleks Gilbert, DL News, ["Crypto bettors' uproar over Titan submarine puts spotlight on 'decentralised truth'"][dlnews], July 1, 2023. Reports the fine-print dispute, UMA's Yes resolution, the whale-collusion complaints, and Hart Lambur's ordinary-language defense ("If you went and asked 100 people on the street… most would say 'Yeah, it was found.'").

[^usni]: USNI News, ["Coast Guard: Titan Submersible Suffered Catastrophic Loss; Debris Found Near Titanic Wreck"][usni], June 22, 2023. Reports the June 22 debris field ~1,600 ft from the Titanic bow, Rear Admiral Mauger's "catastrophic loss of the pressure chamber," and the recovered pieces (nose cone, end bells, tail cone).

[^cbs]: CBS News, ["Debris from OceanGate sub found 1,600 feet from Titanic after 'catastrophic implosion,' U.S. Coast Guard says"][cbs], June 22, 2023. Reports five major debris pieces, the catastrophic loss of the pressure chamber, and that all aboard were believed dead.

[^wiki]: Wikipedia, ["Titan submersible implosion"][wiki]. Records that the identified debris consisted of the tail cone (not part of the pressure vessel) and the forward and aft end bells (parts of the pressure vessel); that no large pieces of carbon fibre are known to have been recovered (the pressure hull was not found intact); and that human remains were recovered June 28, 2023, after the deadline.

[gamma]: https://gamma-api.polymarket.com/events?slug=will-the-missing-submarine-be-found-by-june-23
[dlnews]: https://www.dlnews.com/articles/markets/crypto-bets-on-titan-sub-cause-uproar-at-uma-polymarket/
[usni]: https://news.usni.org/2023/06/22/coast-guard-titan-submersible-suffered-catastrophic-loss-debris-found-near-titanic-wreck
[cbs]: https://www.cbsnews.com/news/missing-submarine-titanic-debris-field-oceangate-us-coast-guard/
[wiki]: https://en.wikipedia.org/wiki/Titan_submersible_implosion
