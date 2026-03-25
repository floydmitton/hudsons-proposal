---
description: From file upload to actionable insights in minutes
---

# How It Works

## The Process

Each pay period (fortnightly), the process is simple:

### Step 1 — Upload Files

Upload three files into the platform:

| File | Source | Format |
| --- | --- | --- |
| **Payslips** | KeyPay | PDF |
| **Rosters** | Employment Hero | Excel (.xlsx) |
| **Timesheets** | KeyPay | Excel (.xlsx) |

Optionally enter **revenue per location** for wage % tracking.

### Step 2 — Automatic Extraction

The system automatically extracts and structures data from each file:

- **Payslips** — Employee ID, name, job title, hourly rates (including casual loading, Saturday rates, overtime rates), hours by pay component, gross/net earnings
- **Rosters** — Shift start/end times, employee, location, break times, work type, planned cost per shift
- **Timesheets** — Actual shift start/end times, employee, location, duration, breaks, work type

### Step 3 — Employee Matching

Employees are automatically matched across all three data sources using:

- **Employee ID** matching (payslip to timesheet)
- **Name matching** with intelligent normalisation
- **AI-assisted fuzzy matching** for edge cases (e.g. "Al Amin Bhuiya" in the roster matching to "Abdur Rahim Al Amin Bhuiya" in payslips)

### Step 4 — Shift-Level Comparison

Each rostered shift is paired with the corresponding timesheet entry by employee, date, and approximate start time. This identifies:

- **Matched shifts** — roster and timesheet align
- **Unrostered shifts** — worked but not on the roster (unplanned cost)
- **Unfilled shifts** — on the roster but not worked
- **Extended shifts** — worked longer than rostered

### Step 5 — Analysis & Flagging

Validation rules run across every employee and shift to flag variances, calculate cost impacts, and determine wage percentages by location.

### Step 6 — Results & Reports

View results in the **interactive dashboard** or export a **formatted Excel report** with full detail for management review.

---

## Data Flow

```
Payslips (PDF) ─────┐
                     │
Rosters (Excel) ─────┼──▶ Extract ──▶ Match ──▶ Compare ──▶ Flag ──▶ Report
                     │
Timesheets (Excel) ──┘
```

The entire process runs in **minutes**, not hours — upload your files and have actionable insights ready for the same meeting.
