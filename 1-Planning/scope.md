# Scope: SpendCLI

## In scope (MVP)
- Add an expense with amount, fixed category, optional note, and optional `--date` (default today): **US-01**
- List expenses, filtered by month and/or category: **US-02**
- Monthly summary: total per category and grand total: **US-03**
- Export all expenses to CSV with a header row: **US-04**
- Offline, local storage, no account (**NFR-01**); install-to-first-expense under 1 minute (**NFR-02**)

## Out of scope (MVP)
| Item | Note |
|---|---|
| Edit or delete an expense | Decided 2026-11-12. Known limitation: mistakes are fixed by hand-editing the local data file (its location and format are documented in Phase 3). |
| Custom categories | The category list is fixed in the MVP. |
| Multiple currencies / currency symbols | Amounts are plain numbers in one currency. |
| Budgets, alerts, recurring expenses | |
| Import (CSV, bank statements) | |
| Sync, cloud backup, multiple devices | |
| Charts or a GUI | |

## Future ideas
- `spend delete <id>` and `spend edit <id>` (first candidates for v1)
- User-defined categories
- Monthly budgets per category with a warning when exceeded
- CSV import
