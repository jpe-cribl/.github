# jpe-cribl

jpe-cribl holds a Cribl Stream pack template and packs for collecting host
metrics and internal telemetry.

## Shared CI and releases

- Reuse workflows from `JacobPEvans/.github` and `JacobPEvans/.github-ai`.
  Reference both at `@v1`; never pin them to a commit SHA.
- Keep organization-managed CI and release steps in the reusable workflows.
  Local workflow files should call the shared implementation with repository
  specific inputs.
- Give each repository exactly one `release.yml` caller for its release
  workflow.
- Configure Renovate to extend only `github>JacobPEvans/.github`.
- Enterprise rulesets inject required checks. Do not add repository copies of
  shared checks.

## Domain conventions

- Keep generic pack scaffolding in `cc-stream-pack-template`; route changes to
  shared pack files through that template.
- Let Release Please propose pack versions. Do not create version tags by hand.
- Keep workflow logic out of inline scripts. Use script files or maintained
  community actions for steps that need scripting.

### Pack file ownership

- Make generic pack-file changes in the template and propagate them through
  template maintenance.
- Keep pack-specific behavior and configuration in each pack repository.

## Repository map

| Repository | Purpose |
| --- | --- |
| `cc-stream-pack-template` | Pack template with container e2e tests |
| `cc-stream-apple-mlx-metrics` | Cribl Stream pack for Apple MLX host metrics |
| `cc-stream-cribl-internal-telemetry` | Cribl internal telemetry pack |
| `cc-stream-cribl-edge-host-metrics` | Cribl Edge host metrics pack |
| `.github` | Organization profile |
