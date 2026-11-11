# Security policy

This is a learning repository. Do not place credentials or environment-specific secrets in source control.

## Never commit

- Azure passwords, client secrets, access tokens, certificates, or private keys.
- Service Bus keys, connection strings, or SAS tokens.
- Logic App callback URLs containing signatures (for example, `sig=`).
- Unredacted screenshots or exported templates containing secrets, tenant IDs, subscription IDs, or personal information.

## Before every commit

1. Review `git status`.
2. Inspect changed files for secrets and tenant-specific values.
3. Replace sensitive values with obvious placeholders.
4. Keep local settings and secret files ignored by `.gitignore`.

If a credential is exposed, revoke or rotate it immediately. Removing it in a later commit does not erase it from Git history.
