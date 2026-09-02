# WashU Student Org Treasurer — Agent System

A [Claude Code](https://claude.com/claude-code) template that automates the recurring work of being a
student org treasurer at Washington University in St. Louis: Financial Transaction Forms, rolling appeals,
Workday reimbursements, the annual budget cycle, fundraising requests, balance tracking, and the
correspondence around all of it.

Built from the official SU materials — the **SU Finance BEARings** Trello reference board, the **Financial
Transaction Form flow chart**, and the **Business Operations Spending Training** — so the agents work from
what SU actually requires rather than generic finance advice.

## Three layers, so it's shareable

```
.claude/agents/     CORE. Nine generic treasurer agents. Org-agnostic — no group names, figures, or
                    contacts baked in. This is what other treasurers reuse untouched.
reference/          SHARED. How WashU SU finance works: caps, deadlines, forms, routing, restrictions.
                    Applies to every org. Fixes here help everyone.
orgs/<your-org>/    YOURS. Category, allocation, ledger, appeal history, e-board contacts. Private.
```

Agents resolve the active org at run time from [`orgs/ACTIVE_ORG`](orgs/ACTIVE_ORG) — they never contain
org-specific data. That's what lets someone else fork this, drop in their own `orgs/<slug>/`, and never touch
the core.

## Agents

| Agent | Use for |
|---|---|
| [compliance-agent](.claude/agents/compliance-agent.md) | **Start here for anything new.** Is this fundable, in-cap, from the right account, correctly sequenced? |
| [spending-agent](.claude/agents/spending-agent.md) | Purchases → the right method → a filled-out FTF (all six transaction types) |
| [reimbursement-agent](.claude/agents/reimbursement-agent.md) | Workday expense reports, the 7-day clock, receipt validation, the student-employee requirement |
| [appeals-agent](.claude/agents/appeals-agent.md) | Rolling appeals: eligibility, the $1K routing split, lead-time caps, justifications that land |
| [budget-agent](.claude/agents/budget-agent.md) | The spring annual budget cycle — three events + overhead, BAM limits, WUGO filing |
| [fundraising-agent](.claude/agents/fundraising-agent.md) | Collecting money, Cashnet, the 7-day deposit rule, the 80/20 revenue split, sponsorship pre-approval |
| [ledger-agent](.claude/agents/ledger-agent.md) | What you *actually* have vs. what the Daily Report says; reports and treasurer handoff |
| [communications-agent](.claude/agents/communications-agent.md) | Drafting email and routing it to the right person out of ~8 possibilities |
| [board-agent](.claude/agents/board-agent.md) | Reading the **live** BEARings Trello board and pulling the daily balance spreadsheets |

## Live board access

The SU Finance BEARings Trello board is **public** — no login, no API key. [`tools/su_board.py`](tools/su_board.py)
reads it with the standard library alone, so it works anywhere including a phone session:

```bash
python tools/su_board.py report operating --group "<YourGroupName>"
```

That finds the newest daily report, downloads it, filters to your group, and totals by event. Also
`sync`, `lists`, `cards`, `card`, `search`, `files`, `get`, `xlsx`. See
[reference/trello-board.md](reference/trello-board.md).

## A few things the agents know that cost treasurers money

- **The SU Daily Report overstates your balance** — unreconciled card purchases and unapproved
  reimbursements don't appear on it. Hence the local ledger.
- **Travel appeal caps depend on filing 4+ weeks out.** Hotels $200 vs. $150/night, flights $400 vs. $300.
  Filing a few days earlier is worth hundreds.
- **Cultural, DEI, and affinity groups may have their group-wide socials and formals treated as
  mission-related**, exempting them from the social cap entirely. Worth arguing rather than accepting.
- **Reimbursements need a student employee** to file the Workday report — though not necessarily the person
  who paid.
- **You can now spend before WUGO approval — but if the event is denied you must repay, and your group is
  blocked from all further spending until you do.**
- **Almost every deadline is 7 days**: reimbursement after purchase, supplier FTF after delivery, deposits
  after an event.

## Using this for your own org

1. Fork this repo. **Keep your fork private** — `orgs/<slug>/` holds real financial data.
2. `cp -r orgs/_template orgs/<your-slug>` and fill it in.
3. `echo <your-slug> > orgs/ACTIVE_ORG`
4. Open in Claude Code and ask in plain language — "can we afford the banquet?", "draft an appeal for the
   speaker", "someone paid out of pocket, what now?"

Full walkthrough in [docs/SETUP.md](docs/SETUP.md).

Leave `.claude/agents/` and `reference/` alone unless something is wrong **for everyone** (a cap changed, a
deadline moved) — then fix it and contribute it back, since every org reads those.

## Caveats worth reading

- **`reference/financial-policies.md` holds the FY27 caps** (verified 2026-09-04 — FY27 policies are now
  published). Two live FY27 sources disagree, though: the Treasury-approved **Financial Policies** card
  governs appeals this year, while the **FY27 BAM** is what the spring 2026 budget round was allocated
  against. Where a number is material, confirm which document applies — finance@su.wustl.edu for policy and
  appeals, budget@su.wustl.edu for the annual budget.
- **The BEARings Trello board is the authoritative policy manual**, and it changes during the year. This repo
  is a compiled snapshot for speed. When it matters, check the board.
- **These agents draft and organize. They do not submit forms, send email, or move money.** You review and
  file everything yourself.
- Source PDFs, slide decks, receipts, and statements are gitignored under `orgs/` on purpose — extract facts,
  don't commit documents.
