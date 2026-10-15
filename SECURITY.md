# Security and privacy

## Public and private boundaries

This public beta repository contains installation documentation and client connection metadata. It contains no backend source, database exports, account records, private repository history or credentials.

Lansary research requests go to `https://mcp.lansary.com/mcp/research` over HTTPS and require customer authentication. Each user authorises access through OAuth using their own Lansary account. The public package does not provide database access.

The research connection is read-only. It does not initiate payments, modify company records or create monitoring jobs.

## Report a problem privately

For a suspected vulnerability, exposed credential, account issue or privacy request, use [Lansary support](https://mcp.lansary.com/support) or email jamie.lansdell@lansary.com.

Include a brief description and redacted reproduction steps. Do not include passwords, one-time sign-in codes, OAuth tokens, payment details or private research material. Do not post security reports or credentials in public GitHub issues.

## For contributors

Only documentation and public connection metadata belong in this repository. Never add:

- Environment files, OAuth credentials, access or refresh tokens, sign-in codes or private keys.
- Database connection strings, schema dumps, database exports or customer records.
- Backend code copied from private projects, raw evidence files, logs or private screenshots.
- Private repository URLs, internal file paths or internal operational instructions.

Review the exact files and commit diff before publishing. Ignore rules reduce accidental additions; they do not remove secrets that have already been committed.

## Service privacy

The assistant platform receives the research results returned by the connector. Review its privacy settings alongside the [Lansary privacy notice](https://mcp.lansary.com/privacy) and [service terms](https://mcp.lansary.com/terms).
