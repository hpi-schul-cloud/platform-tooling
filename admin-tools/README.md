# admin-tools

Operator-focused image for diagnostics and manual maintenance tasks.

Included tools:
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

Contract:
- runs as non-root
- broader than `job-tools`, but still intentionally curated
- suitable for interactive troubleshooting and maintenance jobs
- not the default base for automated workloads
