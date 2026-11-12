# Requirements: SpendCLI (MVP)

| ID | User story | Acceptance criteria |
|---|---|---|
| US-01 | As a user, I can add an expense | `spend add 250 food "lunch"` saves amount, category, note and date. The date defaults to today; `--date YYYY-MM-DD` logs a past expense. The amount must be a positive number (up to 2 decimals). The category must be one of the fixed list below; anything else is rejected with a message listing the valid categories. The note is optional. |
| US-02 | As a user, I can list expenses | `spend list` shows expenses, newest first. Can be filtered by month (`--month YYYY-MM`) and/or category (`--category food`). |
| US-03 | As a user, I can see a monthly summary | `spend summary` shows the total per category and the grand total for the current month; `--month YYYY-MM` for another month. |
| US-04 | As a user, I can export to CSV | `spend export` writes valid CSV with a header row (date, amount, category, note). |

## Fixed categories
`food`, `transport`, `bills`, `shopping`, `other` (case-insensitive input, stored in lowercase).

## Non-functional
| ID | Requirement |
|---|---|
| NFR-01 | Works fully offline, with no account or sign-up. |
| NFR-02 | A new user can install it and log their first expense in under 1 minute. |
