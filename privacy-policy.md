# Privacy Policy

Effective 2026-10-06.

## Who this covers

This policy covers a personal-use budgeting application. Its only user is the
person who wrote and operates it (the operator), and the only data it handles
is the operator's own. Nobody else can create an account, link a bank or see
the data.

## What data is accessed

Through Plaid's Transactions product, the application reads from the
operator's bank accounts:

- account names, types and balances;
- transactions: date, amount, merchant or payee, Plaid's category, and
  pending status.

Access is read-only. The application cannot move money or change anything at
the bank. Plaid's own handling of the data is described in
[Plaid's end user privacy policy](https://plaid.com/legal/#end-user-privacy-policy).

## Why

To produce a monthly household budget: how much discretionary money is left,
how savings funds compare to their targets, and which reimbursements are
outstanding.

## Sharing

The data is not shared with, sold to, or made available to anyone. The only
third parties involved are the banks that hold the accounts and Plaid, which
fetches the data from them.

## Storage and security

The data is stored in a database encrypted at rest, on hardware the operator
owns and controls at home. The encryption key is kept separately from the
database. The budget page built from the data is served only on the
operator's home network, over TLS, behind a password.

## Retention and deletion

Transactions and balances are kept for as long as the application is in use.
Sync logs are kept for 90 days. Deleting a bank's data means removing the
bank connection at Plaid and deleting the data from the database; deleting
everything means removing every connection and deleting the database. The
full procedure is in
[data-retention-and-deletion.md](data-retention-and-deletion.md).

## Changes

Changes to this policy are made by commits to this repository, so its history
is the record of changes.

## Contact

Open an issue on this repository.
