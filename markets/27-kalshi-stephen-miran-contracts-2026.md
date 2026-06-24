# Kalshi: Stephen Miran confirmation-vote contracts

## Bottom line

**Finding: No failure. The seed ("Stephen Miran contracts") resolves to a real, correctly settled Kalshi market — per-senator contracts on Miran's Federal Reserve confirmation vote — and the alleged 2026 misresolution with a CFTC complaint cannot be located in any public record. Confidence: High.**

The seed alleged a contested Miran misresolution "acknowledged by Kalshi support but unresolved publicly," but supplied no ticker, date, disputed strike, complaint number, or article. The market it points to (Kalshi series `KXCONFFEDGOV`) settled cleanly on Senate Roll Call Vote 519, 48-47, with each senator strike graded to the official roll call.[^series][^rollcall] No public record ties any Miran market to a contested misgrade.[^seed]

## Market details

- **Venue:** Kalshi
- **Series:** `KXCONFFEDGOV` — "Fed Governor Confirmation"[^series]
- **Event:** `KXCONFFEDGOV-25` — "Which Senators will vote to confirm Stephen Miran before Sept 15, 2025?"
- **Contract type:** `BILLVOTE` (per-senator Yes/No strikes)[^series][^billvote]
- **Settlement source:** Library of Congress / congress.gov[^series]
- **Governing CFTC self-certification:** `BILLVOTE`, filed May 23, 2025[^cert]
- **Settlement event:** Senate Roll Call Vote 519, Sept 15, 2025, 48-47, "Nomination Confirmed"[^rollcall]

## What happened

On September 15, 2025, the Senate voted 48-47 to confirm Stephen Miran of New York to the Federal Reserve Board of Governors (Roll Call Vote 519, 7:19 PM).[^rollcall] He was reported confirmed and expected to join the Fed's rate-setting committee meeting the following Tuesday, around September 16.[^ab] Republican Senator Lisa Murkowski broke ranks to vote against him.[^ab]

Kalshi's `KXCONFFEDGOV` series listed a per-senator strike for the confirmation. Under the `BILLVOTE` terms, each strike resolves on whether that senator "voted Yea on first final vote of `<bill>` (not a motion to proceed or motion to invoke cloture)."[^billvote] The market settled to Roll Call 519, with each senator strike resolved to that senator's individual recorded vote.[^series][^rollcall] No strike is shown misgraded against the roll call.

## The allegation

The seed claimed there were "Stephen Miran contracts" in 2026, that a trader reported a misresolution, that Kalshi support acknowledged it, and that a CFTC complaint was filed but went unresolved publicly.[^seed] The seed gave no market title, ticker, date, disputed fact, final result, complaint link, or support message.

## Assessment

### Does the seed point to a real, identifiable market?

**Yes.** "Stephen Miran contracts" maps unambiguously to Kalshi series `KXCONFFEDGOV`, event `KXCONFFEDGOV-25`, the per-senator confirmation-vote contracts.[^series]

### Was that market correctly resolved?

**Yes, on the available record.** Settlement tracks Senate Roll Call 519 (48-47, "Nomination Confirmed").[^rollcall] The `BILLVOTE` rules are explicit and mechanical: a Yea on the first final vote resolves Yes; absence, abstention, or a recorded "present" vote resolves No; and post-vote requests to "add, remove, or alter a vote shall not be considered... regardless of any change to the official vote tally."[^billvote] No senator strike is shown misgraded against the official tally.

### Does the alleged 2026 misresolution / CFTC complaint exist in the public record?

**No.** No ticker, date, disputed strike, complaint number, lawsuit, Reddit/X outcry, or news article ties any Miran market to a contested misgrade.[^seed] Every locatable Kalshi resolution dispute is a *different* market (Khamenei death-carveout, Cardi B Super Bowl, 2025 Oscars, UFC, X-CEO/Yaccarino) — none about Miran.

### Overall classification

- **Market existence:** Verified (`KXCONFFEDGOV-25`)
- **Resolution error:** None established
- **Evidence for the alleged 2026 dispute:** None located
- **Best public verdict:** No failure. The market is correctly identified and correctly settled; the alleged misresolution is unsourced and unlocatable.

## Precise blocker to a stronger finding

The seed's alleged CFTC complaint cannot be matched to any record — no ticker, date, disputed strike, complaint number, or public post exists to test. Because nothing identifies a specific contested Miran contract, no failure can be established. (A prior draft mentioned a "Sept 10 clarification + full refund" self-correction; this could not be independently corroborated and is omitted — it does not affect the verdict.) If a specific contested Miran market or ticker were produced, the case could be re-evaluated.

## Sources

[^seed]: Grok seed in `initial_research.md` names "Stephen Miran contracts" and a 2026 misresolution/CFTC complaint, but identifies no contract, disputed outcome, or source. [`initial_research.md`][seed]
[^series]: Kalshi series API — title "Fed Governor Confirmation," settlement source Library of Congress / congress.gov, contract type `BILLVOTE`. [Kalshi `KXCONFFEDGOV` API][series]
[^billvote]: Kalshi `BILLVOTE` contract terms — Yea on "first final vote... (not a motion to proceed or motion to invoke cloture)" resolves Yes; "absence, abstention, or a recorded 'present' vote" resolves No; post-vote requests to "add, remove, or alter a vote shall not be considered... regardless of any change to the official vote tally." [Kalshi BILLVOTE terms (PDF)][billvote]
[^cert]: Governing `BILLVOTE` CFTC product self-certification, filed May 23, 2025. [CFTC filing (PDF)][cert]
[^rollcall]: U.S. Senate Roll Call Vote 519, Sept 15, 2025, 7:19 PM — 48 Yea, 47 Nay, 5 Not Voting; Stephen Miran of New York to the Federal Reserve Board of Governors; "Nomination Confirmed." [Senate Roll Call 519][rollcall]
[^ab]: American Banker — Miran confirmed to Fed board 48-47; Murkowski voted no; expected to join the Fed rate-setting meeting the following Tuesday (~Sept 16, 2025). [American Banker][ab]

[seed]: ../archive/initial_research.md
[series]: https://api.elections.kalshi.com/trade-api/v2/series/KXCONFFEDGOV
[billvote]: https://kalshi-public-docs.s3.amazonaws.com/contract_terms/BILLVOTE.pdf
[cert]: https://www.cftc.gov/filings/ptc/ptc05232522141.pdf
[rollcall]: https://www.senate.gov/legislative/LIS/roll_call_votes/vote1191/vote_119_1_00519.htm
[ab]: https://www.americanbanker.com/news/stephen-miran-confirmed-to-fed-board
