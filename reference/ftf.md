# Financial Transaction Form (FTF)

The workhorse form. A Google Form, found on the **first card of the FORMS (turquoise) column** on the SU
Finance BEARings Trello board.

> **An FTF is required for most financial transactions. Reimbursements are the only exception** — those go
> through a Workday expense report instead (see [spending-methods.md](spending-methods.md)).

The form uses **conditional logic**: your answers on each page determine which pages you see next. So the
field lists below are per transaction type, not all at once.

## Two form links are in circulation — pick by transaction type

Verified across every open card and checklist on 2026-09-04:

| Link | Where the board uses it | Use for |
|---|---|---|
| [`forms.gle/gdFf8bBmXWKJ8nmd6`](https://forms.gle/gdFf8bBmXWKJ8nmd6) | The **Financial Transaction Form** card (the canonical one), the **Reallocations** card, and the deposit/Cashnet checklists | Card purchases, reallocations, fundraising requests, deposits, canceled-event retrieval |
| [`forms.gle/PqKykXFXBh15Skrw7`](https://forms.gle/PqKykXFXBh15Skrw7) | The **"Non-Credit Card Payments (Electronic Payment/Check)"** checklist on the *Spending from your Operating / Fundraising / Gift Account* cards — all three, consistently | **Supplier payments** by check or ACH |

> The FORMS card presents the first link as the single FTF covering all six transaction types, but the
> current spending cards consistently route **supplier/invoice payments** to the second one. Both are live.
> If you're filing a supplier payment, ask your Business Coordinator which to use rather than guessing —
> a form filed in the wrong place is a lost week.

> ⚠️ **The live form is SSO-gated.** An unauthenticated fetch returns a Google sign-in wall, so the field
> lists below **cannot be verified programmatically** — they were captured by a treasurer working through
> the real form. If you hit a field that isn't documented here, add it.

## Timing — file before you shop

- **Card purchases: submit the FTF at least one day before you buy. Same-day card purchases are not
  allowed.**
- You do **not** need to wait for a Business Coordinator's approval email before coming to the office.
- **Supplier payments:** file within **7 days** of whichever comes *first* — service completed, items
  received, or the invoice landing in your inbox. No approval email needed here either.

## The six transaction types

| Type | Use for |
|---|---|
| **Non-travel WashU credit card** | Goods/services bought online, by phone in the SU office, or locally with a checked-out physical card |
| **Travel WashU credit card** | Airfare, ground transportation, lodging, registration |
| **Non-credit-card payment (electronic payment / check)** | Supplier/vendor invoices where the vendor can't take a card |
| **Fundraising request** | Ticket sales, dues, subsidizing a purchase, restaurant fundraisers, selling food/services, merch, sponsorships, co-sponsorships, event fees. (*"Concessions"* appears **0 times** on the live board — treat it as unverified) |
| **Reallocation request** | Using already-allocated funds for a different purpose or item |
| **Canceled event retrieval** | Telling staff you're canceling so unneeded funds can be retrieved and reused for appeals |

**Fundraising requests are not solicitations of gifts or donations** — donations go through Advancement
(see [fundraising-and-gifts.md](fundraising-and-gifts.md)).

## Page 1 — always collected, regardless of type

- Email
- Acknowledgement statement
- Student group name
- Treasurer name(s)
- Business Coordinator
- **Which transaction type** you're making

> **Purchaser field:** if someone other than the treasurer will come in to make the purchase, the treasurer
> files the FTF **in advance** and lists that person as the purchaser.

> **No WUGO questions this year.** The FTF no longer asks about WUGO registration. That does **not** mean
> registration is optional — see the repayment rule in [campus-life.md](campus-life.md).

---

## Fields by transaction type

### Non-travel purchase

Exact fields, in order, as they appear on the live Google Form (confirmed 2026-09-04):

1. **Is this an overhead purchase?** *(required)*
2. **Location of the Event** *(required)*
3. **Date of the Event** *(required, date picker)*
4. **Which account will be used to cover this expense?** *(required — Operating / Fundraising / Gift)*
5. **What items are you purchasing** *(required)*
6. **What is the intended use of the items? How does this item tie into your event, be specific.**
   *(required)*
7. **List the Stores for Each Purchase** *(required)*
8. **Please upload any additional attachments that will facilitate this purchase** *(optional — up to 10
   files, max 10 GB per file)*

> The live form does **not** currently ask for a budget name, whether you're using flat funding, or
> attendee names for events under 13 people — despite those being listed here previously. Know your budget
> name and line item anyway (per the standing checklist below); staff evidently derive it from the account
> selection and event/purchase description rather than a dedicated field. Flag it with your Business
> Coordinator if a purchase's funding source is ambiguous (e.g. flat-funding top-ups).

---

### Travel purchase

**Event information**
- Travel city
- Travel state
- Departure date
- Return date
- **Upload your roster for this trip**
- Will the group include a **coach, graduate students, or individuals not listed on your WUGO roster**? If
  so, provide their **names and titles**

**Purchase information**
- Which account covers this expense — Operating funds (budget) / Fundraising / Gift?
- What is the **budget name** the expense will be pulled from?
- **Type of purchase:** airfare, hotels, transportation, registration
- List the **company/organization name** for each purchase
- **Confirm the number of:** rooms, flights, rental cars, registrations

**Documents**
- Any additional attachments that will facilitate the purchase

> Travel has its own caps, and they get tighter inside 4 weeks — see
> [financial-policies.md](financial-policies.md) before filing.

---

### Supplier invoice request (electronic payment / check)

**Purchase information**
- Is this an overhead purchase?
- Which account covers this expense — Operating funds (budget) / Fundraising / Gift?
- What is the **budget name** the expense will be pulled from?
- What are you purchasing, and what is the intended use of the items?
- List the **stores** for each purchase
- Are you using **flat funding**?

**Vendor / supplier information**
- Vendor name
- Vendor contact name
- Vendor phone number
- Vendor email
- **Did you provide the vendor with your Business Coordinator's contact information?**

**Documents**
- **Invoice**
- **W-9**
- **ACH electronic payment form**
- Any additional attachments

> Get the contract signed via your Campus Life Advisor **first**, and check that W-9/ACH signatures are
> real or DocuSign — **no typed cursive fonts**. File within **7 days** of goods received / service provided.

---

### Fundraising request

**Purpose information** — what is the purpose of collecting money?
- Ticket sales
- Subsidize a purchase or event
- Restaurant fundraiser
- Selling items or services
- Other — provide a description

**Collection / deposit information**
- **Into which account will the collected funds be deposited?**
  - **Operating** — if you received an allocation from SU
  - **Fundraising** — if you did **not** receive an allocation
- When will you **start and stop** collecting money?
- What **method** are you using to collect? **Cash, check, Cashnet**

**Documents**
- **Cashnet application**, if applicable

> All collected money must be deposited **within 7 days following the event**.

---

### Reallocation

Exact fields, in order, as they appear on the live Google Form (confirmed 2026-09-04):

1. **Event Name (Allocate FROM)** *(required)*
2. **Line Item Name (Allocate FROM)** *(required)*
3. **Event Name (Allocate TO)** *(required)*
4. **Line Item Name (Allocate TO)** *(optional, free text — if the line doesn't exist yet under that event,
   type the new line's name here; there's no separate "new line item" field on the live form)*
5. **Requested Amount To Be Reallocated** *(required)*
6. **Reason for the reallocation. Why are these funds going unspent, and why are you attempting to use
   them in this way?** *(required)*
7. **How did you arrive at the above amount? Please provide itemization where necessary** *(required)*
8. **Please upload any documentation to confirm your amount** (ex. screenshot of hotel listing, invoice,
   etc.) *(optional — up to 5 files, max 10 GB per file)*

> **Minor** reallocations (between lines of the *same* event) are handled by Business Operations staff at
> spending time. **Anything else** — notably between *different* events — goes through this form and is
> decided by the **VP of Finance**.

---

### Canceled event retrieval

**Retrieval information**
- Allocated event name
- Retrieval amount
- Reason for retrieval

> Retrieved funds go back into the pool used for appeals. File promptly when you know an event is off.

---

## Before you file — the standing checklist

1. **Check the balance** on the Daily Report for the account and event you're spending from.
2. **Check the rules** for what you're buying ([restrictions.md](restrictions.md),
   [financial-policies.md](financial-policies.md)).
3. **Check the process** for that spending method ([spending-methods.md](spending-methods.md)).
4. Know your **account, budget name, and line item** — every type asks.
5. Then file the FTF, and come in during credit card hours if it's a card purchase.
