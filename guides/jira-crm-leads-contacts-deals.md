---
title: How to manage leads, contacts and deals in Jira
description: A practical guide to running a sales pipeline alongside Jira Cloud, comparing spreadsheets, a Jira project used as a CRM, a separate CRM and a Jira app, and what to look for in each.
---

# How to manage leads, contacts and deals in Jira

Jira tracks the work, but not the customer behind it. To see who a project is for and what is still in the pipeline, you need three things: **a record of each customer**, **a pipeline of deals** and **a link between each deal and the work that delivers it**. This guide covers the options.

## The three building blocks

1. **Customer records.** Leads (people who might buy), contacts (people you deal with) and companies, with their notes and history.
2. **A pipeline.** Deals moving through stages, each with an amount, a close date and a win probability. Weighted pipeline = amount x probability, added up across open deals.
3. **A link to delivery.** A connection between a deal and its Jira work items, so that sales can see progress and delivery can see the customer.

Win rate = deals won / deals closed. Sales cycle = the time from a deal being created to it being closed.

## Option 1: spreadsheets

One row per customer or deal. Fine for a handful of deals, but there is no history of who changed what, no reminders, and no connection to Jira, so it goes stale quickly.

## Option 2: a Jira project used as a CRM

Create a project where each deal is a work item and each stage is a workflow status. You get boards and permissions at no extra cost. The weak spot is the data model: a contact or a company isn't a work item, so the same customer details get retyped on every deal, and forecasts need custom fields and manual reporting.

## Option 3: a separate CRM with an integration

A dedicated CRM has the deepest sales features, including email and calendar sync. The cost is a second tool, a second login and separate seats, and an integration to keep in step with Jira. It suits teams with dedicated sales staff who live in the CRM all day.

## Option 4: a Jira Marketplace app

A CRM app inside Jira keeps customers next to the work, with no second login. When comparing apps, check:

- Are leads, contacts, companies and deals real records, or just work items?
- Can you define your own stages and win probabilities, and see a weighted forecast?
- Can a work item show its customer and deal, and can you link from there?
- Can you search work items by CRM data in JQL?
- Can Jira Automation rules update the CRM?
- Does it have reports for win rate, sales cycle and forecast?
- Can you import existing data, and export it again?
- Where does data live (Forge / Atlassian-hosted vs external servers)?

**[Dealtrail CRM](../crm-for-jira/index.md)** covers all of the above for Jira Cloud: leads with one-click conversion to deals; contacts and companies; a Kanban pipeline with your own stages and a weighted forecast; a CRM panel on every work item; CRM fields in JQL; Jira Automation actions; dashboard, reports and CSV import and export. It runs on Forge with no external servers. It doesn't sync email or calendars, so a team that depends on those should look at Option 3.

## Recommended setup

1. Set your deal stages and win probabilities first, because reports and the forecast depend on them.
2. Import companies, then contacts, then deals, so that each one can link to the record before it.
3. Add new prospects as leads and convert them to deals only when they look real.
4. Link each deal to the Jira work item that delivers it.
5. Always record why a deal was won or lost, and review the pipeline weekly.
