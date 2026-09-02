# SU contacts — who to ask what

WashU-wide, so it lives in `reference/`. Your own e-board and vendor contacts go in
`orgs/<slug>/contacts.md`.

> Names below are the **current** holders per the live BEARings *Business Operations & SU Financial
> Contacts* card ([trello.com/c/3VpF2UAm](https://trello.com/c/3VpF2UAm)) and the **2026–2027 Student Group
> Handbook**, checked **2026-09-04**. Roles are stable year to year; people are not. The role addresses
> (`finance@`, `treasury@`, `budget@`, `activities@`) survive turnover — prefer them over personal
> addresses when the specific person doesn't matter.

## Business Operations team — day-to-day spending

Office: **Campus Life Suite, Danforth University Center (DUC) 270**, 8:30 am – 5:00 pm, Mon–Fri.
Deposits and drop-offs go to the **reception desk on the second floor of the Campus Life Suite (Room 270)**
during those hours.

Your **Business Coordinator is assigned by your group's category**. This is your first call for anything
about actually spending money.

| Coordinator | Covers these group types | Contact |
|---|---|---|
| **Jack Schurk**, SU Business Coordinator | Cultural, Diversity & Inclusion, Performing Arts, **Religious & Spiritual** | j.schurk@wustl.edu |
| **Pam Hayes**, SU Business Coordinator | Sports Clubs, Environmental & Sustainability, Recreational | hayesp@wustl.edu |
| **Kim Moseby**, SU Business Coordinator | Academic & Pre-Professional, Governing, Health & Wellness, Honorary, Media, Political Action, Service & Community Engagement, Social Justice, Special Interest — plus **Sorority & Fraternity chapters** and **Student Union Entities**, which the card's list omits | moseby@wustl.edu |
| **Cathy Winter**, SU Business Manager | Finance rules and processes, student group support, process feedback — and the **one-per-year late expense-report exception** | catherine.winter@wustl.edu |
| **Jordan Burrows**, Administrative Coordinator (Campus Life) | Records cash/check deposits at the DUC 270 reception desk and hands you the receipt; your Business Coordinator then processes the deposit | Email not published on the board — go to the reception desk |

All four Business Ops staff offer bookable appointment times (Outlook Book-with-me / Bookings links are on
the contacts card).

> **Look your own group up rather than reasoning from the category table.** The authoritative mapping is
> the attachment `Campus_Life_Advisors_&_Business_Coordinators_2026_-_2027.xlsx` (also published as
> `FY27_Campus_Life_Advisors_&_Business_Coordinators.xlsx`), one row per group, ~355 groups. The
> category-level assignment above holds for the overwhelming majority, but the sheet contains **individual
> exceptions** — e.g. a couple of Governing and Service groups sit with Jack Schurk rather than Kim Moseby.
>
> ```bash
> python tools/su_board.py get "Campus_Life_Advisors" --out /tmp
> python tools/su_board.py xlsx /tmp/<file>.xlsx --grep "<your group name>"
> ```

> **One name discrepancy to be aware of.** The contacts card lists **"Kim Moseby, SU Business
> Coordinator"** with `moseby@wustl.edu`, but her booking link is labelled **"Book time with Kenyatta."**
> The board doesn't reconcile the two. Use the email; don't assume either first name in writing.

## SU Financial Leadership — policy, allocations, appeals

| Role | Current holder | Ask them about |
|---|---|---|
| **Vice President of Finance** | Cora Johnson — finance@su.wustl.edu | SU Financial Guidelines, **appeals under $1K**, executive appeals, the General Budget, WUGO/Workday, funding allocations, reallocations between events, running out of SU printing money |
| **Speaker of the Treasury** | Palladium Liang — treasury@su.wustl.edu | **Appeals over $1K**, Treasury processes, Treasury rationale, legislative matters |
| **Activities Committee Chair** | Aram Ashrafzadeh — activities@su.wustl.edu | New group applications, category changes, deregistration, name/mission changes, activities fairs, SU long-term storage |
| **Budget Committee Chair** | Molly James — budget@su.wustl.edu | The annual budgeting process, your group's budget |

> ⚠️ **Open cards still name last year's officers. Don't trust card text over this table.** Two live
> examples on the board right now: the **Budget Allocation Manual** card is a signed announcement email
> reading *"My name is Palladium Liang and I am pleased to serve as your Budget Committee Chair for Spring
> 2026"* — he is now **Speaker of the Treasury**, and Molly James chairs Budget. And the **SU Student Group
> Recognition** and **Category Change** cards both link to an Activities Committee Chair card named **Meris
> Damjanovic**, a prior-year holder. This is trap 1 from [trello-board.md](trello-board.md) leaking into
> *open* lists, not just archived ones. **Write to the role address.**

## Campus Life

Every recognized undergraduate group has an assigned **Campus Life Advisor** — a different person from your
faculty/staff advisor, and a different person from your SU Business Coordinator. Your advisor owns the
question *"can this event happen?"*; your Business Coordinator owns *"can SU money pay for it?"*

| Role | Contact | Ask them about |
|---|---|---|
| **Your Campus Life Advisor** | assigned to your group — record in `orgs/<slug>/contacts.md` | Event approval, risk, space, food safety, alcohol, speakers, contracts, good standing |
| **Scott Williams**, Assistant Director for Student Involvement & Student Groups | scott.williams@wustl.edu | New group formation (a **required meeting before** you submit the registration form), **external sponsorships / donations / in-kind support** (Sponsorship Proposal Form) |
| **Zachary Littrell**, Assistant Director for Sorority & Fraternity Life | littrell@wustl.edu | Sorority & Fraternity Life |
| **Performing Arts Department** | pad@wustl.edu; Kelly Ging (ging@wustl.edu), Ryadah Heiskell (rjheiske@wustl.edu) | Reserving **Olin Studio 1 & 2** — requires a 30-minute training first. See [su-resources.md](su-resources.md) |

### Finding your advisor's full name

The FY27 spreadsheet gives your advisor's **first name only**. The **Student Group Handbook (p. 3)** is the
only place the board publishes the full Campus Life roster, and it marks Campus Life Advisors with an
asterisk. Pairing the two:

| Spreadsheet first name | Handbook entry | Typically advises |
|---|---|---|
| Ethan | **Ethan Miller**, Coordinator for In the Lou Programming | Academic / Pre-Professional |
| Jacob | **Jacob Goedde**, Coordinator for Diverse Communities & Group Development | Cultural, Diversity & Inclusion, Religious & Spiritual |
| Jasmine | **Jasmine James-Milford**, Coordinator for Programming & Marketing | Performing Arts |
| Adam | **Adam Brok**, Coordinator for Service & Immersion Experiences | Service & Community Engagement |
| Scott | **Scott Williams**, Assistant Director for Student Involvement & Student Groups | Sports Clubs, Recreation, Health & Wellness |
| Josh | **Joshua Mathews**, Coordinator for Leadership Education & Advising | Media, Honorary, Social Justice, Special Interest, Environmental & Sustainability |
| Sarah | **Sarah Edmondson**, Associate Director for Student Involvement | Governing, Student Union Entities |
| Zach | **Zachary Littrell**, Assistant Director for Sorority & Fraternity Life | Sorority & Fraternity chapters |

> **This pairing is inferred from matching first names across two documents, not stated anywhere on the
> board.** It is right often enough to be useful and wrong badly enough to be worth confirming. **The board
> publishes no email addresses for these staff** except Scott Williams and Zachary Littrell — ask your
> Business Coordinator or the DUC 270 reception desk for the rest rather than guessing at an alias pattern.

Also on the Campus Life roster (handbook p. 3), not advisors: **Marco Valenzuela** (Director), **Carynn
Smith** (Associate Director for Programming & Campus Vibrancy), **Will Atchinson** (Technology Specialist),
**Rachel Pepe** (university-wide graduate student groups). Two positions are listed **vacant**: Associate
Director for Leadership Programs, and **Coordinator of Education & Compliance**.

## Routing cheat-sheet

| Situation | Go to |
|---|---|
| "How do I pay this vendor?" | Business Coordinator |
| "Can we buy this at all?" | Business Coordinator; VPF decides genuine ambiguity |
| Appeal for **< $1,000** | VP of Finance (finance@su.wustl.edu) |
| Appeal for **> $1,000** | Speaker of the Treasury (treasury@su.wustl.edu) |
| Reallocating between different events | VP of Finance, via the FTF |
| Reallocating between lines in the same event | Business Operations staff, at spending time |
| Annual budget questions | Budget Committee Chair (budget@su.wustl.edu) |
| A company wants to sponsor us | Scott Williams, Campus Life — **before** you accept anything |
| We received a gift or donation from a department, sponsor or individual | Your **Business Coordinator, in advance** (Student Group Handbook) |
| Can this event happen / is it registered? | Campus Life Advisor |
| Late expense report, need the annual exception | **Business Manager** (Cathy Winter) |
| We're on the Out of Compliance List | Business Coordinator; the fix is the named officer finishing the Canvas training |
| Where's our package? | DUC 270 reception desk |
| Reporting an incident during group travel | Campus Life Travel Incident Report Form — see [campus-life.md](campus-life.md) |
| Feedback on how SU finance runs | Student Group Feedback Form (FORMS list on the board) |

## Other channels

- **Instagram** `@su_treasury` — reminders, funding decisions, legislation. The board pushes this twice, on
  both the *Welcome Message* and *Student Union Website & Instagram* cards
- **SU website** — [studentunion.wustl.edu](https://studentunion.wustl.edu/) — event calendar, SU Exec
  contacts, Senate info, and SU Finance BEARings
- **Campus Life website** — `campuslife.wustl.edu` → Get Involved → Student Groups → **Student Group
  Resource Hub**, which replaced the old Canvas "Student Group Starting Point" and needs no login
- **Treasury minutes & P&T emails** — posted to a Google Drive folder linked on the *Communications: P&T,
  Minutes, and Reports* card, starting the first week of the fall semester
- **Credit card hours** (subject to change): **Thu & Fri, 10 am–12 pm and 2 pm–4 pm**, DUC Suite 270 —
  semester start/end dates in [calendar.md](calendar.md)
- **Packages**: pick up at the DUC 270 reception desk within **7 days** of receipt. The arrival tracker is a
  **SharePoint sheet requiring WashU SSO** (linked on the PACKAGES card) — an agent cannot read it for you
- **Mailing address for checks made out to WashU**: Washington University in St. Louis, 1 Brookings Drive,
  MSC 1128-226-270, St. Louis, MO 63130. Ask issuers to make checks payable to *Washington University* with
  your group name on the memo line
