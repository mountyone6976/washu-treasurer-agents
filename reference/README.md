# WashU SU Finance reference

Shared, org-agnostic knowledge about how student org finance actually works at WashU. Every org using
this template reads from here. **Nothing org-specific goes in this folder** — that belongs in `orgs/<slug>/`.

## Source and currency

Compiled from official WashU Student Union materials:

- **SU Finance BEARings 2026–2027** Trello reference board (exported 2026-07-14)
- **Financial Transaction Form (FTF) Flow Chart** (official field map)
- **Business Operations Spending Training** video (SU Business Operations)

> ✅ **FY27 policies are live** (verified against the board **2026-09-04**).
> [financial-policies.md](financial-policies.md) now carries the FY27 caps, not FY26.
>
> ⚠️ **But two FY27 sources disagree.** The **Financial Policies** card (Treasury-approved, governs
> **appeals this year**) and the **FY27 BAM** (written spring 2026, governs what the **annual budget round**
> was allocated against) give different numbers for the travel cap, flights, gas, conferences, and socials.
> Both are live. Every affected file carries a conflict callout. Confirm which applies before relying on a
> figure: **finance@su.wustl.edu** for policy/appeals, **budget@su.wustl.edu** for the annual budget.

## Files

| File | Contents |
|---|---|
| [su-finance-overview.md](su-finance-overview.md) | How the whole system fits together; start here |
| [trello-board.md](trello-board.md) | **Reading the live BEARings board and its spreadsheets** — no login required |
| [treasurer-role.md](treasurer-role.md) | Your duties, expectations, credit card hours, communication norms, advisor boundaries |
| [contacts-su.md](contacts-su.md) | SU Financial Leadership + Business Operations team, and who to ask what |
| [categories.md](categories.md) | Category I / II / III — what each can and can't get |
| [accounts.md](accounts.md) | Operating vs. Fundraising vs. Gift accounts; lifespans and rollover |
| [funding-sources.md](funding-sources.md) | Budget allocation, flat funding, appeals — where money comes from |
| [annual-budget.md](annual-budget.md) | The spring annual budgeting cycle (BAM, BAT, WUGO submission) |
| [appeals.md](appeals.md) | Rolling appeals: WUGO submission, the $1K split, 3/4-week deadlines, turnaround |
| [financial-policies.md](financial-policies.md) | FY27 caps: socials, honoraria, travel, retreats, conferences, revenue, etc. |
| [restrictions.md](restrictions.md) | Funding principles and what SU will not pay for |
| [spending-methods.md](spending-methods.md) | Credit card, Workday reimbursement, supplier payment |
| [travel.md](travel.md) | Travel caps, rental cars, canceled flights, conferences, retreats |
| [ftf.md](ftf.md) | Financial Transaction Form: when required, and every field by transaction type |
| [fundraising-and-gifts.md](fundraising-and-gifts.md) | Fundraising, sponsorships, gifts, Cashnet, revenue split |
| [campus-life.md](campus-life.md) | The non-money approvals: WUGO event registration, advisor, travel |
| [su-resources.md](su-resources.md) | Free resources to use before spending money |
| [calendar.md](calendar.md) | The treasurer year: recurring deadlines in order |
| [glossary.md](glossary.md) | WUGO, Workday, Cashnet, BAM, BAT, FTF, SAF, DUC, and the rest |

## Keeping this current

The board is public and machine-readable, so verifying any claim here costs one command:

```bash
python tools/su_board.py card "Restrictions"
```

When the board and this folder disagree, **the board wins** — fix the file here and contribute it back,
since every org using the template reads it. See [trello-board.md](trello-board.md) for the traps that
produce wrong answers: archived lists, checklist-only content, double-entry reports, inverted signs.
