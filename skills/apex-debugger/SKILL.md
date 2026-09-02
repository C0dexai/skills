---
name: apex-debugger
description: Diagnose and advance the AI-INTEL APEX Debugger page, toolchain detection, event streaming, and ESM build-to-NIM pipeline.
---

# APEX Debugger

Treat the debugger as an evidence surface spanning UI, build toolchain, event transport, and inference routing.

1. Reproduce the smallest failing path and capture its observable state.
2. Identify the boundary: page rendering, toolchain detection, build, event normalization, transport, gateway policy, or NIM inference.
3. Trace one correlation ID across browser, API, event stream, build worker, and provider when available.
4. Fix the earliest broken boundary rather than masking downstream symptoms.
5. Verify with a deterministic fixture and explicit pass criteria.

Keep these event families distinguishable: run lifecycle, build lifecycle, tool requests, approvals, content deltas, usage, completion, and failure. Never claim the ESM-to-NIM path works solely because the frontend build succeeds.
