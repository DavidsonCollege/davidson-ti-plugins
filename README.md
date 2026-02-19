# Davidson T&I Plugin Marketplace

Official Claude Code plugin marketplace for Davidson College Technology & Innovation. This marketplace distributes curated plugins for IT operations, procurement, and campus technology management.

## Installation

### 1. Add the marketplace

```shell
/plugin marketplace add DavidsonCollege/davidson-ti-plugins
```

### 2. Browse and install plugins

```shell
/plugin install <plugin-name>@davidson-ti-plugins
```

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

## Private Repository Access

This is a private marketplace. To install plugins from it, you need Git credentials that can access the repository.

### For interactive use

Authenticate with the GitHub CLI:

```bash
gh auth login
```

### For background auto-updates

Set a GitHub token in your shell profile (~/.zshrc or ~/.bashrc):

```bash
export GITHUB_TOKEN=ghp_your_token_here
```

The token needs the `repo` scope to access private repositories.

## Adding New Plugins

To add a plugin to this marketplace, create a new entry in `.claude-plugin/marketplace.json` with the plugin's name, source repository, and metadata. See [Anthropic's plugin marketplace documentation](https://code.claude.com/docs/en/plugin-marketplaces) for the full schema.

## Updating

To pull the latest marketplace catalog:

```shell
/plugin marketplace update
```
