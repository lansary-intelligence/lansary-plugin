# Install Lansary in Claude

**Public beta.** This uses Claude's custom remote connector feature. You do not need a Lansary listing in the official Connectors Directory to add a custom connection.

## Before you start

- [Create or sign in to your Lansary account](https://mcp.lansary.com/signup).
- Use the same Lansary email as in ChatGPT to share your monthly allowance.
- Check whether your Claude account and workspace permit custom connectors. Anthropic currently documents support on Free, Pro, Max, Team and Enterprise; Free accounts are limited to one custom connector.

## Personal accounts

1. Open **Customize → Connectors** in Claude. Some versions place this under **Settings → Connectors**.
2. Select **+ Add → Add custom connector**.
3. Enter **Lansary** as the name.
4. Enter this exact remote MCP server URL:

   ```text
   https://mcp.lansary.com/mcp/research
   ```

5. Select **Continue** and review the detected authentication.
6. Keep **OAuth** sign-in. If an OAuth client option is shown, use the detected automatic/discovery settings where supported; do not supply a shared client secret. If manual client credentials are required, contact Lansary support.
7. Finish adding the connector and choose **Connect** or **Sign in now**, as offered.
8. On Lansary's sign-in page, choose **Create an account or sign in with email**, verify your own email and approve `company:research` access.
9. Open a conversation and enable Lansary from the **+ → Connectors** menu or the connector picker shown in your version.

For Claude Desktop and Cowork, use the remote connector through your Claude account. No local backend or database installation is needed.

## Team and Enterprise workspaces

An authorised owner or administrator must first add Lansary under **Organization settings → Connectors → Add → Custom → Web**. Enterprise may allow additional roles with the required connector-management permission.

Use the same URL and OAuth settings above. Once the connector is available to members, each customer connects with their own Lansary account. Do not configure a shared token that would give everyone the same customer access.

## Try it

> Use Lansary to trace Tidyco Limited's registered ownership chain. Cite the source for each available link and explain where the evidence stops.

Confirm that Claude called Lansary and returned attributed evidence. If it answers without using the connector, enable Lansary and ask again.

Opening evidence for a new company can use one of your five monthly company briefs.

## Troubleshooting

- **No custom connector option:** check your Claude plan and organisation permissions. Free accounts may need to remove an existing custom connector before adding another.
- **Authentication fails:** verify the server URL and reconnect using your own Lansary email. If OAuth registration fails, contact support; never paste a sign-in code or access token into an issue.
- **A browser visit to the MCP URL returns an error:** it is a protocol endpoint. Use the connector setup rather than the address bar.
- **Lansary is not being used:** enable it in the current conversation and name it explicitly in your request.
- **Company evidence is incomplete:** check the legal entity, source dates and available coverage. A missing record is an evidence gap.

Disconnect or remove Lansary in Claude to revoke the assistant connection. Signing out of the Lansary website does not disconnect Claude.

## Official references

Interface labels may change. These guides were prepared on 15 October 2026.

- [Anthropic: custom connectors using remote MCP](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp).
- [Anthropic: desktop and web connectors](https://support.claude.com/en/articles/11725091-when-to-use-desktop-and-web-connectors).
- [Lansary support](https://mcp.lansary.com/support).
