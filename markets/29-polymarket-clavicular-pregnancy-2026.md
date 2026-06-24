# Polymarket: Clavicular pregnancy market

## Bottom line

**Finding: Failure. Polymarket finalized a Yes resolution on a Kick-streamer "pregnancy" market built entirely on material that the reputable-media consensus treated as a joke, stunt, or debunked rumor — exactly the category the market's own credibility/joke-exclusion clause was supposed to exclude — and the bad Yes now stands as a final, automatically resolved outcome. Confidence: Medium-high.**

The market for `clavicular-pregnancy-in-2026` required a *credible* pregnancy announcement and expressly disqualified jokes and non-credible statements.[^gamma] It settled Yes (outcomePrices `["1","0"]`), is closed and resolved, and resolved early on May 1, 2026 rather than running to its scheduled December 31, 2026 end.[^gamma] Yet the only real-world basis was an April 2026 "pregnancy contest" / "I'm gonna be a dad" livestream stunt plus a viral rumor that the streamer had gotten a 10-day girlfriend pregnant — material that contemporaneous fact-checks uniformly found to be unconfirmed or false.[^toi][^complex] No credible-media consensus of an actual pregnancy ever existed. This is a credibility-rule / oracle-process failure, and it is **Unresolved**: the bad Yes stands and No-holders were not made whole.

## Market details

- **Venue:** Polymarket
- **Market:** `clavicular-pregnancy-in-2026` (event 400878 / market 2037907)
- **Market URL:** https://polymarket.com/event/clavicular-pregnancy-in-2026
- **Subject:** "Clavicular" is Kick streamer Braden Eric Peters.
- **Listed:** April 20, 2026; scheduled end December 31, 2026, 11:59 PM ET.
- **Resolved early:** May 1, 2026 (`closedTime` / `umaEndDate` 2026-05-01), automatically resolved, `umaResolutionStatus` "resolved".[^gamma]
- **Outcome:** Yes (`outcomePrices` `["1","0"]`), final — not in review.[^gamma]
- **Dispute history:** two UMA proposal/dispute cycles (`umaResolutionStatuses` `["proposed","disputed","proposed","disputed"]`).[^gamma]
- **Volume:** ~$13.9M on the Polymarket page; reported up to ~$16.46M in dispute coverage.[^gamma][^bitget]

## What happened

The market asked whether the Kick streamer Clavicular would credibly announce a pregnancy. The verbatim rule was: *"This market will resolve to 'Yes' if Clavicular announces that he and a partner are expecting a baby through pregnancy between market creation and December 31, 2026, 11:59 PM ET. Otherwise... 'No'. Only credible announcements will qualify. Pregnancy announcements that are not credible, for example jokes, will not suffice. This market will resolve based on the date of announcement... The resolution source will be statements from Clavicular or his representatives; however, a definitive consensus of credible media reporting may be considered."*[^gamma]

The real-world basis was thin. In April 2026 Clavicular ran a "pregnancy contest" / "I'm gonna be a dad" livestream stunt, and a viral rumor spread that he had gotten a girlfriend of about 10 days pregnant. Reputable fact-checks did not corroborate any pregnancy. The Times of India (via inkl) concluded the claim was "false and likely came from a mix of jokes, clips taken out of context," with "no video [confirming] a pregnancy" and no confirmed girlfriend.[^toi] Complex, Hindustan Times, and AOL framed the contest / "I'm gonna be a dad" material as a viral stunt or joke.[^complex] No credible-media consensus of an actual pregnancy existed through June 2026.

Despite that, the market went through two UMA proposal/dispute cycles and finalized Yes, resolving early on May 1, 2026.[^gamma] The case drew oracle-manipulation and conflict-of-interest criticism, with reporting that 60%+ of active UMA voters hold Polymarket positions and one outlet headlining an "Oracle Manipulation Controversy."[^kucoin][^bitget]

## The allegation against Polymarket

The allegation is that UMA/Polymarket certified jokes and intent statements — not a credible announcement of an existing pregnancy — as a qualifying Yes. The statements at issue were stunt/contest material and a debunked rumor, which is precisely the "not credible, for example jokes" category the rule excludes. Critics further argued the oracle process was compromised: a large majority of active UMA voters reportedly hold Polymarket positions, creating a conflict of interest in a high-volume market, and at least one outlet framed the episode as oracle manipulation.[^kucoin][^bitget]

## Polymarket's / the resolver's defense

No direct Polymarket statement defending this specific Yes was located. The implicit defense has two parts.

