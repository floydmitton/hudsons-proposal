---
description: Everything included in this engagement
---

# Scope of Work

This solution is built as an extension of Nine Advisory's existing payroll monitoring platform, leveraging infrastructure already in place (file upload, employee matching, validation engine, reporting, and dashboard).

---

## Data Ingestion

| Data Source | Format | Purpose |
| --- | --- | --- |
| **Payslips** | PDF (KeyPay) | Actual pay rates, gross earnings, hours by component |
| **Rosters** | Excel (Employment Hero) | Planned shifts, locations, expected cost per shift |
| **Timesheets** | Excel (KeyPay) | Actual shifts worked, hours, locations |
| **Revenue** | Manual entry via dashboard | Weekly/fortnightly revenue per location |

The system accepts uploads each pay period and automatically extracts, matches, and analyses the data.

---

## Employee Matching

Employees are automatically matched across all three data sources using a combination of employee ID matching, name normalisation, and AI-assisted fuzzy matching. This handles the common challenge where names appear differently across systems.

---

## Roster vs Actual Analysis

The core of the tool — for each employee, each shift, and each location:

### Per-Employee Analysis
- Total rostered hours vs total actual hours (with variance flagging)
- Planned cost (from roster) vs actual cost (from payslip) with dollar variance
- List of specific shifts that differed from the roster

### Shift-Level Flagging
- **Unrostered shifts** — worked but not on the roster (unplanned cost)
- **Unfilled shifts** — on the roster but not worked
- **Extended shifts** — worked longer than rostered (early starts, late finishes)
- **Overtime triggers** — extra hours pushing into overtime rates
- **Location mismatches** — rostered at one location, worked at another
- **Break compliance** — rostered breaks not taken or shortened

### Per-Location Summary
- Total rostered vs actual hours by location
- Total planned vs actual cost by location
- Headcount variance (rostered vs actual)
- Top variance contributors

---

## Wage % Monitoring

- Calculate total wage cost as a percentage of revenue per location per period
- Configurable target thresholds (e.g. target 30%, warning at 35%, critical at 40%)
- Visual traffic light indicators (green/amber/red)
- Period-over-period trend tracking

---

## Dashboard & Reporting

### Interactive Dashboard
- Wage % overview with trend across periods
- Per-location wage % breakdown
- Top variances ranked by dollar impact
- Drill-down from location to employee to individual shifts

### Excel Export
- **Summary sheet** — totals by location
- **Employee detail sheet** — per-employee roster vs actual
- **Shift variance sheet** — every shift with planned vs actual side by side
- **Wage % sheet** — revenue vs wages by location
- **Unrostered shifts sheet** — all unplanned labour

---

## Standard Payroll Validation

In addition to roster analysis, the tool runs standard payroll checks:

- Timesheet hours vs payslip hours reconciliation
- Leave compliance checks
- Employee coverage verification

---

## Out of Scope (This Phase)

- Lighthouse and Playcollective integration (future phase)
- Direct API integration with KeyPay or Employment Hero (manual upload for now)
- Automated revenue feeds from POS/accounting systems
- Award rate interpretation or pay rate calculations
- Rostering recommendations or schedule optimisation
- Mobile application
