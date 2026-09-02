---
name: provider-health
description: Check AI model provider configuration, reachability, model discovery, and latency without running paid inference or changing provider state.
---

# Provider Health

Use the connection-binding skill before contacting an AI-INTEL provider.

- Confirm the configured provider identity and endpoint.
- Prefer its registered health or model-list route.
- Record DNS resolution, HTTP status, latency, response shape, and model count when available.
- Distinguish network failure, authentication failure, incompatible API shape, empty model inventory, and inference failure.
- Do not run inference merely to prove availability unless the user explicitly requests it.
- Never print API keys, bearer tokens, cookies, ADC tokens, or credential files.

Return a compact provider matrix with `verified`, `degraded`, `blocked`, or `unknown`, followed by the smallest next diagnostic step.
