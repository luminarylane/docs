# Connect Claude

Add Lane to Claude as a custom connector, sign in, and approve the connection on one page. Read [Connect your AI agent](connect-your-ai-agent.md) first for what your agent can and cannot do.

## Before you start

- Custom connectors depend on your Claude plan and workspace settings. On Team and Enterprise plans an admin may need to add the connector for the organization, and then each member signs in with their own account. See Claude's own guide: [Get started with custom connectors using remote MCP](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp).
- Lane's address:

```
https://mcp.luminarylane.app/mcp
```

## Steps

1. In Claude, open the connector settings and choose to add a custom connector. Menu names change, so follow Claude's guide above if yours differ.
2. Name it **Luminary Lane** and paste Lane's address.
3. Connect. Claude opens Lane's sign-in in your browser. Sign in to your Lane account.
4. On the approval page, check the name and the address it sends you back to (for Claude this is a `claude.ai` or `claude.com` address), wait a second for **Allow** to become active, and press **Allow**.
5. Back in Claude, ask something like "List my brands in Lane."

<!-- TODO(screenshot): Claude's add-custom-connector form with Lane's address -->
<!-- TODO(screenshot): the approval page showing a claude.ai address -->
<!-- TODO(screenshot): Claude listing brands from a test brand -->

## Good to know

- If your organization added the connector for everyone, each member still signs in and approves their own connection.

## Troubleshooting

See [Connect your AI agent](connect-your-ai-agent.md#troubleshooting). If Claude says the connector failed, remove it and add it again.
