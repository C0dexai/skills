---
name: ai-intel-connection-binding
description: Resolve AI-INTEL and NET2OOLS service intents to registered URLs, routes, authentication, health checks, risk classes, and CAM/AEGIS approval requirements before connecting or executing.
---

# AI-INTEL Connection Binding

Resolve the requested capability before any service connection or mutation.

1. Identify the service, operation, environment, and target stage.
2. Resolve the service only from the maintained service registry or a verified service contract. Never invent a hostname, route, port, credential, or fallback.
3. Use a local URL only when the worker is verified on the service host; otherwise use the registered public HTTPS URL.
4. Verify the registered health endpoint before publish, mutation, deployment, destructive, or privileged operations.
5. Apply the registered authentication method without exposing credentials.
6. Classify approval as `none`, `policy`, `operator`, or `cam-and-operator`.
7. Stop when identity, route, environment, authorization, or readiness is unresolved.

Report the service ID, exact endpoint, method, operation class, authentication type, health result, approval requirement, correlation ID, and one execution status: `NOT EXECUTED`, `BLOCKED`, `AUTHORIZED`, `EXECUTED AND VERIFIED`, `EXECUTED, VERIFICATION FAILED`, or `ROLLED BACK`.

A successful health check proves readiness, not authorization. A prior approval does not authorize a new correlation ID or parameter set.
