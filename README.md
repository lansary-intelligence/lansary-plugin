# Lansary Plugin — Public Beta

Company research in ChatGPT and Claude, with evidence, sources and dates.

**Status: Public beta · v0.1.0-beta.1**

This is Lansary's public connection package and installation guide for its hosted research service. It is independently provided by Lansary. Public beta access does not imply directory approval, certification or endorsement by OpenAI or Anthropic.

## Get started

1. [Create your free Lansary account](https://mcp.lansary.com/signup) using your email and a one-time sign-in code.
2. Follow the guide for your assistant:
   - [Install in ChatGPT](docs/chatgpt.md).
   - [Install in Claude](docs/claude.md).
3. Approve research access, select Lansary in a conversation and ask a company question.

You do not need to download this repository, run a server or keep your computer on. Your assistant connects to Lansary's hosted service. Platform plans, workspace permissions and regional availability can affect access.

## Connection details

| Setting | Value |
| --- | --- |
| Name | Lansary |
| MCP server URL | `https://mcp.lansary.com/mcp/research` |
| Transport | Streamable HTTP |
| Authentication | OAuth |
| Research scope | `company:research` |

Use your own Lansary account. The normal customer connection does not require a shared API key, database connection string or a client secret copied from this repository.

## What you can research

- Resolve a business name to the correct registered legal entity.
- Follow the available registered ownership and control chain.
- Explore financial filing facts with their reporting periods.
- Compare companies using the evidence available for each one.
- Follow source links and identify gaps requiring further research.

The initial customer release focuses on UK register entities and public-source company facts. Coverage varies. Extracted figures are not independently verified; missing evidence does not establish that an activity does not exist.

## Free allowance

Five distinct companies are included per UTC calendar month. Use the same Lansary email across ChatGPT, Claude and the website to share your allowance. Search is free; opening evidence for a new company uses one brief. Follow-up evidence for that company is included during the month. The allowance resets on the first. No card is required.

The research connector is read-only. It does not place orders, initiate payments, edit company records or run monitoring jobs.

## Try a question

> Use Lansary to research Sheffield Forgemasters International Limited, company number 04883675. Confirm the legal entity, follow its registered ownership chain and show the sources, source dates and financial reporting periods. Flag gaps in the evidence.

> Use Lansary to trace Tidyco Limited's registered ownership chain. Explain where the evidence stops.

## Public package, private service

This repository contains documentation and connection manifests only. Lansary's backend implementation, database, account records, private source material and credentials are not included. The manifests declare a public HTTPS endpoint and OAuth connection settings; authentication takes place through Lansary.

See [security and privacy](SECURITY.md), [the changelog](CHANGELOG.md) and [package installation for compatible desktop clients](docs/package-installation.md).

## Support and service information

- [Lansary company research](https://lansary.com/company-research/)
- [Hosted connection guide](https://mcp.lansary.com/directory)
- [Support](https://mcp.lansary.com/support)
- [Privacy notice](https://mcp.lansary.com/privacy)
- [Service terms](https://mcp.lansary.com/terms)

Use public GitHub issues for general documentation or installation feedback. Send account problems, private company questions and security reports through the support channel. Never post sign-in codes, tokens or other credentials.

Lansary is a trading name of Quorion Ltd. ChatGPT and Claude are products of their respective owners.
