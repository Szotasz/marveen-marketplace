# Marveen Marketplace

Channel plugin registry for the [Marveen](https://github.com/Szotasz/marveen) agent fleet (ClaudeClaw).

Currently lists:

- `slack-channel` — [jeremylongshore/claude-code-slack-channel](https://github.com/jeremylongshore/claude-code-slack-channel)

## Install

```bash
claude plugin marketplace add Szotasz/marveen-marketplace
claude plugin install slack-channel@marveen-marketplace
```

Then start Claude Code with:

```bash
claude --channels plugin:slack-channel@marveen-marketplace --dangerously-load-development-channels
```

The `--dangerously-load-development-channels` flag is required because the Slack plugin is not on the official Anthropic-approved channels allowlist yet.
