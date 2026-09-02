---
name: event-streaming
description: Design, inspect, and verify normalized SSE or WebSocket event streams for AI-INTEL runs, tools, approvals, builds, and model output.
---

# Event Streaming

Choose SSE for ordered server-to-client run output unless bidirectional low-latency messaging is required; use WebSockets when both sides must publish during a session.

Define a stable envelope with event type, run ID, correlation ID, timestamp, source, sequence, and payload. Preserve provider-specific data only under a namespaced metadata field.

Verify:

- monotonic sequence ordering;
- reconnect behavior and replay boundary;
- heartbeat and idle timeout behavior;
- terminal completion or failure exactly once;
- cancellation propagation;
- proxy buffering disabled where required;
- secret and sensitive-data redaction.

Do not infer successful execution from a connected stream. Report transport health and run outcome separately.
