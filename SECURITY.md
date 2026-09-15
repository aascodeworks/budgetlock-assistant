# Security

## Only use the file from these addresses

- https://budgetlock.app/model (the download page)
- https://budgetlock.app/downloads/BudgetLock-Assistant-v6.gguf
- the releases of this repository

Budget Lock refuses a file whose size or SHA-256 does not match the version
the app expects, so a copy from anywhere else either passes that check (and
is the same file) or is not used. You can run the same check yourself:
[docs/verify-the-file.md](docs/verify-the-file.md).

## Reporting a problem

Email **support@budgetlock.app** if:

- a file from one of the addresses above does not match the SHA-256 listed in
  [CHANGELOG.md](CHANGELOG.md),
- you find the file offered somewhere else under the Budget Lock name,
- or you think you have found a security issue in Budget Lock.

Please do not open a public issue for a security problem.
