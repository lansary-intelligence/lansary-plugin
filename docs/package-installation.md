# Package installation for compatible desktop clients

**Public beta.** The primary ChatGPT and Claude web installation routes are the [ChatGPT](chatgpt.md) and [Claude](claude.md) guides. These do not require cloning this repository.

The files below also support compatible plugin hosts. Availability varies by client and workspace policy. Repository package installation has not yet been verified end to end with a fresh customer account.

## Claude Code

Add Lansary's repository marketplace from a Claude Code session:

```text
/plugin marketplace add lansary-intelligence/lansary-plugin
/plugin install lansary@lansary-public-beta
```

Use `/mcp` to inspect the Lansary connection and complete OAuth sign-in using your own Lansary account. Approve research access; do not add shared authentication headers.

Alternatively, connect directly without installing the package:

```sh
claude mcp add --transport http lansary https://mcp.lansary.com/mcp/research
```

Then start Claude Code and use `/mcp` to authenticate.

## Codex and supported ChatGPT desktop surfaces

Add the marketplace using the Codex CLI:

```sh
codex plugin marketplace add lansary-intelligence/lansary-plugin
```

Open the desktop Plugins directory, select **Lansary Public Beta**, install **Lansary** and complete its OAuth connection. Restart or refresh the client if it does not show the new marketplace.

This is a repository marketplace, separate from the universal public plugin directory. Adding it does not grant platform approval or make the plugin available on every surface. Use the main ChatGPT guide for a direct web connection.

## Package contents

- `plugin.json`: portable plugin identity and public metadata.
- `mcp.json`: hosted Streamable HTTP server and OAuth registration settings.
- `.mcp.json` and `.claude-plugin/`: Claude-compatible connection and marketplace metadata.
- `.agents/plugins/marketplace.json`: marketplace metadata for compatible OpenAI clients.

These files contain no application code, backend deployment, database connection, API key, OAuth client secret or customer token. OAuth registration and user consent happen through the hosted service.

## Official references

- [OpenAI: package and distribute plugins](https://developers.openai.com/plugins/build/plugins).
- [Anthropic: create a plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces).
- [Anthropic: connect Claude Code to remote MCP servers](https://code.claude.com/docs/en/mcp).
