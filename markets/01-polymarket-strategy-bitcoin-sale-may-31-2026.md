# Polymarket: Strategy sells Bitcoin by May 31, 2026

## Bottom line

**Finding: Failure. The governing rule was event-based — resolve Yes if Strategy sold any Bitcoin by 11:59 PM ET on May 31, 2026 — and Strategy's own SEC Form 8-K reports it sold 32 BTC during May 26-31, 2026, presented as of May 31 at 4:00 PM ET, inside the window. Polymarket nonetheless resolved the market No after posting a post-deadline "Additional context" note requiring that the sale be *confirmed* within the window, a requirement absent from the published rule. The same 8-K caused the event's June 30 and December 31, 2026 markets to resolve Yes. The No result is reachable only by substituting a confirmation-timing test for the rule's sale test. Confidence: high. Failure-resolved: Unresolved.**

The May 31, 2026 sub-market resolved **No**: the Gamma API reports `outcomePrices` of `["0","1"]` for outcomes `["Yes","No"]`, with `umaResolutionStatuses` of `["proposed","disputed","proposed","disputed"]` — two No proposals, both disputed, escalated to a UMA token-holder vote that finalized No.[^api] Strategy's Form 8-K, filed June 1, 2026, states it sold 32 BTC during May 26-31, 2026.[^filing] The two facts are in direct conflict with the published, event-based rule.[^api][^filing]

The conflict is not merely counterintuitive. Within the same event, the June 30, 2026 and December 31, 2026 markets — governed by identical wording — resolved **Yes** off the same disclosure (`outcomePrices` `["1","0"]`), while May 31 resolved No.[^api] The decisive difference was not whether Strategy sold Bitcoin in the window, but whether the sale was publicly confirmable before the window closed. That confirmation-timing element was introduced by a clarification posted after the deadline, not by the original rule.[^api][^galaxy][^coindesk]

## Market details

- **Venue:** Polymarket
- **Event:** `MicroStrategy sells any Bitcoin by ___ ?` (event slug `microstrategy-sell-any-bitcoin-in-2025`).[^api]
- **Disputed market:** `MicroStrategy sells any Bitcoin by May 31, 2026?` (sub-market slug `microstrategy-sells-any-bitcoin-by-may-31-2026`).[^api]
- **Condition / question IDs:** conditionId `0x3733a1b6…3239b3868`; questionID `0x0382b71b…3e68f83d`; resolvedBy `0x65070BE9…56C2f2A7`.[^api]
- **Stated deadline:** May 31, 2026 at 11:59 PM ET.[^api]
- **Governing rule (verbatim, from the May 31 sub-market `description`):** "This market will resolve to 'Yes' if MicroStrategy sells any of its Bitcoin by 11:59 PM ET on the date specified in the title. Otherwise, this market will resolve to 'No'. The primary resolution source for this market will be information from MSTR and on-chain data, however a consensus of credible reporting will also be used."[^api]
- **Final resolution:** No (`outcomePrices` `["0","1"]`); UMA statuses `["proposed","disputed","proposed","disputed"]`; closed June 4, 2026; volume ~$375.8 million.[^api]
- **Sibling markets, same wording, same 8-K:** June 30, 2026 and December 31, 2026 both resolved Yes (`["1","0"]`); March 31, 2026 resolved No.[^api]

## What happened

### May 31: the deadline passed with no public confirmation

The market's deadline was May 31 at 11:59 PM ET.[^api] As of that moment, no public source had documented a Strategy Bitcoin sale within the window, according to Polymarket's later clarification.[^galaxy][^coindesk] The absence of contemporaneous public evidence did not establish that no sale had occurred; it established only that no disclosure had yet appeared.

### June 1: Strategy disclosed an in-window sale

Strategy filed a Form 8-K on June 1, 2026 (SEC EDGAR, CIK 1050446, accession 0001193125-26-249768; report date May 30, 2026). Under Item 8.01, it states: "On June 1, 2026, Strategy Inc ('Strategy') announced an update with respect to sales made under its at-the-market offering program." The bitcoin table reports, "During Period May 26, 2026 to May 31, 2026: BTC Sold: 32; ... Average Sale Price: $77,135," and notes: "Bitcoin activity and holdings information is presented as of May 31, 2026, 4:00 p.m. Eastern Time."[^filing]

This is direct evidence from the rule's named primary source — MSTR itself — that at least one sale occurred inside the window, before the 11:59 PM ET deadline.[^filing][^api]

### June 1: Polymarket posted a confirmation requirement

