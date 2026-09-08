---
name: eli-fintech
description: Explain fintech and financial-system behaviour simply while preserving the distinctions among money, obligations, balances, ledgers, lifecycle stages, settlement, reconciliation, risk, and controls.
---

# ELI Fintech

Apply the evidence discipline of `eli-biz` and the honest simplification of
`eli5`. Use financial-services language accurately, define it plainly, and avoid
implying that an illustrative flow is universal across products, institutions,
providers, or regions.

## Start with the business event

Identify:

- the initiating party and requested action;
- the financial instrument, account, agreement, or obligation involved;
- which party owes what to whom;
- which balances, holds, ledger entries, limits, or statuses change;
- when the change becomes final, reversible, visible, or settled;
- which controls can stop, delay, refer, reverse, or repair it.

## Default explanation

1. Give the customer-visible story in plain language.
2. Name the parties, accounts, obligations, and systems of record.
3. Separate lifecycle stages such as initiation, authorisation, posting,
   clearing, settlement, reconciliation, reversal, and dispute when applicable.
4. Show money movement separately from messages, status changes, and ledger entries.
5. Distinguish ledger balance, available balance, pending amounts, limits, and
   actual external funds where the distinction matters.
6. Explain business rules, cut-offs, calendars, thresholds, controls, and overrides.
7. Include the happy path and material timeout, duplicate, retry, reversal,
   partial-failure, and manual-repair paths.
8. State accounting, regulatory, or product assumptions and regional variation.
9. Report requirement, test, implementation, and documentation conflicts explicitly.

Do not give legal, regulatory, accounting, or financial advice. Explain the
observed system and identify where an authoritative specialist is required.

For a visual explanation, follow
[`../../shared/bento-viewgraph.md`](../../shared/bento-viewgraph.md). Prefer
separate cells for customer story, parties, money or obligation, ledger effect,
lifecycle, controls, failure paths, and simplified assumptions.

