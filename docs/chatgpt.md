# Install Lansary in ChatGPT

**Public beta.** A custom connection is separate from an official directory listing. Access depends on your ChatGPT plan, workspace settings and permissions.

## Before you start

- Use [ChatGPT on the web](https://chatgpt.com/).
- [Create or sign in to your Lansary account](https://mcp.lansary.com/signup).
- Use the same Lansary email if you also connect Claude.

## Add the custom connection

The current OpenAI documentation describes this flow:

1. Open **Plugins** in ChatGPT.
2. Select the **plus** button, then **Add custom MCP server**.
3. Enter **Lansary** as the name.
4. Enter this exact server URL:

   ```text
   https://mcp.lansary.com/mcp/research
   ```

5. Select **OAuth** authentication.
6. Review the connection notice, then select **Create as a plugin**.
7. Complete the Lansary sign-in flow. Choose **Create an account or sign in with email** if offered, enter your own email and verify the one-time code.
8. Approve the `company:research` scope. If a scope field is shown during setup, use that value.
9. Find Lansary in your **personal plugins** and install it using the **plus** button.

Allow the client to discover the server's OAuth settings. Do not paste passwords, sign-in codes or bearer tokens into server settings, and do not use another customer's credentials. If your workspace requires a manually registered OAuth client, contact [Lansary support](https://mcp.lansary.com/support) instead of inventing a client ID or secret.

Some ChatGPT interfaces still use **Apps**, **Connectors** or **Developer mode** labels. Follow your account's custom MCP setup and use the same server URL and OAuth authentication. If no custom connection option is available, ask your workspace administrator or check current OpenAI access requirements.

## Use Lansary

1. Open a new **Work** chat where that surface is available.
2. Type `@` and select **Lansary**, or select it through the app/plugin picker your interface provides.
3. Ask:

   > Use Lansary to research Sheffield Forgemasters International Limited, company number 04883675. Confirm the legal entity and cite source dates and financial reporting periods.

4. Check that Lansary was actually invoked and the response includes attributed company evidence. A normal web-search answer alone does not establish a working Lansary connection.

Your first request for a new company's evidence can use one of your five monthly company briefs.

## Troubleshooting

| Problem | Next step |
| --- | --- |
| No custom MCP option | Check your platform plan and workspace permissions. Creating a Lansary account does not enable a restricted ChatGPT feature. |
| Sign-in fails or expires | Reconnect through OAuth using your own Lansary email. Never share the one-time code in GitHub issues. |
| ChatGPT does not call Lansary | Select or mention Lansary explicitly in a new chat. |
| A browser visit to the MCP URL returns an error | The URL is a protocol endpoint, not a website. Add it through the custom MCP setup. |
| The free allowance is exhausted | Check your Lansary account and the UTC-month reset. Creating extra accounts is not a workaround. |
| Client ID or secret is required unexpectedly | Use automatic registration/discovery where supported, or contact support. No shared credentials are published here. |

To disconnect, remove or disconnect Lansary in ChatGPT. Signing out of the Lansary website does not disconnect your assistant.

## Official references

Interface labels may change. These guides were prepared on 15 October 2026.

- [OpenAI: connect an MCP server and test a personal plugin](https://developers.openai.com/plugins/quickstart).
- [OpenAI: custom MCP servers](https://developers.openai.com/api/docs/guides/custom-mcp-server).
- [Lansary: hosted connection guide](https://mcp.lansary.com/directory).
