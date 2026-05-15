# Dual-Lane Operating Model

The operating model is complementary: OpenClaw and Hermes can review and support each other while staying under human approval gates.

```text
OpenClaw / NOVA  <---->  gun-wiki shared brain  <---->  Hermes
primary operator          durable context          secondary operator
```

## Boundaries

- One lane owns the active user-facing work at a time.
- The other lane can audit, review, prepare recovery, or summarize evidence.
- Risky actions require explicit approval.
- Public artifacts receive sanitized summaries, not raw private logs.

## Why it works

A second operator is valuable when the primary runtime is degraded, the context has reset, or a risky change needs independent review. The shared brain prevents the two lanes from drifting into separate memory islands.
