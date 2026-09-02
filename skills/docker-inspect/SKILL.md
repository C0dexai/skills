---
name: docker-inspect
description: Inspect Docker daemon, container, image, network, volume, Compose, port, log, and resource state without mutating workloads.
---

# Docker Inspect

Use the AI-INTEL connection binding when operating through Docker Forge or another registered service.

Prefer non-mutating commands and APIs: daemon info, list, inspect, stats, logs, Compose config, and port mappings. Identify the Docker context and daemon before interpreting results.

Report:

- container identity, image, state, health, restart policy, ports, networks, and mounts;
- recent relevant logs with secrets redacted;
- resource pressure and dependency failures;
- whether evidence is host-local, remote, or simulated.

Do not start, stop, restart, build, deploy, delete, prune, pull, or modify Compose state under this skill. Route those operations through the registered policy and approval workflow. Never grant an unrestricted agent access to `/var/run/docker.sock`.
