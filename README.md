# .github

Organization profile

## Shared pack CI

### Test

`cribl-pack-test.yml` validates pack structure and runs the Cribl pipeline test matrix.

- `pack_type`: required; `edge` or `stream`.
- `cribl_versions`: JSON version matrix; defaults to `latest` (required), `4.17.1` (optional), and `4.16.1` (optional).
- `node_version`: defaults to `lts/*`.
- `yq_version`: defaults to `4.44.5`.

Caller job:

```yaml
jobs:
  pack-test:
    uses: jpe-cribl/.github/.github/workflows/cribl-pack-test.yml@<40-hex commit SHA> # main
    with:
      pack_type: edge
```

### Release

`cribl-pack-release.yml` builds `.crbl` archives and uploads them to a draft release.

- `additional_files`: optional space-separated paths; defaults to empty.
- `tag`: draft release tag; defaults to the caller's `github.ref_name`.

Caller job:

```yaml
jobs:
  release:
    uses: jpe-cribl/.github/.github/workflows/cribl-pack-release.yml@<40-hex commit SHA> # main
```

### End-to-end

`cribl-pack-e2e.yml` checks out the caller pack and runs `e2e/run.ts` with Node.js 24. It has no inputs. The caller keeps these triggers:

```yaml
on:
  workflow_dispatch:
  pull_request:
    paths:
      - 'e2e/**'
      - '.github/workflows/e2e.yml'

permissions:
  contents: read

jobs:
  e2e:
    uses: jpe-cribl/.github/.github/workflows/cribl-pack-e2e.yml@<40-hex commit SHA> # main
```
