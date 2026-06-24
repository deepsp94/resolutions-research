# Polymarket: Israel-Hezbollah cease-fire extension market

## Bottom line

**Finding: Failure. Polymarket resolved the "Israel x Hezbollah ceasefire extended by April 26, 2026?" market Yes even though the only announced extension was an Israel-Lebanon ambassador-level deal that Hezbollah was excluded from and publicly rejected, contradicting the market's own rule naming Hezbollah as a required confirming party. The structurally identical, same-drafter "US x Iran ceasefire extended by" twin resolved No on the very same "named party didn't confirm" gap. Confidence: high that the resolution contradicts the rule and the US-Iran twin; medium that a Yes was indefensible (the media-consensus fallback gives a fig leaf).**

This is the genuinely anomalous contract in the family. The ~$20.9M extension market resolved Yes after two UMA dispute cycles,[^gamma-ext] yet the real-world event it cited was negotiated between the Israeli and Lebanese *ambassadors* at the White House, with Hezbollah neither party to nor a confirmer of the deal.[^cnbc][^yalibnan] The near-twin US-Iran extension market, written with the same "clear public confirmation from both [governments]" rule, resolved No on an identical defect.[^gamma-iran]

(Note: a prior version of this case file analyzed the wrong contract — the April 18 "Israel x Hezbollah ceasefire by" market, ~$98-112M, slug `israel-x-hezbollah-ceasefire-by`. That market also drew two UMA disputes and is differently and more weakly worded; it is not the anomalous result. The disputed contract here is the *extension* market.)

## Market details

- **Venue:** Polymarket
- **Event:** `israel-x-hezbollah-ceasefire-extended-by`
- **Sub-market:** "Israel x Hezbollah Ceasefire extended by April 26, 2026?" (slug `...-extended-by-april-26-2026`)
- **Volume:** ~$20.9M (gamma reports $20,894,917.90).[^gamma-ext]
- **Closed:** May 1, 2026.[^gamma-ext]
- **Resolution:** Yes (gamma `outcomePrices` `["1","0"]`), after two UMA dispute cycles (`umaResolutionStatuses` `["proposed","disputed","proposed","disputed"]`).[^gamma-ext]
- **Core rule:** Requires "clear public confirmation from both the Israeli government and Hezbollah" of a longer-than-10-day halt, or an official extension "confirmed by an overwhelming consensus of media reporting"; explicitly excludes informal understandings, backchannel communication, de-escalation, or unilateral pauses.[^gamma-ext]

## What happened

The extension market's verbatim rule reads: "An extension of the ceasefire agreement requires clear public confirmation from both the Israeli government and Hezbollah that they have agreed to halt military hostilities against one another for longer than the initially agreed 10-day period, or for an official extension of the ceasefire agreement in place to be otherwise confirmed by an overwhelming consensus of media reporting." It adds that resolution "will be based on official statements from the Israeli government and Hezbollah," with overwhelming credible-media consensus of an "official ceasefire extension agreement" sufficing, and excludes "Any form of informal understanding, backchannel communication, de-escalation, or unilateral pause in hostilities without a confirmed agreement on a qualifying extension."[^gamma-ext]

The only announced extension came on April 23, 2026, when President Trump said on Truth Social that Israel and Lebanon had agreed to a three-week extension. It was negotiated at the White House by the Israeli and Lebanese ambassadors (with US ambassadors Huckabee and Issa present); Trump framed it as the US working "with Lebanon in order to help it protect itself from Hezbollah."[^cnbc] Hezbollah was not a party to the talks.[^cnbc][^yalibnan] Hezbollah publicly rejected it: MP Ali Fayyad, on Hezbollah's Al-Manar, called the truce "meaningless," said the group "firmly rejects" the extension because it was excluded from the negotiations, and asserted a right to respond to Israeli operations.[^yalibnan] On April 29, 2026, IDF Chief of Staff Lt. Gen. Eyal Zamir told troops in southern Lebanon "there is no ceasefire" as the two sides continued exchanging fire.[^toi-zamir]

## The allegation against Polymarket

The contract names Hezbollah — by name — as a required confirming party. Hezbollah did the opposite of confirming: it was excluded from the deal and publicly called it meaningless.[^cnbc][^yalibnan] The deal that was struck was an Israel-Lebanon, ambassador-level government arrangement — precisely the kind of "informal understanding" / non-Hezbollah agreement the rule's exclusion clause targets, since Hezbollah neither signed nor confirmed it. Resolving Yes therefore reads Hezbollah's confirmation requirement out of the rule.

The strongest evidence of inconsistency is internal: the structurally identical "US x Iran ceasefire extended by" family, written with the same "clear public confirmation from both [governments]" standard, resolved **No** (gamma `outcomePrices` `["0","1"]`) on the same defect — a named party not confirming — with one April 22 sub-market grinding through six dispute cycles.[^gamma-iran] Two near-identical contracts resolved oppositely on the same structural gap.

## Polymarket's / the resolver's defense

Two arguments cut for Yes, and should be stated fairly.

First, the media-consensus fallback. Many credible outlets loosely headlined the event as extending the "Israel-Hezbollah ceasefire" — Euronews ran exactly that headline[^euronews] — because the original April 16 truce was itself an Israel-Lebanon arrangement *aimed at* Hezbollah. A UMA voter could argue an "overwhelming consensus of media reporting" labeled this an Israel-Hezbollah extension, satisfying the fallback prong.

