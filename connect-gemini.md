# Connect Gemini

Add Lane to Gemini as a custom connected app, sign in, and approve the connection on one page. Read [Connect your AI agent](connect-your-ai-agent.md) first for what your agent can and cannot do.

## Before you start

- Custom connected apps in Gemini depend on your Google account, your plan and your workspace settings. On a work or school account an admin may need to allow them. These rules change, so check Google's own Gemini help for where custom apps are available to you.
- Lane's address:

```
https://mcp.luminarylane.app/mcp
```

## Steps

1. In Gemini, open **Connected Apps** and choose to add a custom app (**Custom**). Menu names change, so follow Google's own help if yours differ.
2. In **Connect to an MCP server**, paste Lane's address into **MCP Server URL** and choose **Next**.
3. Gemini opens Lane's sign-in. Sign in to your Lane account.
4. On the approval page, check the name and the address it sends you back to (for Gemini this is an `oauth-redirect.googleusercontent.com` address, ending in an id that is unique to your connector), wait a second for **Allow** to become active, and press **Allow**.
5. Back in Gemini, ask something like "List my brands in Lane."

<!-- TODO(screenshot): Gemini's Connect to an MCP server dialog with Lane's address -->
<!-- TODO(screenshot): the approval page showing a googleusercontent.com address -->
<!-- TODO(screenshot): Gemini listing brands from a test brand -->

## Good to know

- Gemini sets itself up with Lane automatically. You do not need to enter a client ID or a client secret.
- **Each Gemini connector has its own address that it sends you back to.** That is why the approval page shows the full address, including the id at the end. If you did not just add that connector yourself, press **Cancel**.
- Gemini shows a notice that a custom connected app has not been reviewed by Google. That is Google's standard notice for any custom app: connect only what you trust.

## Troubleshooting

See [Connect your AI agent](connect-your-ai-agent.md#troubleshooting). If Gemini says "Automatic registration with this server failed" and asks for a client ID and secret, remove the connector and add it again as a new one. If it still asks, email support@luminarylane.app.
