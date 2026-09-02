---
name: mcp-discovery
description: Discover and inspect registered MCP servers, transports, tools, schemas, health, and governance without executing tools unless separately authorized.
---

# MCP Discovery

Use connection binding before contacting an AI-INTEL or NET2OOLS MCP service.

1. Resolve the MCP server and transport from an approved registry or supplied configuration.
2. Verify server identity and health.
3. List tools and read their descriptions and input schemas.
4. Classify each tool as read, inference, publish, mutation, deployment, destructive, or privileged.
5. Report authentication and approval requirements.

Discovery is not permission to execute. Never treat a health endpoint as a tool route, silently switch servers, or expose credentials. For tool calls, obtain the required AEGIS decision, operator approval, or CAM manifest immediately before execution.
