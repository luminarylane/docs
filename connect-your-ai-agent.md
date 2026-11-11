# Connect your AI agent

If you already work with a personal AI agent, you can connect it to Lane. Your agent becomes the remote control: you ask it about your brands, and it reads from Lane and makes edits there. Lane keeps running your marketing in its own cloud, and **every approval stays with you, in the app.**

## What you need

- A Lane account with at least one brand.
- An AI agent that lets you add connectors, which are extra tools you point it at (this works through a standard called MCP). We have tested **Claude**, **ChatGPT**, **Hermes**, **Grok** and **Gemini**; see the guide for yours below.
- Lane's connector address:

```
https://mcp.luminarylane.app/mcp
```

## Guides

- [Claude](connect-claude.md) — add Lane as a custom connector
- [ChatGPT](connect-chatgpt.md) — add Lane as a custom connector
- [Hermes](connect-hermes.md) — add Lane from the command line
- [Grok](connect-grok.md) — add Lane as a custom connector
- [Gemini](connect-gemini.md) — add Lane as a custom connected app

We list an agent only after we have tested it, and we add more as they pass.

## How connecting works

1. You add Lane to your agent using the address above.
2. You sign in to your Lane account.
3. Lane shows you one approval page: **who is asking to connect** and **exactly where the sign-in will be sent back to**. Nothing is shared until you press **Allow**. If you did not start the connection yourself, press **Cancel**.

<!-- TODO(screenshot): the approval page, taken on a test brand -->

The name an app shows on that page is chosen by the app itself, so check the address it sends you back to as well.

## What your agent can do

- List the brands on your account and read a brand's setup: foundation, voice, objectives, personas, competitors and market events.
- Read Lane's status, plans and recent cycles, and see what is waiting for you.
- Make edits directly, such as updating a persona, your brand voice, competitor notes and guardrails, your goals and which goals Lane includes in its plan, or the wording of a draft that is waiting for you. **These edits apply immediately and replace what was there.** Lane does not keep earlier versions of your brand setup, so check what your agent changed.
- Add LinkedIn connections to your network and submit opportunity blurbs.

## What stays with you

Your agent **cannot** approve, publish, send, spend or delete anything, change your budgets or Lane's run settings, or choose who an outreach email goes to. The tools that do those things are not even visible to a connected agent. Nothing is published, sent or spent until you approve it in the **Lane Actions queue** in the app.

## What to grant, and what not to

- Connect with the sign-in above. Do not paste Lane API keys into a chat with an agent.
- Connect only agents you trust with your brand information. What your agent reads from Lane becomes part of your conversation with it, so your agent provider's own terms and privacy policy apply to it.
- Because edits apply immediately, turn on your agent's "ask before changing things" setting if it has one. Most agents let you set this per connector.
- Check the name and address on the approval page every time.

## Troubleshooting

- **The approval page says "This link did not work" and mentions cookies.** Lane needs to see the same browser window you started in. Use that window, make sure cookies are allowed for the site (private windows and in-app browsers often block them), and start the connection again.
- **"This link has expired."** The approval page is valid for 10 minutes. Start the connection again from your agent.
- **The Allow button does not respond straight away.** It becomes active after about a second. This is on purpose, so a stray click cannot approve a connection.
- **An older connector stopped working.** Connectors created before 9 November 2026 need to be removed and added again once.
- **Your agent says it cannot do something.** If it is approving, publishing, sending or spending, that is by design. Do it in the Lane Actions queue in the app.
- **Your agent does not see Lane's tools.** Check the connector is enabled for the conversation, then see the guide for your agent.

## Disconnecting

Remove the Lane connector in your agent's settings. Your agent then drops its sign-in and stops working with Lane. A sign-in the agent already holds can keep working until it expires, so if you need access ended right away, email **support@luminarylane.app**.
