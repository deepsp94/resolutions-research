# Polymarket: RFK Jr. withdraws before September 2024

## Bottom line

**Finding: This was a real wording ambiguity, but not a proven Polymarket misresolution. Confidence: medium-high.**

The Polymarket dispute turned on whether Robert F. Kennedy Jr. had "withdrawn" from the 2024 presidential election before September. On August 23, 2024, Kennedy suspended his campaign, endorsed Donald Trump, and said he would try to remove his name from ballots in some battleground states. But he also remained on ballots in many states and, according to CoinDesk, the market used "withdrawal" rather than "suspension."[^coindesk][^newsweek]

That made both sides plausible:

- **Yes:** ordinary political speech often treats suspending a campaign, endorsing another candidate, and ending active campaigning as dropping out.
- **No:** a suspended campaign is not necessarily legally terminated, can continue to receive donations, and Kennedy remained on ballots in multiple states.[^coindesk][^newsweek]

The strongest finding is that the market was badly specified. It should have defined whether "withdraw" meant public suspension, ending active campaigning, FEC/legal termination, removal from all ballots, or removal from enough ballots to make victory impossible.

## Market details

- **Venue:** Polymarket
- **Question as described in reporting:** whether RFK Jr. would withdraw from the 2024 presidential election before September
- **Relevant real-world event:** Kennedy suspended his campaign and endorsed Trump on August 23, 2024
- **Dispute:** whether "withdrawal" included suspension plus endorsement
- **Resolution process:** CoinDesk reported that bettors were arguing over UMA's role in the resolution dispute.[^coindesk]

I could not recover the live Polymarket market page or full rule text during this pass. The case therefore relies mainly on CoinDesk's contemporaneous account of the market language and dispute.

## What happened

Kennedy announced on August 23, 2024 that he was suspending his presidential campaign and supporting Trump.[^coindesk][^newsweek]

Newsweek reported that Kennedy said he had made the decision to suspend his campaign and support Trump. It also reported that he would seek to remove himself or withdraw from ballots in roughly ten battleground states while still being set to appear on ballots in many other states.[^newsweek]

CoinDesk reported that Polymarket users disputed whether this counted as withdrawal for the market. It emphasized that campaigns commonly "suspend" rather than legally terminate campaigns, partly because a suspended campaign can keep receiving donations and paying debts.[^coindesk]

CoinDesk also reported that Kennedy's continued ballot presence mattered: at the time, his name was still on ballots in 23 states according to Newsweek's reporting.[^coindesk][^newsweek]

## The allegation against Polymarket

### 1. Ordinary voters would say he dropped out

Kennedy stopped actively seeking victory in the ordinary sense. He endorsed Trump and told supporters in key states not to help Kamala Harris by voting for him. Many headlines and ordinary descriptions treated the move as dropping out or ending his independent bid.

If the market was meant to track ordinary political reality, Yes had a strong claim.

### 2. "Withdraw" was not operationalized

The reported contract wording used "withdrawal" without defining what act counted.[^coindesk]

That was the core drafting failure. A presidential candidate can:

- suspend campaigning;
- endorse another candidate;
- stop fundraising for victory;
- withdraw ballot petitions in some states;
- remain on ballots in other states;
- keep an FEC committee open; and
- legally terminate the campaign later, if ever.

Those are different events. A binary market needed to choose one.

### 3. The market invited a mismatch between media shorthand and legal status

Political journalism often uses "drops out" and "suspends campaign" loosely. Election law and campaign finance treat them differently. The market appears to have depended on that distinction without making it clear to traders.

## Polymarket's defense

Polymarket does not appear in the reviewed sources to have published a detailed defense. The strongest defense is the No-side interpretation described by CoinDesk.

That defense is:

- Kennedy said he was suspending, not ending, his campaign.[^newsweek]
- Suspended campaigns are not necessarily legally terminated and can continue to receive donations.[^coindesk]
- Kennedy remained on ballots in multiple states.[^coindesk][^newsweek]
- He told supporters in noncompetitive red and blue states that they could still vote for him, according to Newsweek's account of his remarks.[^newsweek]

Under that interpretation, he had not fully withdrawn from the election before September. He had suspended active campaigning and strategically withdrawn from some ballot positions.

## Assessment

### Did Kennedy suspend active campaigning and endorse Trump before September?

**Yes.**

That is well supported by CoinDesk and Newsweek.[^coindesk][^newsweek]

### Did he fully legally withdraw from the presidential election before September?

**No, not on the available evidence.**

He remained on ballots in many states and his campaign was described as suspended rather than legally terminated.[^coindesk][^newsweek]

### Was a Yes resolution clearly required?

**No.**

Yes was reasonable under ordinary political language, but the reported wording used "withdrawal," and there were concrete facts supporting a narrower No interpretation.

### Was a No resolution clearly required?

**No.**

No was reasonable under legal/formal campaign status, but ordinary users could fairly object that the market title tracked a real-world political exit, not FEC technicalities.

### Was this a real failure for the tracker?

**Yes, as a wording failure.**

The market exposed a predictable ambiguity in political-event drafting. "Withdraw," "drop out," "suspend," "endorse another candidate," and "remain on ballot" need separate definitions.

### Overall classification

- **Operational settlement error:** Not established
- **Semantic/legal ambiguity:** Yes
- **Final outcome clearly wrong:** Not established
- **Rule-design weakness:** Yes
- **Best public verdict:** Inconclusive on final result; clear drafting failure

## Precise blocker to a stronger finding

The missing evidence is the exact Polymarket rule text, final resolution, and any UMA request/rationale. CoinDesk identifies the dispute and reports that the contract asked about "withdrawal," but the original market page is needed to determine whether the detailed rules resolved the ambiguity.

## Sources

[^coindesk]: Sam Reynolds, CoinDesk, ["Did RFK Jr. Really 'Drop Out'? Polymarket Bettors Argue Over Contract Resolution"][coindesk], August 26, 2024. Describes the Polymarket dispute, the suspension-versus-withdrawal distinction, continued ballot access, and campaign-finance implications.

[^newsweek]: Aila Slisco, Newsweek, ["Robert F. Kennedy Jr. May Still Be on the Ballot in 23 States"][newsweek], August 23, 2024. Reports Kennedy's suspension, support for Trump, planned ballot withdrawals in some states, and continued ballot presence in many states.

[coindesk]: https://www.coindesk.com/markets/2024/08/26/did-rfk-jr-really-drop-out-polymarket-bettors-argue-over-contract-resolution
[newsweek]: https://www.newsweek.com/robert-f-kennedy-jr-may-still-ballot-23-states-1943742
