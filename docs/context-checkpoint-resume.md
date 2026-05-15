# Context Checkpoint and Resume

Long AI conversations need safe reset and resume patterns. Hermes and OpenClaw both benefit from the same lightweight handoff structure.

## Prepare before reset

Record only what is needed to resume:

- current objective
- last completed step
- important decisions
- open blockers
- next one to three actions
- exact file or wiki pointer to read after reset

## Resume after reset

1. Read the checkpoint.
2. Verify live repo/runtime state.
3. Continue from the next concrete action.
4. Ask before risky actions such as updates, restarts, destructive cleanup, or external publishing.

## Why it matters

The goal is not to preserve every chat token. The goal is to preserve enough state that the next operator turn can act safely without replaying the whole conversation.
