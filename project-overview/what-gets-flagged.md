---
description: The specific variances and issues the tool will detect
---

# What Gets Flagged

The system runs a comprehensive set of checks across every employee and every shift. Here's what it catches:

---

## Roster vs Actual — Per Employee

| Check | What It Flags |
| --- | --- |
| **Hours Variance** | Total rostered hours vs total actual hours — flags when an employee works significantly more or less than planned |
| **Cost Variance** | Planned cost (from roster) vs actual cost (from payslip) — shows the dollar impact of the variance |
| **Unrostered Shifts** | Shifts that appear on the timesheet but were never on the roster — unplanned labour cost |
| **Unfilled Shifts** | Shifts on the roster that were never worked — planned labour that didn't happen |

---

## Roster vs Actual — Per Shift

| Check | What It Flags |
| --- | --- |
| **Extended Shifts** | Employee rostered 8am–4pm but actually worked 7:30am–4:30pm — early starts, late finishes |
| **Overtime Triggers** | Extra hours that push into overtime rates — quantifies the cost impact of the rate change |
| **Location Mismatch** | Rostered at Albert Park but timesheet shows they worked at Seddon |
| **Work Type Mismatch** | Rostered as ordinary hours but paid at Saturday or overtime rates |
| **Break Compliance** | Rostered breaks not taken or shortened — affects both cost and compliance |

---

## Wage % Monitoring — Per Location

| Check | What It Flags |
| --- | --- |
| **Wage % vs Target** | Total wages as a percentage of revenue — flags when above your configured threshold |
| **Trend Direction** | Whether wage % is improving or deteriorating compared to previous periods |
| **Location Comparison** | Which locations are running efficiently and which are over budget |

---

## Example Outputs

> **Employee: John Smith — Albert Park**\
> Rostered: 72.0 hours |  Actual: 78.5 hours |  Variance: +6.5 hours\
> Planned cost: $2,185 |  Actual cost: $2,450 |  Over budget: **+$265**\
> 2 unrostered shifts detected (Sat 8 Feb, Sun 9 Feb)

> **Location: Laundry — Fortnight ending 24 Feb**\
> Total wages: $32,400 |  Revenue: $89,000 |  Wage %: **36.4%**\
> Target: 32% |  Status: **Over target**\
> Top contributor: 4 unrostered overtime shifts (+$1,200)

---

## Severity Levels

Every flag is categorised by severity to help you prioritise:

| Severity | Meaning | Example |
| --- | --- | --- |
| **Critical** | Significant cost impact, immediate attention needed | Wage % 10%+ over target |
| **High** | Material variance that should be investigated | Employee 8+ hours over roster |
| **Medium** | Minor variance worth reviewing | Shift extended by 30–60 minutes |
| **Low** | Informational | Small timing differences within tolerance |
