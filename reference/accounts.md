# The three accounts

Every student group has up to three accounts. **Which account pays for a purchase is asked on every
Financial Transaction Form**, so know the answer before you file.

| | **Operating** | **Fundraising** | **Gift** |
|---|---|---|---|
| Funded by | SU: budget allocation, flat funding, appeals | Your sales, ticket revenue, sponsorships | Donations via University Advancement |
| Deposited | **Automatically** when awarded — no action needed | You deposit what you collect | Routed by Advancement |
| Rollover | ❌ **Resets to $0 at fiscal year end** | ✅ Carries over | ✅ Carries over |
| Spending rules | Full SU restrictions and caps apply | SU restrictions on accounts still apply | SU restrictions on accounts still apply |

## Operating account — the SU money

Funds land here automatically whenever Treasury or the VP of Finance awards you anything. You don't file
anything to receive them.

**Different awards have different lifespans inside the account:**

| Award type | Lifespan |
|---|---|
| Budget allocation — **overhead** | Available all school year (or until spent) |
| Budget allocation — **event** | **That specific event only**; closes out once the event's expenses process |
| **Flat funding** | Available any time, all school year (or until spent) |
| **Appeal** | **That specific request only**; closes out once its expenses process |

**End-of-year reset:** operating funds are use-it-or-lose-it. Anything left at fiscal year end goes to
zero — it does not roll over.

> 🟢 **The Operating account may not carry a negative balance.** It cannot go below $0. Combined with
> "approval before spending," this means you cannot front a purchase against expected funds.

**Only these three accounts.** Student groups may use **only** the Operating, Fundraising, and Gift accounts
within Workday. No outside bank accounts, personal checking accounts, or Venmo — all financial activity must
stay in the three official accounts.

**But "use it or lose it" is not permission to waste it.** Funds must be used for their originally
intended purpose in support of the group's mission. Don't dump leftover money into random last-minute
purchases. If you have room left, contact Business Operations — they will help you pivot the funds to
meaningful, approved activity before the year closes.

## Fundraising account

Carries over year to year by design, so you can build toward long-term goals. Two ways to fill it:
product/event sales and sponsorships — see [fundraising-and-gifts.md](fundraising-and-gifts.md).

Also receives your **20% share of revenue** from SU-funded events (the other 80% returns to SU), plus any
overage where SU's 80% would exceed its principal allocation.

## Gift account

For genuine donations — money given with **no tangible benefit expected in return**. That's the line
between a gift and a sponsorship. Carries over between fiscal years, so it can accumulate as savings.

## Getting money in — approved methods only

For **all** accounts, incoming funds must be collected via **Cash, Check, or Credit Card (Cashnet)**.
Those are the only university-approved payment methods for student organizations. Do not collect through
personal payment apps.

Gifts are the exception in routing: they go through **University Advancement**, not your own collection —
see [fundraising-and-gifts.md](fundraising-and-gifts.md).

### File an FTF *before* you start collecting

Submit a **Financial Transaction Form (fundraising request)** before your group collects any funds, so your
Business Coordinator can review and approve the process in advance.

### ⏰ Deposit deadlines

| Collection type | Deposit within |
|---|---|
| **For an event** | **7 days of the event** taking place |
| **Non-event** (dues, merch sales) | **7 days of collecting** the money |

Sitting on cash risks losing it and makes your balances wrong.

### Cash and check drop-off

- **Where:** reception desk, **second floor of the Campus Life Suite, DUC Room 270**
- **When:** Monday–Friday, **8:30 am – 5:00 pm**
- **Who:** the Administrative Coordinator, **Jordan**, records the funds and hands you a **receipt for your
  records**. Your Business Coordinator then processes the deposit into the right account.

**Checks** should be made payable to **Washington University**, with your **student group's name on the memo
line** (e.g. "Washington University – Troll Club").

**Mailing address for checks:**

```
Washington University in St. Louis
1 Brookings Drive, MSC 1128-226-270
St. Louis, MO 63130
```

### Cashnet (collecting by credit card)

1. Submit the FTF and **attach the Cashnet Application** (on the BEARings board).
2. Your Business Coordinator reviews and approves.
3. The team works with Accounting to set up your link; **Accounting contacts you directly** to finalize
   details and launch your custom payment link.

Two things to plan for:

- **Cashnet is for purchases and sales, not donations.** Donations go through the Gift department
  (gifts.wustl.edu) so donors get proper tax credit.
- **~3% credit card processing fee.** Net sales are deposited shortly after payment; the **fees appear in
  your account the following month** — so budget for them and don't be surprised by next month's line.

### Which account do collected funds go into?

- **Operating** — if you're collecting to help cover an event/project **funded by an SU allocation** (ticket
  sales, participation fees, member dues for that specific event). Keeping it with the allocation makes
  vendor payment and expense tracking work.
- **Fundraising** — if you did **not** receive an allocation for it.

This also applies to **co-sponsorship money** collected toward an SU-allocated project: it goes to Operating.

## Checking your balance

- Balances for all accounts are updated **every weekday (Mon–Fri)** in the **Daily Report** — Excel files
  attached to the account-balance cards on the BEARings board.
- Check it **before** submitting any spending request or planning a large purchase.

Fastest way to read it:

```bash
python tools/su_board.py report operating --group "<your group name>"
```

Doing it by hand: open the spreadsheet, filter the **Group** column to your group, filter **Event** to the
specific event/budget, and scroll to the bottom for the remaining balance. Two things to know — **negative
amounts are money *into* your account**, and each award also appears against the SU "Budgets/Appeals"
source project, so filter to your own `PJ…` number or the totals cancel out. See
[trello-board.md](trello-board.md).

> ⚠️ **The report overstates what you have.** Unreconciled credit card purchases and unapproved
> reimbursements do **not** appear on it. Keep your own ledger (`orgs/<slug>/budget/ledger.csv`) and
> reconcile.

## If a group disbands

Leftover **Fundraising** (and Gift) money stays on campus: it transfers to a general Office of Student
Success account, and the Vice Chancellor for Student Success reallocates it to other student programs,
campus events, and active clubs.
