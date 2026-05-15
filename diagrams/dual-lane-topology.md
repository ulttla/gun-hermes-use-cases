# Dual-Lane Topology

```mermaid
flowchart LR
  Human[Human approval] --> OpenClaw[OpenClaw / NOVA]
  Human --> Hermes[Hermes]
  OpenClaw <--> Wiki[gun-wiki shared brain]
  Hermes <--> Wiki
  OpenClaw -. audit / recovery .-> Hermes
  Hermes -. audit / recovery .-> OpenClaw
  Wiki --> Public[Public-safe GitHub / portfolio summaries]
```
