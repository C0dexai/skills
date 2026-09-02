# AI-INTEL Capabilities

Installable Codex plugin containing governed Agent Skills for the AI-INTEL and NET2OOLS platform.

## Included skills

- `ai-intel-connection-binding` — resolve approved services, routes, authentication, health, and governance.
- `provider-health` — verify model-provider availability without invoking inference.
- `mcp-discovery` — inspect MCP servers and tool contracts safely.
- `network-diagnostics` — perform evidence-based DNS, route, port, and reachability checks.
- `apex-debugger` — diagnose APEX Debugger UI, toolchain, streaming, and ESM-to-NIM failures.
- `event-streaming` — design and verify normalized SSE/WebSocket event flows.
- `openclaw-operations` — inspect and operate OpenClaw with narrow tools and explicit approvals.
- `docker-inspect` — inspect Docker state without granting unrestricted daemon control.

Each skill keeps discovery and read-only diagnosis separate from mutations. Policy-gated operations must use the AI-INTEL binding and approval workflow.