After the filing became public and Yes priced up, Polymarket posted "Additional context" on the market page. Galaxy reproduces the statement and times it at approximately 1:00 PM ET: "No information from MSTR, on-chain data, or consensus of credible reporting confirmed that MicroStrategy sold Bitcoin within the market's timeframe. ... Confirmation achieved outside of the market's time frame does not qualify."[^galaxy] CoinDesk, Decrypt, and crypto.news independently reproduce the same wording and read it as making confirmation timing dispositive.[^coindesk][^decrypt][^cryptonews]

This text does not appear in the Gamma API `description` field, which still carries only the original event-based rule.[^api] The "Additional context" wording and timing are therefore established from contemporaneous secondary reporting rather than from a primary Polymarket data field.

### June 1-4: two No proposals were disputed, then No was finalized

The Gamma API record shows `umaResolutionStatuses` of `["proposed","disputed","proposed","disputed"]`: No proposed, disputed; No proposed again, disputed; then escalation to a UMA token-holder vote.[^api] Galaxy records the market going to a 48-hour final review and resolving No on the third proposal.[^galaxy] The API shows the market closed June 4, 2026 with the final No price.[^api]

## The allegation against Polymarket

The allegation is that Polymarket changed the test after the event. The original rule asks whether Strategy *sold* Bitcoin by the deadline; the post-deadline clarification asks whether a sale was *confirmed* by the deadline.[^api][^galaxy] Those tests diverge whenever a company transacts before a deadline but discloses afterward — exactly this situation.[^filing]

The strongest support is internal consistency: the event's June 30 and December 31, 2026 markets, with identical wording, resolved Yes off the same 8-K, while May 31 resolved No.[^api][^decrypt] The only variable distinguishing them is whether the sale was confirmable before each window closed. Polymarket also demonstrated, in its separately drafted announcement markets, that it knew how to make disclosure timing controlling: that wording says resolution is "based on announcements made within the market's designated time frame regardless of when the actual purchases were made."[^announcement] The sale market used no such language.

## Polymarket's defense

The reconstructed good-faith defense, drawn from the clarification and reporting, is:

1. A resolver must decide from information available at the deadline; nothing had confirmed a sale by 11:59 PM ET May 31.[^galaxy][^coindesk]
2. Allowing post-deadline disclosure to reach backward would leave expired markets unsettled indefinitely and let losing holders dispute-and-wait for later evidence, weakening deadline finality.[^coindesk]
3. Prior Polymarket disputes were reportedly resolved using only information available within the stated timeframe.[^coindesk]
4. Polymarket cannot override a finalized UMA vote, so the on-chain No result stands.[^api][^galaxy]

This is a legitimate market-design concern. It supports writing a confirmation cutoff into a contract before trading, not adding one after the event.

## Assessment

### Did Strategy sell Bitcoin within the window?

**Yes.** Strategy's Form 8-K reports 32 BTC sold during May 26-31, 2026, presented as of May 31 at 4:00 PM ET — inside the 11:59 PM ET window, sourced to MSTR, the rule's named primary source.[^filing][^api]

### Did the market resolve consistently with that fact?

**No.** The Gamma API shows the May 31 market resolved No (`outcomePrices` `["0","1"]`), contradicting both the underlying sale and the ordinary reading of the event-based rule.[^api][^filing]

### Was the clarification part of the governing rule, or added later?

**Added later.** The primary `description` field carries only the event-based rule, with no confirmation-timing requirement.[^api] The "Additional context" requiring in-window confirmation is documented by contemporaneous reporting as posted after the deadline (~1:00 PM ET June 1), and is absent from primary Polymarket data fields.[^galaxy][^coindesk][^decrypt]

### Does the cross-market pattern corroborate the substitution?

**Yes.** The June 30 and December 31, 2026 markets — identical wording, same 8-K — resolved Yes (`["1","0"]`), while May 31 resolved No.[^api] The distinguishing factor is confirmation timing relative to the window close, not whether a sale occurred — direct evidence that a confirmation test, not the sale test, drove the No result.[^api][^decrypt]

### Did the dispute process correct the problem?

**No, and it is not finally settled in substance.** The two disputes forced a UMA vote that ratified No rather than correcting it.[^api][^galaxy] The on-chain outcome is final, but the substantive question — whether the No resolution honored the published rule — remains unresolved against the primary evidence.

### Overall classification

- **Resolution-outcome failure:** Yes — the named primary source documents an in-window sale; the market resolved No.[^filing][^api]
- **Post-launch clarification failure:** Yes — a confirmation-timing requirement absent from the rule was added after the deadline and drove the outcome.[^api][^galaxy]
- **Original drafting deficiency:** Yes — delayed official reporting was foreseeable and the contract did not specify whether post-deadline evidence could prove an in-window sale.
- **Pure oracle malfunction:** Not established — UMA appears to have followed Polymarket's clarification.[^api][^galaxy]
- **Fraud or deliberate favoritism:** Not established.
- **Best public verdict:** Failure (failure-resolved: Unresolved).

