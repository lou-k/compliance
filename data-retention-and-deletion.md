# Data Retention and Deletion

Effective 2026-10-06. Applies to the personal budgeting application
described in the [privacy policy](privacy-policy.md).

## Retention

| Data | Retained |
|---|---|
| Bank transactions and balances | As long as the application is in use; up to 24 months of history is fetched when a bank is first linked |
| Plaid access tokens | Until the bank is unlinked; stored inside the encrypted database |
| Sync run logs | 90 days, pruned automatically |
| Generated budget page | Until the next sync overwrites it |
| Monthly budget reports | As long as the application is in use; one per reviewed month, stored in the encrypted database |

Everything is stored on hardware the operator owns, encrypted at rest.

## Deletion

To remove one bank, the operator removes the connection at Plaid, after which
Plaid stops providing data for it, and deletes that bank's data from the
database.

To delete everything, the operator removes every bank connection at Plaid,
deletes the database, the generated page and the monthly reports, deletes any
copy of the database, and discards the encryption key so that any copy that was missed
stays unreadable.

Deletion is manual and is done by the operator, who is the only person whose
data is involved.
