# Codex Goal: Review Case Files for Prediction-Market Resolution and Rules Failures

## Goal Text

Review every case-by-case Markdown file under `markets/` to determine, as conclusively as the evidence allows, whether the relevant prediction-market platform committed a failure or mistake. The ultimate purpose is to produce website-ready research that explains, with sources, whether a failure occurred, what kind of failure it was, and why the conclusion is warranted.

The review is not limited to final payout errors. A platform failure may include, among other things:

- a wrong final resolution;
- an UMA/oracle/process failure;
- manipulation or breakdown of the dispute process;
- unclear, misleading, or internally inconsistent market rules;
- a title/rules mismatch, while recognizing that a title cannot capture every nuance and the issue is whether the presentation materially misled users;
- a source-rule or timing-rule problem;
- an operational grading or execution mistake;
- a post-launch clarification or "additional context" that contradicted, narrowed, or materially changed the initially published rules;
- a transparency failure, including failure to explain a resolution, source set, refund, remediation, or override.

For each file, verify the existing writeup against the underlying sources. Do not rely on the prior agent's summaries, the seed allegations, or the platform's characterization without checking the evidence. Use primary sources, contemporaneous reporting, official market pages/API records, on-chain or UMA records, archived pages, and Exa where normal browsing is blocked or insufficient.

Do not unconsciously sympathize with Polymarket, Kalshi, UMA, or any other resolver. Do not give the venue the benefit of the doubt merely because a rule can be read in its favor after the fact. A platform's rule ambiguity, poor drafting, late clarification, opaque source standard, or failure to preserve/communicate decisive evidence can itself be the failure. At the same time, do not assume every allegation is true; if the evidence does not prove a failure, say that clearly and explain the blocker.

Each reviewed case file should make the strongest sourced argument against the platform and the strongest sourced platform defense, then evaluate both. Platform defenses can be explicit public statements, contract text, market rules, source hierarchy, UMA procedure, remediation actions, or the strongest implicit defense available from the record. The defense should be tested rather than accepted.

The goal is complete when every `markets/*.md` file has been reviewed and, where necessary, edited so that the file gives a source-grounded answer to the core question: did the platform fail, in what way, and how conclusively can we know? If the answer cannot be conclusive, the file should explain the precise evidentiary or conceptual blocker. The reviewer should use whatever reasoning structure fits the specific case, while avoiding unsupported claims, platform-friendly assumptions, and overconfident conclusions from weak evidence.
