# Davidson T&I Plugin Marketplace

Official Claude Code plugin marketplace for Davidson College Technology & Innovation. This marketplace distributes curated plugins for IT operations, procurement, and campus technology management.

## Installation

### Claude Code (CLI)

1. Add the marketplace:

```shell
/plugin marketplace add DavidsonCollege/davidson-ti-plugins
```

2. Install a plugin:

```shell
/plugin install <plugin-name>@davidson-ti-plugins
```

### Claude Desktop (Cowork)

Cowork is available in the [Claude Desktop app](https://claude.com/download) for macOS and Windows. A paid Claude plan (Pro, Max, Team, or Enterprise) is required.

1. Open **Claude Desktop** and click the **Cowork** tab at the top of the window.
2. Click **Plugins** in the left sidebar.
3. Click the **+** button next to **Personal plugins** and select **Add marketplace from GitHub**.
4. Enter `DavidsonCollege/davidson-ti-plugins` and confirm.
5. Click the **Personal** tab in the **Browse plugins** dialog to see the marketplace and its plugins.
6. Click a plugin to install it.

## Available Plugins

### vendor-research (v0.3.0)

Comprehensive multi-agent vendor research toolkit for higher education IT procurement. Launches 7 parallel research agents and synthesizes findings into a professional Vendor Research Brief.

```shell
/plugin install vendor-research@davidson-ti-plugins
```

| Skill | Example Trigger |
|-------|----------------|
| vendor-research-coordinator | "Evaluate Zoom as a vendor" |
| vendor-security-review | "Run a security review of Okta" |
| vendor-reputation | "What's the reputation of ServiceNow?" |
| vendor-cost-analysis | "How much does Canva cost for higher ed?" |
| vendor-legal-contract | "Review the legal terms for Slack" |
| vendor-competitive-analysis | "Compare Monday.com to Asana" |
| vendor-higher-ed-fit | "Is Notion a good fit for higher ed?" |
| vendor-build-feasibility | "Could we build our own ticketing system?" |

## Adding New Plugins

To add a plugin to this marketplace, create a new entry in `.claude-plugin/marketplace.json` with the plugin's name, source repository, and metadata. See [Anthropic's plugin marketplace documentation](https://code.claude.com/docs/en/plugin-marketplaces) for the full schema.

## Updating

To pull the latest marketplace catalog:

```shell
/plugin marketplace update
```
