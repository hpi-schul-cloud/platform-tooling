# platform-tooling

Container images for shared operational tooling.

## Images

### `job-tools`

Security-focused base image for automated Kubernetes `Job` and `CronJob` workloads.

Current scope:
- Debian `stable-slim`
- non-root runtime user
- `sh`
- `curl`
- `jq`
- `rclone`
- `ca-certificates`

Non-goals:
- interactive debugging convenience
- broad operator toolbox
- language runtimes

### `admin-tools`

Broader operator-focused image for human-driven maintenance and diagnostics.

Current scope:
- Debian `stable-slim`
- non-root runtime user
- `sh`
- `curl`
- `jq`
- `rclone`
- `ca-certificates`
- `iputils-ping`
- `traceroute`
- `iproute2`
- `dnsutils`
- `netcat`

Non-goals:
- application runtimes
- package compilation toolchains
- becoming the default base for automated jobs

## Publishing

Intended registry layout:
- branch and PR builds: `ghcr.io`
- tags: `ghcr.io` and `quay.io`

Registry credentials and repository setup are intentionally not handled in this repo skeleton.
