# Four-Channel Separation

Hermes is easier to operate when work is separated by lane. Public docs describe the roles, not private channel names or IDs.

| Lane | Purpose | Public-safe description |
|---|---|---|
| Hermes development | Work on Hermes itself | configuration, behavior tuning, runtime hardening |
| OpenClaw recovery | Help when OpenClaw has issues | audit, rollback review, recovery evidence |
| Personal assistant | Everyday non-engineering tasks | listing drafts, copy review, personal workflows |
| Research | Focused investigation | source collection, summaries, handoff notes |

The separation reduces context bleed and makes it clearer which operator owns which work.

## Shared co-working lanes

The four Hermes lanes can also connect to shared OpenClaw/Hermes spaces:

| Shared lane | Purpose | Public-safe description |
|---|---|---|
| Knowledge co-working | gun-wiki digestion, retrieval checks, source-backed notes | Shared brain maintenance |
| General co-working | tasks where both operators add value | Bounded two-operator collaboration |

These shared lanes should still preserve ownership. OpenClaw should not mutate
Hermes runtime state without approval, and Hermes should not mutate OpenClaw
runtime state without approval. The shared value is context, review, and handoff
quality, not unchecked cross-control.
