# Connect Hermes

Hermes is an agent you run yourself, so you add Lane from the command line. Read [Connect your AI agent](connect-your-ai-agent.md) first for what your agent can and cannot do.

## Before you start

- A working Hermes install with the `hermes` command available.
- Lane's address:

```
https://mcp.luminarylane.app/mcp
```

## Steps

1. Add Lane as an OAuth server:

   ```
   hermes mcp add lane --url https://mcp.luminarylane.app/mcp --auth oauth
   ```

2. Sign in. Run this from a **fresh terminal**, because the sign-in waits for you to finish in the browser:

   ```
   hermes mcp login lane
   ```

   Your browser opens Lane's sign-in. Sign in, then on the approval page check that it says it is an app on this computer, wait a second for **Allow** to become active, and press **Allow**.

3. Check the connection:

   ```
   hermes mcp test lane
   ```

   You should see Lane's tools listed.

4. Pick up the new connection in any Hermes session that was already running by running `/reload-mcp` in it, or restart the Hermes background service (the gateway). A session started before you signed in does not see the new tools until you do.

<!-- TODO(screenshot): terminal showing `hermes mcp test lane` listing tools (test brand, no secrets) -->
<!-- TODO(screenshot): the approval page for Hermes -->

## Good to know

- Hermes can ask before it uses tools that change things. In your Hermes configuration, set `trust: untrusted` on the `lane` server. Note that Hermes's auto-approve mode (YOLO) skips that question, and because Lane's edits apply immediately, leave it off when you use Lane.
- Lane's approval tools are not visible to a connected agent, so Hermes cannot approve, publish or send even if it is told to.

## Troubleshooting

See [Connect your AI agent](connect-your-ai-agent.md#troubleshooting). If Hermes does not show Lane's tools, or says it is not signed in to Lane, run `hermes mcp login lane` again. Then run `hermes mcp list` to check the server is enabled, `hermes mcp test lane`, and `/reload-mcp` in any session that was already running.
