---
name: network-diagnostics
description: Diagnose DNS, routing, interfaces, ports, TLS, proxies, tunnels, and service reachability for AI-INTEL and NET2OOLS using non-destructive evidence.
---

# Network Diagnostics

Start with read-only checks appropriate to the executing environment.

- Identify Windows, WSL, Linux, container, or remote context before interpreting addresses.
- Check name resolution, route selection, listening sockets, TCP reachability, HTTP/TLS behavior, and proxy or tunnel status in that order when relevant.
- Separate host-local, WSL NAT, container bridge, LAN, and public addresses.
- Preserve timestamps and the exact target tested.
- Do not scan broad networks, change firewall rules, restart services, or alter DNS without explicit authorization.

Lead with the observed cause or narrowest hypothesis. Provide commands that expose no secrets and define the expected pass condition for each next check.
