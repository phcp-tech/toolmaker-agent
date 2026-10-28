## Toolmaker Agent v0.1.2

### Changes

- **Free Edition: up to 3 products.** The product limit per organization is raised from 2 to 3.
- **New default port: 28080.** The web UI, REST API and MCP server now listen on port `28080` instead of `8080`, so Toolmaker Agent no longer clashes with the many developer tools that use `8080`. See [Upgrading](#upgrading-the-mcp-configuration) below.
- **New links in Settings.** The Settings page of the web UI now has **Docs**, **Terms of Service** and **Privacy Policy** entries. Each one opens the matching page on toolmaker.io in a new tab, in the language the UI is currently set to.

### Upgrading the MCP configuration

The MCP address changes from `http://127.0.0.1:8080/agtapi/v2/mcp` to `http://127.0.0.1:28080/agtapi/v2/mcp`. If you registered the old address, remove it and add the new one.

Open the web UI at `http://localhost:28080` from now on.

**Claude Code**

```bash
claude mcp remove toolmaker-agent -s user
claude mcp add --scope user --transport http toolmaker-agent http://127.0.0.1:28080/agtapi/v2/mcp
```

**Codex**

```bash
codex mcp remove toolmaker-agent
codex mcp add toolmaker-agent --url http://127.0.0.1:28080/agtapi/v2/mcp
```

Other MCP clients: change the URL in their configuration to the new address.

### Free Edition

- For local use by a single person only.
- Up to 3 products per organization.
