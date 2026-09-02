# Setup — adopting this template for your org

## 1. Get the repo

Fork it on GitHub, **keeping your fork private** (you'll be putting real financial data in it), then clone:

```bash
git clone https://github.com/<your-username>/washu-treasurer-agents-template.git
```

## 2. Create your org folder

```bash
cp -r orgs/_template orgs/<your-org-slug>
```

Short lowercase slug — `aiche`, `wubs`.

## 3. Point the repo at your org

```bash
echo <your-org-slug> > orgs/ACTIVE_ORG
```

## 4. Fill in your org's data

In priority order — the agents degrade gracefully but can't do much without the first three:

1. **`org.md`** — most importantly your **SU category** (only Cat I can appeal or submit budgets), your
   **group type** (determines your Business Coordinator), **active member count** (drives flat funding), and
   your **project number** (needed for every Workday expense report).
2. **`contacts.md`** — your Business Coordinator, your Campus Life Advisor, and **who in the group is a
   student employee**. That last one is the reimbursement bottleneck: only student employees can file Workday
   expense reports. Find out before you need it.
3. **`budget/allocation.md`** — what SU awarded you, per line, per account.
4. **`budget/ledger.csv`** — transactions as they happen. Start now; retroactive reconstruction is miserable.
5. **`appeals/`** — one file per appeal, **including denials and their rationale**.
6. **`training/`** — your own notes.

### Getting your numbers

Balances live in the **Daily Report** — Excel files attached to the account-balance cards on the BEARings
Trello board, one per account. Filter the **Group** column to your group, then the **Event** column to a
specific event, and scroll to the bottom for the remaining balance.

Copy those allocations into `allocation.md`. But **keep your own ledger too**: unreconciled credit card
purchases and unapproved reimbursements don't appear on the report, so it overstates what you have.

## 5. Check the shared reference layer

`reference/` is compiled from the official SU materials, but two things go stale:

- **`financial-policies.md` holds FY27 caps** (verified against the board 2026-09-04). New policies drop in
  the **second week of the fall semester** — update that file when the next fiscal year's land.
- **Names in `contacts-su.md`** turn over annually. The role addresses (`finance@`, `treasury@`, `budget@`,
  `activities@`) don't.

Fixes to `reference/` help every org using the template — contribute them upstream rather than keeping them
in your fork.

## 6. Use it

Open the repo in Claude Code and ask in plain language. The right agent picks it up, or name one directly.

Things worth asking early in the year:

- *"What deadlines am I on the hook for this semester?"*
- *"Walk me through buying X"* — produces a ready-to-file FTF
- *"Can we afford the banquet, and is it even fundable?"*
- *"Someone paid out of pocket three days ago — what now?"*
- *"Draft an appeal for the speaker event"*

And near the end of the year: *"write the treasurer handoff doc."* Operating funds reset to $0 at fiscal year
end, and the next treasurer inherits nothing but what you wrote down.

## What not to commit

Already gitignored, but worth understanding:

- **Receipts, bank/account statements, scanned forms** (PDFs, images, spreadsheets under `orgs/`)
- **Anything with account numbers, card numbers, SSNs, or Workday/WUGO credentials** — including in handoff
  docs. Describe *where* access lives and who to ask.
- **The Canvas course videos, slide decks, and Trello export PDF** — WashU's material. Extract the facts you
  need into `reference/`; leave the source documents on your own disk.
