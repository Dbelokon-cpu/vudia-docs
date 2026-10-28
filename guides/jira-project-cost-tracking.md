---
title: How to track project cost, budget and profit in Jira
description: A practical guide to calculating project cost, budget vs actual and profit margin in Jira Cloud from worklogs, with hourly rates, and what to look for in an app.
---

# How to track project cost, budget and profit in Jira

Jira tracks time and work, but not money. To know what a project costs and whether it makes a profit, you need three inputs: **time spent per person** (worklogs), **a rate per hour** for each person or role, and **a budget**. This guide covers the options.

## The three building blocks

1. **Worklogs.** Time logged on issues. This is the only reliable source of "who spent how long".
2. **Rates.** A *cost rate* (what an hour costs you) and a *billing rate* (what you charge). Cost = hours x cost rate. Revenue = hours x billing rate, or a fixed price.
3. **Budget.** The amount you planned. Budget vs actual and remaining budget follow from the first two.

Profit = revenue - cost. Margin = profit / revenue.

## Option 1: spreadsheets

Export worklogs, multiply by a rate table, sum by project. Works for one or two projects but needs a manual export every time and goes stale immediately.

## Option 2: a Jira Marketplace app that reads worklogs

An app that reads existing worklogs and applies rates removes the manual step: numbers update when someone logs work. When comparing apps, check:

- Does it use existing Jira worklogs, or force a new time tracker?
- Can it hold both cost and billing rates, per person and per role?
- Does it show budget vs actual, remaining and forecast?
- Does it handle fixed-price revenue as well as hourly billing?
- Can it combine projects into portfolios?
- Does it export (XLSX)?
- Where does data live (Forge / Atlassian-hosted vs external servers)?

**[Cost Tracker for Jira](https://marketplace.atlassian.com/apps/2743016176/cost-tracker-financial-budget-rates-and-profit-for-jira?hosting=cloud&tab=overview)** covers all of the above for Jira Cloud: cost and billing rates per person, role or account; budget vs actual with forecast; revenue, margin and profit; portfolios; recurring expenses; CAPEX/OPEX accounts by JQL; XLSX export; and it runs on Forge with no external servers. See the [product overview](../cost-tracker/index.md).

## Option 3: BI tools

Pull worklogs into a BI tool and model rates there. Powerful, but needs setup and maintenance.

## Recommended setup

1. Make sure the team logs work in Jira.
2. Define rates by role, then override for specific people.
3. Set a budget per project and, if you bill clients, a billing rate or fixed price.
4. Group related projects into a portfolio and review budget vs actual weekly.
