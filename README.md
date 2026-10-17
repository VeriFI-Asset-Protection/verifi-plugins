# verifi

Connect to your VeriFi account. You sign in with your own VeriFi login and can only see and change what your VeriFi permissions allow. Every request is recorded in VeriFi's audit trail. Changes are confirmed with you first and nothing can be permanently deleted.
## Install

- **Claude (web, desktop, Cowork):** Customize › Plugins › Add › Add marketplace, enter `VeriFI-Asset-Protection/verifi-plugins`,
  install `verifi`, then open its Connectors tab and connect it, signing in to VeriFi.
- **Claude Code:**

```
/plugin marketplace add VeriFI-Asset-Protection/verifi-plugins
/plugin install verifi@verifi-plugins
```

## What it connects to

This plugin adds one remote MCP server, `https://vault.verifiassetprotection.com/mcp/v1`, run by VeriFi Asset Protection. Each person
signs in to VeriFi in their browser with OAuth; the plugin contains no passwords, keys or secrets. Your assistant
sends VeriFi the requests you ask it to make and receives the matching VeriFi records. The plugin itself fetches
nothing else. The tools each person sees depend on their VeriFi permissions.

## Skills

- `setup`: welcomes you after install, checks the connection works, and points your assistant at the VeriFi how-to guides your role can use.

## Support

https://www.veri.fi · Privacy policy: https://www.veri.fi/privacy-policy