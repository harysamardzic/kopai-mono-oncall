# Kopai Dev

A Claude plugin for building with Kopai: instrument applications with
OpenTelemetry, prove the telemetry is good against a local Kopai, and
build Kopai dashboards.

| Skill                  | What it does                                                                                  |
| ---------------------- | --------------------------------------------------------------------------------------------- |
| `otel-instrumentation` | Adds OpenTelemetry to an app in any of a dozen languages and validates the data against Kopai |
| `create-dashboard`     | Builds Kopai dashboards from time-series, stat, histogram, log and trace tiles                |

The plugin declares the Kopai MCP server (`https://api.kopai.app/v2/mcp`).
For a local Kopai (`npx @kopai/app start`), the MCP endpoint is
`http://localhost:8000/mcp`.

## Install in Claude Code

```bash
claude plugin marketplace add kopai-app/kopai-mono
claude plugin install kopai-dev@kopai
```

For incident response, use the `kopai-oncall` plugin instead.

These skills are generated from the repository's top-level `skills/`
folder by `scripts/sync-plugin-skills.mjs`. Edit them there.