## Precise blocker to a stronger finding

The decisive facts are primary-verified: the event-based rule and the No outcome from the Gamma API (`outcomePrices` `["0","1"]`, `umaResolutionStatuses`), the SEC Form 8-K reporting 32 BTC sold May 26-31, and the Yes resolutions of the June 30 and December 31 sibling markets off the same filing.[^api][^filing] The one non-primary link is the exact wording and ~1:00 PM ET timing of the "Additional context" note: it is not preserved in any primary Polymarket data field and is established from five independent secondary outlets quoting identical language.[^galaxy][^coindesk][^decrypt][^cryptonews] A live or archived capture of the market-page bulletin, or the UMA on-chain dispute log for questionID `0x0382b71b…`, would upgrade that single link from secondary to primary; neither is required to reach the Failure verdict.

## Sources

### Primary

[^api]: Polymarket Gamma API, event metadata for `microstrategy-sell-any-bitcoin-in-2025`. The May 31, 2026 sub-market (`microstrategy-sells-any-bitcoin-by-may-31-2026`) carries the verbatim event-based `description`, `outcomePrices` `["0","1"]` (Yes=0, No=1 → No), `umaResolutionStatuses` `["proposed","disputed","proposed","disputed"]`, closedTime June 4, 2026, volume ~$375.8M, conditionId `0x3733a1b6…`, questionID `0x0382b71b…`. The same event's June 30, 2026 and December 31, 2026 sub-markets show `outcomePrices` `["1","0"]` (Yes), and March 31, 2026 shows `["0","1"]` (No). [API][api]

[^filing]: Strategy Inc., Form 8-K filed June 1, 2026 (SEC EDGAR, CIK 1050446, accession 0001193125-26-249768; date of earliest event reported May 30, 2026). Item 8.01 reports an ATM-program update: "During Period May 26, 2026 to May 31, 2026: BTC Sold: 32; ... Average Sale Price: $77,135," and notes the bitcoin information is "presented as of May 31, 2026, 4:00 p.m. Eastern Time." [8-K][filing]

[^announcement]: Polymarket, event `microstrategy-announces-1000-btc-purchase-may-12-18`. Its `description` resolves Yes "based on announcements made within the market's designated time frame regardless of when the actual purchases were made" — an express disclosure-timing standard the sale market did not use. [API][announcement]

### Contemporaneous reporting and analysis

[^galaxy]: Will Owens, Galaxy Research, "Strategy Sold Bitcoin in May. Polymarket Says It Didn't," June 2026. Reproduces the original rule, the ~1:00 PM ET "Additional context" note ("Confirmation achieved outside of the market's time frame does not qualify"), the filing, the dispute chronology (two disputes, 48-hour final review, No), and characterizes the change as retroactive. Galaxy discloses a financial interest in Yes shares. [Galaxy][galaxy]

[^coindesk]: Sam Reynolds, CoinDesk, "Strategy sold bitcoin in late May, and told the market in June," June 2, 2026 (and follow-up "Polymarket says No for May, Yes for June," June 4, 2026). Independently reproduces the confirmation-based clarification and reports the May 31 contract collapsing from ~81% Yes to under 1% after the note, plus the arguments on all sides. [CoinDesk][coindesk]

[^decrypt]: Decrypt, "Strategy's Bitcoin Sale Timing Throws Polymarket Bet Into Dispute," June 2026. Quotes the "Additional context" note and reports that the June 30 and December 31 markets both resolved Yes while May 31 was disputed and resolved No. [Decrypt][decrypt]

[^cryptonews]: crypto.news, "Polymarket upholds 'No' ruling in disputed Strategy Bitcoin sale market," June 2026. Reports Polymarket added a market-page note that "confirmation achieved outside of the market's time frame does not qualify," and the final No resolution. [crypto.news][cryptonews]

[api]: https://gamma-api.polymarket.com/events?slug=microstrategy-sell-any-bitcoin-in-2025
[filing]: https://www.sec.gov/Archives/edgar/data/1050446/000119312526249768/mstr-20260530.htm
[announcement]: https://gamma-api.polymarket.com/events?slug=microstrategy-announces-1000-btc-purchase-may-12-18
[galaxy]: https://www.galaxy.com/insights/research/strategy-bitcoin-sale-polymarket-resolution-dispute-may-2026
[coindesk]: https://www.coindesk.com/markets/2026/06/04/polymarket-says-no-for-may-yes-for-june-after-strategy-s-recent-bitcoin-sale
[decrypt]: https://decrypt.co/369664/strategy-bitcoin-sale-throws-50-million-polymarket-bet-dispute
[cryptonews]: https://crypto.news/polymarket-upholds-no-ruling-in-disputed-strategy-bitcoin-sale-market/
