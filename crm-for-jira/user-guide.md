# Dealtrail CRM: User Guide

Dealtrail CRM keeps your sales pipeline inside Jira. You track leads, contacts,
companies, deals, products and tasks in one place, and you can link any record
to a Jira work item.

Open it from the **Apps** menu in Jira, then choose **Dealtrail CRM**. There is
nothing to sign in to: you use the same account as in Jira.

## Contents

1. [Finding your way around](#finding-your-way-around)
2. [A typical sales flow](#a-typical-sales-flow)
3. [Leads](#leads)
4. [Deals](#deals)
5. [Contacts and Companies](#contacts-and-companies)
6. [Products](#products)
7. [Tasks](#tasks)
8. [Notes, Timeline and record cards](#notes-timeline-and-record-cards)
9. [Searching, filtering and saved views](#searching-filtering-and-saved-views)
10. [Working with many records at once](#working-with-many-records-at-once)
11. [Import and export](#import-and-export)
12. [Dashboard](#dashboard)
13. [Reports](#reports)
14. [Activities](#activities)
15. [Settings](#settings)
16. [Linking to Jira and sharing records](#linking-to-jira-and-sharing-records)
17. [Jira Automation](#jira-automation)
18. [Good to know](#good-to-know)
19. [Privacy](#privacy)

## Finding your way around

The menu on the left has ten sections:

| Section | What it is for |
|---|---|
| **Leads** | People or companies that might become customers |
| **Deals** | Sales opportunities moving through the pipeline |
| **Contacts** | People you deal with |
| **Companies** | Organisations, including parent and subsidiary links |
| **Products** | Your catalogue of things you sell |
| **Tasks** | To-dos, calls, emails and meetings |
| **Dashboard** | Numbers that show what needs attention |
| **Activities** | A log of who changed what |
| **Reports** | Charts and breakdowns, with a period comparison |
| **Settings** | Currency, the stale-deal threshold and data tools |

A number in brackets after a section name, such as **Tasks (3)**, means that
section has items needing attention (for example overdue tasks).

Each section has its own search box. Where a form links one record to another
(a deal's contact, a contact's company), start typing a name in the picker: it
finds records whose name, or for people whose surname, begins with what you
typed.

## A typical sales flow

1. A new prospect arrives. Add it as a **Lead**.
2. Contact them and update the lead's status. When it looks real, press
   **Convert**. The lead becomes a **Deal**.
3. Move the deal through the stages, adding notes, products and tasks.
4. When it ends, mark the deal **Won** or **Lost** and say why. Those reasons
   feed the reports.

## Leads

A lead is someone who has shown interest but is not yet a customer.

**Add a lead:** open **Leads**, press **Create Lead**, fill in the form and
press **Create Lead** again. Only the name is required. Useful fields:

- **Status**: New, Contacted, Qualified, Converted or Lost.
- **Rating**: Hot, Warm or Cold.
- **Source**: Web, Referral, Advertisement, Trade Show, Cold Call, Partner or
  Other.
- **Assignee**: who is responsible for the lead.

Two ways to look at leads: **Table** and **Kanban**. Switch with the buttons
above the list. In Kanban, each column is a status.

**Losing a lead:** when you set the status to Lost you are asked for a reason
(Unqualified, No Response, Not Interested, Duplicate, Wrong Contact or Other).

**Converting a lead:** open the lead and press **Convert to Deal**. You are
asked to confirm. The app creates a deal, carries over the lead's products,
and marks the lead Converted. The lead's card then shows the **Converted deal**
so you can jump to it.

Two leads or contacts cannot share the same email address. The app tells you
if you try.

## Deals

A deal is a sale you are working on.

**Add a deal:** open **Deals**, press **Create Deal**. Fields include name,
amount, **Close date**, **Next step** and its due date, **Type** (New Business,
Existing Business or Renewal), the contact and the company, and the owner.

### Stages

Every deal is in one stage of your pipeline. A new workspace starts with
these, each with a default chance of winning:

| Stage | Win probability |
|---|---|
| New | 10% |
| Discovery | 25% |
| Negotiation | 50% |
| Proposal | 75% |
| Won | 100% |
| Lost | 0% |

A Jira administrator can change the stages before Won and Lost in
**Settings → Deal Stages** (see [Settings](#settings)). Won and Lost are always
there and always last.

You can set a different probability on a single deal if you know better.
**Weighted pipeline** is each open deal's amount multiplied by its probability.
It is a more realistic forecast than the raw total.

Change a stage by dragging the card to another column on the Kanban board, or
from the deal's stage selector.

**Won and Lost:** press **Mark as Won** or **Mark as Lost** on the deal. You
choose a reason (for example *Best Price* or *Product Fit* for a win, *Lost to
Competitor* or *No Budget* for a loss). Please always pick one, because
Reports break results down by reason.

### Kanban and Table

Deals open as a **Kanban** board with a column per stage and the total value of
each column. Press **Table view** to see them as a sortable list, and
**Kanban view** to go back.

### Products on a deal

Open a deal and add products from your catalogue as line items. The deal's
amount follows the line items.

### Stale deals

A deal is flagged **stale** when it has not changed stage for 14 days. An
administrator can change that number in [Settings](#settings). Use the **Stale**
filter to list them.

## Contacts and Companies

**Contacts** are people. Fields include name, title, email (and a secondary
email), phone, LinkedIn, tags, the company they work for, and who they
**Report to**. Tick **Do not contact** for people who must not be contacted;
there is a quick filter to show or hide them.

**Companies** are organisations. Fields include website, industry, address,
number of employees, annual revenue, tags, owner and a **Parent** company, so
you can model subsidiaries.

Opening a contact or company shows everything linked to it: deals, tasks,
notes and the people at that company.

**Deleting** a contact or company that has linked records shows a warning
first, so nothing disappears by accident.

**Merging duplicates:** open the duplicate record, choose **Merge into**, pick
the record you want to keep, and confirm with **Merge and Delete**. Everything
that pointed at the duplicate is moved to the record you keep.
Merging cannot be undone.

## Products

The **Products** section is your catalogue: name, **SKU**, **Price**, **Cost**,
category, unit (License, Service, Project, Subscription or One-time) and a
description. The list shows the margin. Open a product to see which deals use
it. The **Unused** filter lists products that no deal uses.

## Tasks

Tasks are things to do. Give a task a title, a type (To-do, Call, Email,
Meeting or Other), a priority (High, Normal or Low), a due date in
`YYYY-MM-DD` format and an assignee. A task can be tied to a lead, contact,
company or deal.

You can also add a task straight from a record's card (see below). Tick a task
to complete it. The **Overdue**, **Due Today** and **My Tasks** filters keep
your day under control, and the **Dashboard** lists tasks that are due soon.

## Notes, Timeline and record cards

Click a record's name anywhere in the app to open its **card**. Cards have
two columns: the details on one side, and three tabs on the other.

- **Tasks**: tasks tied to this record, with a box to add a new one.
- **Notes**: type in the *Add a note…* box and add it. Notes can be up to
  2000 characters.
- **Timeline**: every change made to the record, with who did it and when,
  for example *rating: Cold → Hot*.

The card also shows **Last activity**.

## Searching, filtering and saved views

**Search box in each section** searches that section. Long lists show 50 rows
at a time with page numbers under the table; search and filters always cover
the whole list. On the Kanban boards each column shows its first 25 cards and
says how many more there are; switch to the table view or filter to see them.

**Quick filters** sit above each list. Which ones you see depends on the
section: *My Leads/Deals/Contacts/Companies*, *Stale*, *Overdue*, *Due Today*,
*Unassigned*, *No Next Step*, *Do Not Contact*, *Unused* and filters by stage,
status, source, rating, industry and category. The numbered tiles on lists
work as filters too: click a tile and the list narrows to exactly those rows.

**Sorting:** click a column heading.

**Saved views:** once you have filters set, **Save view** appears. Give the view
a name and press **Save**. It shows up as a button above the list; click it to
bring those filters back, or **×** to delete it. Saved views are yours alone.

## Working with many records at once

Tick the boxes at the start of rows. Buttons appear for:

- **Assign owner**: choose a person and apply it to every selected row.
- **Change stage** (on deals).
- **Delete**: asks you to confirm before deleting.
- **Export selected rows to CSV**.

## Import and export

**Export:** press **Export CSV** on a list. A window shows the data as text.
Select all (Ctrl+A or Cmd+A), copy it, and paste it into a spreadsheet or a
file ending in `.csv`. Exports follow your current filters. Settings can also
export all your data.

**Import:** press **Import CSV** on Contacts, Companies, Leads, Deals,
Products or Tasks. Paste CSV text whose **first row is the column names**.
The window lists the column names it recognises. Each row is checked exactly
like the normal form, so a row with an invalid email, for example, is skipped
and listed with the reason; the other rows are still imported.
Check a few rows after importing: nothing can be undone in bulk.

## Dashboard

The **Dashboard** groups numbers by what you would do with each one, for
example open pipeline, weighted pipeline, win rate, sales cycle length,
tasks due soon and rep performance.

The tiles are clickable. Click **Stale** or **No Next Step** and you land on
the list of exactly those deals.

## Reports

Dashboard and Reports figures are worked out from a summary the app refreshes
every few minutes, so a change you just saved can take a little while to show.
The line under the title says when the figures were worked out; press
**Refresh** to update them now.

**Reports** are grouped into sections:

- **Pipeline**: deals by stage, value by stage, forecast by close month,
  open pipeline by owner, deals by type.
- **Leads**: by status, source and rating; conversion rate by source and by
  rating; lost leads by reason.
- **Revenue**: by lead source and assignee.
- **Deal outcomes**: why you win and why you lose.
- **Accounts** and **Products**: companies by industry and size, products by
  category.
- **Operations**: tasks by type, priority and assignee.

**Compare periods:** pick a period (This month, Last month, This quarter, This
year, Last 30 days) to see won value, deals won, deals lost, win rate and new
deals next to the period before, with the change.

**Report snapshot:** press it to get a short text summary. Copy it into a Jira
comment, a Confluence page or a chat message, and it shows up formatted.

Several tables have their own **Export to CSV** button.

## Activities

**Activities** is the log of every change: who created, edited, reassigned,
converted, merged or deleted what, and when. Filter by record type or event
type. Only the most recent 500 entries are kept.

## Settings

- **Currency**: USD, EUR, GBP, JPY or INR. It changes how amounts are shown
  everywhere; it does not convert existing amounts.
- **Stale deal threshold**: days without a stage change before a deal is
  flagged stale, from 1 to 365 (default 14).
- **Deal Stages** (Jira administrators): the stages a deal moves through
  before it is won or lost. Rename them, change their order with **Up** and
  **Down**, set each one's win probability, add up to 12 with **Add Stage**,
  or **Remove** one. If deals are still in a stage you remove, choose the
  stage they move to; they move when you press **Save Stages**, and the move is
  recorded on each deal's timeline. Won and Lost cannot be changed.
- **Custom Fields** (Jira administrators): fields of your own on contacts,
  companies, deals and leads, up to 15 per record type. Pick the record type,
  press **Add Field**, name it and choose its type: **Text**, **Number**,
  **Date** (typed as `YYYY-MM-DD`) or **Dropdown** (list the options, separated
  by commas). Then press **Save Fields**. Custom fields appear at the bottom of
  the record's form, in a **More fields** box on its card, and as columns in
  its CSV export. You can rename a field, reorder it and edit a dropdown's
  options later; its type is fixed once it is added. Removing a field hides
  its values, and they are cleared from a record the next time it is saved.
- **Data administration** (Jira administrators):
  - **Export All Data** as one CSV for backup.
  - **Load Sample Data** adds a small example pipeline (companies, contacts,
    deals, leads, tasks and notes) so you can try every screen. It is added
    next to your own records, and loading it twice gives two copies.
  - **Delete All Data** removes every record, note and history entry. Type
    DELETE to confirm. Settings are kept. This cannot be undone.
- **Data size**: press **Count Records** to see how many records each section
  holds. Sections are designed for up to 5,000 records each; one near or over
  that is marked, because opening it gets slower.
- **Audit log**: how many entries are kept.

Press **Save** after changing a setting. Settings apply to everyone on your
Jira site.

## Linking to Jira and sharing records

**Link to a work item:** many records have a **Jira** field. Type a work item
key such as `PROJ-123` and save. The app checks the item exists and that you can
see it, then shows its summary and status next to the record. Use it to point
a deal at the ticket that delivers it.

**See CRM records on the work item:** every Jira work item has a **CRM** panel
in its details sidebar. Expand it to see the deals, contacts, companies and
leads linked to that work item, with the deal's stage and amount or the
contact's company and email. Click a name to open its card in the CRM.
**Link a CRM record** links another one from right there: pick the record type,
type to search by name, press **Link**. **Unlink** removes a link. A record
links to one work item at a time, so linking it here moves it from wherever it
was linked before. Links and unlinks are recorded on the record's timeline.
When a work item is moved to another project, or a project's key is renamed,
its links follow it to the new key within a few minutes, and the change is
recorded on each record's timeline.

**Find work items by their CRM records:** every linked work item carries four
read-only fields: **Dealtrail Deals**, **Dealtrail Leads**, **Dealtrail
Contacts** and **Dealtrail Companies**. They follow the record as it changes,
and you can search on them in JQL, use them in filters and boards, and add
them as list columns:

| Field | You can search by |
|---|---|
| Dealtrail Deals | Name, Stage, Amount, CloseDate, Company, Owner |
| Dealtrail Leads | Name, Status, Rating, Source, Company, Assignee |
| Dealtrail Contacts | Name, Title, Company, Owner |
| Dealtrail Companies | Name, Industry, Country, Owner |

For example:

```
"Dealtrail Deals.Stage" = "Negotiation"
"Dealtrail Deals.Owner" = currentUser()
"Dealtrail Leads.Status" = "Qualified" AND status != Done
"Dealtrail Deals" is not EMPTY
```

A Jira administrator can add the fields to a work item screen to show them
there; search works without that. Anyone who can see the work item can read
these fields, so they hold no emails or phone numbers.

**Your follow-ups on a Jira dashboard:** add the **My CRM follow-ups** gadget
to a Jira dashboard (**Edit** the dashboard, then **Add gadget**). It lists
your open CRM tasks and the next steps of the deals you own that are overdue,
due today or due in the next 7 days. Click one to open it in the CRM, or press
**Done** to complete a task. Each person sees their own.

**Share a record:** every card has its own web address. When you open a card,
the address in your browser changes. Copy it and paste it into a Jira
comment, and whoever opens it lands on the same record.

## Jira Automation

Add Dealtrail CRM steps to a Jira Automation rule, so that something happening
in Jira updates the CRM. Search for "Dealtrail CRM" when adding an action:

- **Move deals in Dealtrail CRM** moves the open deals linked to a work item to
  a stage. Won and lost deals stay as they are, and a work item with no deals is
  skipped without an error.
- **Create lead in Dealtrail CRM** creates a lead, linked to the work item if
  you keep `{{issue.key}}`.
- **Add note in Dealtrail CRM** adds a note to every linked record of the type
  you choose.
- **Create task in Dealtrail CRM** creates a task on the work item's linked
  record, taking a deal first, then a contact, company or lead.

Text fields accept smart values such as `{{issue.summary}}`. For example: when a
work item moves to Done, move its deals to Won.

The first time you add a step, Jira asks you to connect Automation to the app.
Rule runs then act as the person on that connection, and the record's history
shows their name. If a step fails, the rule stops, and the reason is in the
rule's audit log.

Rules can't start from a change in the CRM: Jira doesn't let apps add their own
triggers.

## Good to know

- **Required fields** are marked. Email, phone and website are checked for a
  sensible format, and amounts must be zero or more.
- **Dates** are typed as `YYYY-MM-DD`, for example `2026-11-30`. There is no
  date picker.
- **Saving takes a moment.** Wait for the window to close before you move on.
- **Need more room?** The arrow at the top of the side menu collapses it to a
  narrow column of icons; hover over an icon to see its name. The app remembers
  your choice, for you alone.
- **Not included on purpose:** email, calendar and file attachments on
  records, email notifications and multiple pipelines. Reminders are the
  **My CRM follow-ups** dashboard gadget and the counts on the side navigation.
- **Large data sets:** each section loads its own records when you open it,
  and sections are designed for up to 5,000 records. If one starts to feel
  slow, tell your administrator.

## Privacy

Everything you enter stays in Atlassian's Forge storage on your own Jira site;
the app sends nothing to Vudia or anyone else. What is stored, why, and how it
is deleted is described in the [privacy policy](privacy-policy.md).