First, the market ran through the full UMA dispute process — proposed, disputed, proposed, disputed — and UMA voting "determined the announcement was compliant," finalizing Yes.[^gamma][^bitget] Some crypto outlets framed the underlying event as "the streamer announced his partner is pregnant," which, if a direct qualifying statement existed, would make Yes defensible.[^bitget]

Second, the rule named "statements from Clavicular or his representatives" as the resolution source, so a direct self-announcement by the streamer could in principle satisfy it without independent media confirmation. The weakness is that the reviewed reporting describes only stunt/contest/rumor material, not a credible announcement of an existing pregnancy.

## Assessment

### Did the market finalize Yes, and is it final?

**Yes.** The gamma API shows `outcomePrices` `["1","0"]`, closed and resolved, `automaticallyResolved`, resolved early on May 1, 2026 after two dispute cycles. It is final, not in review; aggregators showing "Active" or "In Review" are stale.[^gamma]

### Did the resolving material satisfy the credibility / joke-exclusion clause?

**No, on the public record.** The only material was an April 2026 "pregnancy contest" / "I'm gonna be a dad" stunt and a viral rumor that reputable fact-checks uniformly found unconfirmed or false — the exact "not credible, for example jokes" category the rule excludes.[^toi][^complex] No credible-media consensus of an actual pregnancy existed.

### Was the oracle process credibly contested?

**Yes.** Two dispute cycles, plus reporting that 60%+ of active UMA voters hold Polymarket positions and explicit "Oracle Manipulation Controversy" framing.[^kucoin][^bitget]

### Overall classification

- **Credibility-rule violation:** Yes — Yes finalized on joke/stunt/debunked-rumor material the rule excludes.
- **Operational/oracle-process failure:** Yes — disputed twice; conflict-of-interest criticism.
- **Remediation:** None — bad Yes stands; No-holders not made whole.
- **Best public verdict: Failure (Unresolved): the credibility/joke-exclusion clause was violated, the Yes is final, and affected holders were not made whole.**

## Precise blocker to a stronger finding

The only residual gap is that the exact statement UMA voters certified as the "credible announcement" is not preserved in primary form. The uniform fact-check record (no confirmed pregnancy, no confirmed girlfriend, jokes/stunt/clips-out-of-context) makes the rule-violation judgment strong, but without the certified statement verbatim the analysis cannot fully reconstruct what voters claimed to rely on. This lowers confidence; it is not a blocker — the market is final and the credibility-rule violation is well-supported.

## Sources

[^gamma]: Polymarket gamma API, event `clavicular-pregnancy-in-2026`. Verbatim resolution rule incl. credibility and joke-exclusion clauses; `outcomePrices` `["1","0"]` (Yes); closed/resolved, `automaticallyResolved`, `closedTime`/`umaEndDate` 2026-05-01; two dispute cycles (`["proposed","disputed","proposed","disputed"]`); volume ~$13.9M. [gamma-api][gamma]

[^toi]: Times of India fact-check (inkl mirror). Concluded the pregnancy claim was "false and likely came from a mix of jokes, clips taken out of context," with no video confirming a pregnancy and no confirmed girlfriend. [Times of India / inkl][toi]

[^complex]: Complex. Framed the "pregnancy contest" / impregnation-competition material as a viral stunt; corroborates the joke/stunt nature of the underlying event (also reflected in Hindustan Times and AOL coverage). [Complex][complex]

[^kucoin]: KuCoin. Reported UMA dispute-resolution scrutiny, including that 60%+ of active UMA voters hold Polymarket positions, raising conflict-of-interest/fraud concerns. [KuCoin][kucoin]

[^bitget]: Bitget / BlockBeats. "Oracle Manipulation Controversy" framing; ~$16.46M volume; UMA voting "determined the announcement was compliant"; pro-Yes framing that the streamer announced a pregnancy. [Bitget / BlockBeats][bitget]

[gamma]: https://gamma-api.polymarket.com/events?slug=clavicular-pregnancy-in-2026
[toi]: https://www.inkl.com/news/fact-check-is-clavicular-really-expecting-his-first-child-after-10-days-relationship-amid-viral-pregnancy-contest-rumor
[complex]: https://www.complex.com/pop-culture/a/tracewilliamcowen/clavicular-male-bonnie-blue-impregnation-competition
[kucoin]: https://www.kucoin.com/news/flash/polymarket-dispute-resolution-system-under-scrutiny-as-uma-voting-raises-fraud-concerns
[bitget]: https://www.bitgetapp.com/news/detail/12560605393170
