# job-tools

Minimal runtime image for automated operational jobs.

Included tools:
- `sh`
- `curl`
- `jq`
- `kubectl`
- `rclone`
- `ca-certificates`

Contract:
- runs as non-root
- suitable for Kubernetes `Job` and `CronJob` usage
- intended to work with read-only root filesystems when `/tmp` is writable
- no debugging extras by default
