# Skill and Workflow Examples

Hermes use cases can include reusable skill patterns when they are public-safe. The goal is to publish the reusable operating pattern, not a private runtime dump.

## Good examples

- Notion API automation cheat sheets
- Google Workspace CLI workflows
- checkpoint and resume patterns for long conversations
- research summary templates

## Example package shape

A useful public skill package normally includes:

1. **Purpose** — what the workflow helps a person do.
2. **Setup assumptions** — required CLI, account, or API access, written generically.
3. **Common operations** — small commands or pseudocode that readers can adapt.
4. **Approval boundary** — which actions are read-only, which are writes, and which require human review.
5. **Validation step** — a smoke test, link check, or dry run that proves the workflow is safe to reuse.

## Reader path

Start with a small read-only example, then add write operations only after the approval boundary is clear. For example:

- search or list records
- fetch one item by id
- draft a change locally
- ask for approval before writing remotely
- verify the result with the smallest meaningful check

## Do not publish

- personal finance automations
- raw runtime skills with private channel IDs
- hotpatches tied to one local installation
- internal agents that encode private operational policy
- raw browser profiles, cookies, saved sessions, or local-only credentials
