# Cribl 🦑

**Logs go in, insights come out, and nobody's pipeline gets Cribl'd.**
Cribl Stream packs for shaping telemetry: less noise, more signal, smaller
bills.

## Start here

| Repository | What it does |
| --- | --- |
| [`cc-stream-pack-template`](https://github.com/jpe-cribl/cc-stream-pack-template) | Cribl Stream template for real-container E2E tests. Clone, tweak, ship. |
| [`cc-stream-apple-mlx-metrics`](https://github.com/jpe-cribl/cc-stream-apple-mlx-metrics) | Cribl Stream pack: Apple MLX host metrics. |
| [`cc-stream-cribl-internal-telemetry`](https://github.com/jpe-cribl/cc-stream-cribl-internal-telemetry) | Cribl internal telemetry. Cribl, watching Cribl. |
| [`cc-stream-cribl-edge-host-metrics`](https://github.com/jpe-cribl/cc-stream-cribl-edge-host-metrics) | Cribl Stream pack: Cribl Edge host metrics. |

Cribl Notes (the short version) live at
[docs.jacobpevans.com](https://docs.jacobpevans.com).

## The family 👪

- [dryvist](https://github.com/dryvist) (infrastructure as code-medy)
- [Jacob's Splunk Dump](https://github.com/jpe-splunk)
  (a well-organized dump)
- [Ansible Collections](https://github.com/jpe-ansible)
  (playbooks, not play-by-ear)
- [Jacob's OpenBao Secrets Plugins][openbao] (Bao-nus secrets)
- [VCT Cribl](https://github.com/vct-cribl) (Edge-ucation)
- [VCT Splunk](https://github.com/vct-splunk) (Splunk it like it's hot)
- [JacobPEvans HQ](https://github.com/JacobPEvans) (the front door)

[openbao]: https://github.com/jpe-openbao-plugin-secrets

<!-- org-index:start -->
## Repositories

### Other

- [.github](https://github.com/jpe-cribl/.github): Organization profile
- [cc-edge-ai-transcript-shared-io](https://github.com/jpe-cribl/cc-edge-ai-transcript-shared-io): Cribl Edge pack: shared AI CLI log breaker and masking
  pipeline (topics: ai, cribl, cribl-edge, cribl-pack)
- [cc-edge-claude-code-io](https://github.com/jpe-cribl/cc-edge-claude-code-io): Collects Claude Code telemetry from OpenTelemetry and/or session log sources
  via Cribl Edge, then forwards it to a Cribl Stream worker group for indexing, analysis, and search.
- [cc-edge-codex-io](https://github.com/jpe-cribl/cc-edge-codex-io): Cribl Edge pack: OpenAI Codex CLI session transcript ingestion
- [cc-edge-macos-diagnostic-reports-io](https://github.com/jpe-cribl/cc-edge-macos-diagnostic-reports-io): Cribl Edge pack: macOS crash, hang and diagnostic
  reports (topics: cribl, cribl-edge, cribl-pack, macos)
- [cc-edge-macos-firewall-io](https://github.com/jpe-cribl/cc-edge-macos-firewall-io): Cribl Edge pack: macOS firewall logs (topics: cribl, cribl-edge,
  cribl-pack, macos)
- [cc-edge-macos-power-thermal-io](https://github.com/jpe-cribl/cc-edge-macos-power-thermal-io): Cribl Edge pack: macOS power, wired memory and thermal
  metrics (topics: cribl, cribl-edge, cribl-pack, macos)
- [cc-edge-macos-process-telemetry-io](https://github.com/jpe-cribl/cc-edge-macos-process-telemetry-io): Cribl Edge pack: macOS process lifecycle and
  per-process telemetry (topics: cribl, cribl-edge, cribl-pack, macos)
- [cc-edge-macos-unified-logs-io](https://github.com/jpe-cribl/cc-edge-macos-unified-logs-io): Cribl Edge pack: macOS unified log processing (topics: cribl,
  cribl-edge, cribl-pack, macos)
- [cc-edge-macos-ws-monitor-io](https://github.com/jpe-cribl/cc-edge-macos-ws-monitor-io): Cribl Edge pack: macOS window-server stall monitor samples and
  captures (topics: cribl, cribl-edge, cribl-pack, macos)
- [cc-edge-mlx-serving-io](https://github.com/jpe-cribl/cc-edge-mlx-serving-io): Cribl Edge pack: local MLX model serving logs and metrics (topics: cribl,
  cribl-edge, cribl-pack, mlx)
- [cc-edge-pack-template](https://github.com/jpe-cribl/cc-edge-pack-template): Template repo for dryvist Cribl packs - reusable test/release workflows and
  scaffolding
- [cc-stream-apple-mlx-metrics](https://github.com/jpe-cribl/cc-stream-apple-mlx-metrics): Cribl Stream pack: Apple MLX host metrics (topics: cribl,
  cribl-pack)
- [cc-stream-cribl-edge-host-metrics](https://github.com/jpe-cribl/cc-stream-cribl-edge-host-metrics): Cribl Stream pack: Cribl Edge host metrics (topics:
  cribl, cribl-pack)
- [cc-stream-cribl-internal-telemetry](https://github.com/jpe-cribl/cc-stream-cribl-internal-telemetry): Cribl Stream pack: Cribl internal telemetry (topics:
  cribl, cribl-pack)
- [cc-stream-macos-fanout-io](https://github.com/jpe-cribl/cc-stream-macos-fanout-io): —
- [cc-stream-openrouter-rest-io](https://github.com/jpe-cribl/cc-stream-openrouter-rest-io): —
- [cc-stream-pack-template](https://github.com/jpe-cribl/cc-stream-pack-template): Template for Cribl Stream packs with real-container e2e testing
- [cc-stream-secret-redaction-io](https://github.com/jpe-cribl/cc-stream-secret-redaction-io): Cribl Stream pack that masks credential patterns out of events,
  attached as a destination post-processing pipeline (topics: cribl, cribl-pack, cribl-stream, data-masking, log-management, observability, redaction,
  security)

## Archived repositories (1)

### Other (archived)

- [cc-edge-the-mac-pack-io](https://github.com/jpe-cribl/cc-edge-the-mac-pack-io): Cribl Edge Pack for macOS system health monitoring and anomaly detection —
  the TA-nix equivalent for macOS via Cribl Edge
<!-- org-index:end -->
