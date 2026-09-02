---
name: openclaw-operations
description: Inspect, configure, secure, and troubleshoot an existing OpenClaw or NemoClaw gateway and its MCP connections without creating duplicate instances.
---

# OpenClaw Operations

Identify the authoritative installation, host or WSL distribution, process manager, configuration path, gateway listener, and current MCP registry before changing anything.

- Prefer status, doctor, probe, configuration lookup, and security audit operations first.
- Distinguish OpenClaw acting as an MCP server from its outbound MCP client registry.
- Keep the gateway on loopback or a private interface behind an authenticated proxy.
- Allow only narrow tools and sandbox mounts; do not expose home directories, credential stores, system paths, or the Docker socket.
- Require binding and approval for AI-INTEL MCP tool execution.
- Stop before reinstalling, resetting, rotating credentials, or starting a second gateway unless explicitly authorized.

After proxy or tool changes, verify authorized access, denied unauthorized access, redacted logs, intended agent routing, and approval behavior for high-impact tools.
