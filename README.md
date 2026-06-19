# Resolution Failures Research

This repo tracks prediction-market cases where a venue may have made a real mistake in resolution, rules, source selection, live clarifications, or implementation.

The goal is to determine conclusively, with sources, whether a failure actually happened. If the answer is not conclusive, the case should explain exactly why.

## Start Here

Begin with [`case_verdict_table.md`](case_verdict_table.md).

That table is the top-level index. It lists each case, the current verdict, the short reason, and the remaining blockers. Treat it as an overview.

## Case Files

The detailed case studies are in [`markets/`](markets/).

Each file should cover roughly the following surface area:

- what the allegation is
- what the platform's strongest defense is
- what the sources show
- whether the case is a failure, no failure, or inconclusive
- what evidence is still missing, if any

The case files are the source of truth. The verdict table should summarize them.

## Research Standard

For each case, try to answer:

1. Did a real failure occur?
2. What exactly was the failure?
3. What sources support that conclusion?
4. What is the strongest argument on the other side?
5. If the case is inconclusive, what is the blocker?

Do not give platforms the benefit of the doubt by default. Also do not mark a case as a failure unless the sources support it. If the evidence is incomplete, say that clearly.

## Collaborating

Open a pull request if you have sourced corrections, stronger primary sources, missing market rules, better wording, or a challenge to a verdict.
