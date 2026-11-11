# Connect Grok

Add Lane to Grok as a custom connector, sign in, and approve the connection on one page. Read [Connect your AI agent](connect-your-ai-agent.md) first for what your agent can and cannot do.

## Before you start

- Custom connectors in Grok depend on your plan and your workspace settings. On Business and Enterprise plans a team admin may need to add the connector first. These rules change, so check xAI's own guide: [xAI's guide to Grok connectors](https://docs.x.ai/grok/connectors).
- Lane's address:

```
https://mcp.luminarylane.app/mcp
```

## Steps

1. In Grok, open **Connectors** and choose **New Connector**. Menu names change, so follow xAI's guide above if yours differ.
2. Choose **Custom**, then paste Lane's address.
3. Grok opens Lane's sign-in. Sign in to your Lane account.
4. On the approval page, check the name and the address it sends you back to (for Grok this is a `grok.com` address), wait a second for **Allow** to become active, and press **Allow**.
5. Back in Grok, ask something like "List my brands in Lane."

<!-- TODO(screenshot): Grok's New Connector form with Lane's address -->
<!-- TODO(screenshot): the approval page showing a grok.com address -->
<!-- TODO(screenshot): Grok listing brands from a test brand -->

## Good to know

- Grok sets itself up with Lane automatically. You do not need to enter a client ID or a client secret, and you do not need to ask us to set anything up.
- If you did not just add that connector yourself, press **Cancel** on the approval page.

## Troubleshooting

See [Connect your AI agent](connect-your-ai-agent.md#troubleshooting). If Grok cannot connect, remove the connector and add it again as a new one.