Second, takes-effect-or-not is irrelevant by rule: the market triggered on an announced extension regardless of "whether the extension ultimately takes effect," so the later collapse of the truce (Zamir's "no ceasefire") does not, on its own, undermine a Yes.

These give Yes a fig leaf. But they sit against the fallback's own text, which requires consensus that an *official ceasefire extension agreement* — i.e., one between the named parties — was reached, while the underlying reporting itself stated Hezbollah was excluded.[^cnbc][^yalibnan]

## Assessment

### Did the rule require Hezbollah's confirmation, and did Hezbollah confirm?

**Yes, it required it; no, Hezbollah did not.** The rule names Hezbollah as a confirming party.[^gamma-ext] Hezbollah was not party to the deal and publicly rejected it as "meaningless."[^cnbc][^yalibnan]

### Does the media-consensus fallback rescue a Yes?

**Only weakly.** Outlets did headline an "Israel-Hezbollah ceasefire" extension,[^euronews] but the fallback requires consensus that an *official agreement between the named parties* was reached, and the same reporting documented Hezbollah's exclusion.[^cnbc][^yalibnan] It is a fig leaf, not a clean trigger.

### Is the result inconsistent with comparable Polymarket resolutions?

**Yes.** The same-drafter US-Iran extension family, with the identical both-parties rule, resolved No on the same "named party didn't confirm" gap.[^gamma-iran] That is strong evidence the Yes here is an inconsistency, not a principled reading.

### Was this a real failure for the tracker?

**Yes.** A Yes resolution contradicts the market's own both-parties rule and its near-twin's outcome. The defense is real but thin.

### Overall classification

- **Exact market located:** Yes (extension market, not the "ceasefire by" market)
- **UMA dispute:** Yes (two cycles)
- **Rule contradicted:** Yes — Hezbollah named as confirmer; Hezbollah excluded and rejected
- **Internal inconsistency:** Strong — US-Iran twin resolved No on identical defect
- **Media-consensus fig leaf:** Present but weak
- **Remediation:** None — bad Yes stands on-chain; settled; not remedied (FAILURE_RESOLVED = Unresolved)
- **Best public verdict:** Failure. The Yes resolution contradicts the market's own both-parties confirmation rule and the oppositely-decided US-Iran twin; the media-consensus fallback gives Yes a defensible-looking but thin justification.

## Precise blocker to a stronger finding

None material to the failure finding. The rule text, both outcomes, the dispute counts, and the real-world facts (ambassador-level Israel-Lebanon deal, Hezbollah excluded and rejecting, fighting continuing) are all on the record. The only thing not captured is the exact UMA voter rationale and per-vote timestamps for the two dispute cycles — useful color, but not needed to establish that Yes contradicts the named-party rule and the US-Iran twin.

## Sources

[^gamma-ext]: Polymarket gamma API, ["israel-x-hezbollah-ceasefire-extended-by" event][gamma-ext]. Verbatim both-parties rule and exclusion clause; sub-market "Israel x Hezbollah Ceasefire extended by April 26, 2026?"; ~$20.9M volume; closed May 1, 2026; `outcomePrices` `["1","0"]` (Yes); `umaResolutionStatuses` `["proposed","disputed","proposed","disputed"]`.

[^gamma-iran]: Polymarket gamma API, ["us-x-iran-ceasefire-extended-by" event][gamma-iran]. Same "clear public confirmation from both [governments]" rule; sub-markets resolved No (`outcomePrices` `["0","1"]`); the April 22 sub-market went through six dispute cycles.

[^cnbc]: CNBC, ["Trump says Israel-Lebanon ceasefire extended by three weeks"][cnbc], April 23, 2026. White House meeting with the Israeli and Lebanese ambassadors; Trump frames the US as helping Lebanon "protect itself from Hezbollah"; Hezbollah not party to the talks and rejecting any agreements made in them. (Washington Post and Axios corroborate the ambassador-level, Israel-Lebanon framing.[^wapo])

[^wapo]: Washington Post, ["Israel and Lebanon extend ceasefire for three weeks, Trump says"][wapo], April 23, 2026. Corroborates the Israel-Lebanon, government-level extension and Hezbollah's exclusion.

[^yalibnan]: Ya Libnan, ["Defiant Hezbollah calls Israel-Lebanon ceasefire extension meaningless"][yalibnan], April 24, 2026. Hezbollah MP Ali Fayyad, on Al-Manar, calls the truce "meaningless" and says Hezbollah "firmly rejects" the extension because it was excluded from the negotiations.

[^euronews]: Euronews, ["Israel-Hezbollah ceasefire extended by three weeks, Trump says"][euronews], April 24, 2026. Example of outlets loosely headlining the event as an "Israel-Hezbollah" ceasefire extension — the basis for the media-consensus defense.

[^toi-zamir]: The Times of Israel, ["IDF chief says there's 'no ceasefire' in south Lebanon amid continued fighting with Hezbollah"][toi-zamir], April 29, 2026. Lt. Gen. Eyal Zamir: "there is no ceasefire" on the combat front as Israel and Hezbollah keep exchanging fire.

[gamma-ext]: https://gamma-api.polymarket.com/events?slug=israel-x-hezbollah-ceasefire-extended-by
[gamma-iran]: https://gamma-api.polymarket.com/events?slug=us-x-iran-ceasefire-extended-by
[cnbc]: https://www.cnbc.com/2026/04/23/trump-israel-lebanon-ceasefire-iran-war.html
[wapo]: https://www.washingtonpost.com/national-security/2026/04/23/us-israel-lebanon-ceasefire/
[yalibnan]: https://yalibnan.com/2026/04/24/defiant-hezbollah-calls-israel-lebanon-ceasefire-extension-meaningless/
[euronews]: https://www.euronews.com/2026/04/24/trump-says-israel-hezbollah-ceasefire-extended-by-three-weeks
[toi-zamir]: https://www.timesofisrael.com/idf-chief-says-theres-no-ceasefire-in-south-lebanon-amid-continued-fighting-with-hezbollah/
