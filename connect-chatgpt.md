# Connect ChatGPT

Add Lane to ChatGPT as a custom connector, sign in, and approve the connection on one page. Read [Connect your AI agent](connect-your-ai-agent.md) first for what your agent can and cannot do.

## Before you start

- Custom connectors in ChatGPT depend on your plan and your workspace settings, and in a team workspace an admin may need to add them. These rules change, so check OpenAI's own guide: [OpenAI's guide to adding custom connectors in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt).
- Lane's address:

```
https://mcp.luminarylane.app/mcp
```

## Steps

1. In ChatGPT, open the settings where you add connectors or MCP servers and choose to create a new one. Menu names change, so follow OpenAI's guide above if yours differ.
2. Name it **Luminary Lane**, paste Lane's address, and choose **OAuth** (the sign-in option) if it asks how to authenticate.
3. Connect. ChatGPT opens Lane's sign-in. Sign in to your Lane account.
4. On the approval page, check the name and the address it sends you back to (for ChatGPT this is a `chatgpt.com` address, usually ending in an id that is unique to your connector), wait a second for **Allow** to become active, and press **Allow**.
5. Back in ChatGPT, ask something like "List my brands in Lane."

<!-- TODO(screenshot): ChatGPT's create-connector form with Lane's address -->
<!-- TODO(screenshot): the approval page showing a chatgpt.com address -->
<!-- TODO(screenshot): ChatGPT listing brands from a test brand -->

## Good to know

- **Each ChatGPT connector has its own address that it sends you back to.** That is why the approval page shows the full address, including the id at the end. If you did not just create that connector yourself, press **Cancel**.
- You do not need to ask us to set anything up for a new connector.

## Troubleshooting

See [Connect your AI agent](connect-your-ai-agent.md#troubleshooting). If ChatGPT cannot connect, delete the connector and create it again as a new one.
