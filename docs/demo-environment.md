# Demo environment

[← Back to README](../README.md)

## Dataset

- **Period:** six consecutive months of due dates, Jun–Nov 2026 — 120 obligations.
- **Categories:** Team Payments (Team Member A–E, fictional monthly amounts from USD 2,500 to 4,800), Tools & Subscriptions (generic tool names), Operating Costs (coworking, accounting, bank and payment-processing fees, a quarterly retainer, annual renewals and one equipment purchase).
- **Reference date:** Nov 15, 2026 (`Settings!B2`). With this date the dataset contains 111 paid, 6 pending and 3 overdue obligations — including one overdue item from October.
- **Examples included on purpose:** a payment made after its due date (still *Paid*), a payment made before its due date, and open items both before and after the reference date.
- **Currency:** USD.

## Rules

| Rule | Detail |
| --- | --- |
| Status | Paid = paid date exists · Pending = open and due on/after the reference date · Overdue = open and due before the reference date |
| Open balance | Pending + Overdue |
| Invoice total | Paid + Open balance (checked in *Monthly Summary* and on the dashboard) |
| Monthly grouping | By the month of the **due date**, not the payment date |
| Partial payments | Not used in this demo — each obligation is either fully paid or fully open |

## How the demo relates to the original

| Original operation | Demo |
| --- | --- |
| Separate tabs for team payments and for tools, with a status typed by hand | One consolidated register with a **Category** column and a **Status formula** based on dates |
| Monthly invoice dashboard used by the founder on a phone | Rebuilt from scratch as an interactive WordPress page reading only the demo spreadsheet |
| Payment calendar in Notion with reminders | Documented in [payment-calendar.md](payment-calendar.md); not reproduced interactively |

## What is not published

Real names, vendors, amounts, dates, payment details, links, screenshots, workspace content and the name of the company.
