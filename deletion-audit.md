# cleanup-drill — Deletion Audit

- **Repository:** cleanup-drill (https://github.com/mcpmark-eval-liuhezi/cleanup-drill)
- **Removed path:** configs/legacy-config.yaml
- **Deletion commit (full SHA):** 7a5eba0078a971e588196a08cca998e41ea3abed
- **Commit message:** chore: remove legacy config
- **README.md sha256 (tip of default branch, post-cleanup):** af3ea1d57afe4806daa6f24aad722646b8101008cc58d8e4471aacfb82e7147e

## Verification (fresh anonymous clone of the repository)

- Working-tree check: PASSED — configs/legacy-config.yaml (and the empty configs/ directory) are absent from the working tree of a fresh clone; README.md is the only tracked file.
- History check: PASSED — commit 7a5eba0078a971e588196a08cca998e41ea3abed with message "chore: remove legacy config" is present in the cloned history and is the tip of the default branch (short SHA 7a5eba0).

## Pre-deletion read-back

File was read back from the repository before deletion and matched the committed content exactly:

```
# legacy service config
deprecated: true
removal_ticket: OPS-142
```

## Publication note

This audit was intended to be published as a gist (file `deletion-audit.md`, description
"cleanup-drill deletion audit") on the account HeziLiu. That was not possible: the
personal access token in use returns `403 Resource not accessible by personal access
token` for gist creation (both public and secret variants), i.e. it lacks gist scope.
The token also cannot create repositories under the user account (same 403), which is
why the drill repository lives in the accessible organization mcpmark-eval-liuhezi
instead. This file is therefore published on the `audit` branch of this repository.
