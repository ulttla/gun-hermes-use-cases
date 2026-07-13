# Durable Kanban, Goals, and Scheduled Operations

## Why this lane exists

Some work should outlive one chat turn: scheduled briefs, research follow-ups, maintenance reviews, and goals that require evidence before completion.

The Hermes lane uses durable task state for this class of work while keeping risky actions human-approved.

## Current lab snapshot

Verified on 2026-07-12:

- Hermes Agent v0.18.2 stable release;
- Discord gateway operation with per-user session isolation;
- OpenAI Codex OAuth with a local GPT-5.6 Sol profile;
- active scheduled briefing and audit jobs;
- SQLite-backed Kanban boards for persistent task tracking;
- shared durable context through the wiki-first gun-wiki process.

This is a dated local lab snapshot, not a claim about Hermes defaults or every installation.

## Operating pattern

1. Use a short session for one-turn research or review.
2. Use a persistent goal when work spans turns and needs an explicit completion contract.
3. Use Kanban when ownership, status, restart recovery, or an audit trail matters.
4. Use scheduled jobs for time-based briefs or checks, with delivery and failure evidence.
5. Promote reusable results into the shared wiki; keep raw runtime state private.

## Completion evidence

A durable task should name:

- intended outcome;
- verification evidence;
- constraints and approval boundaries;
- stop condition;
- remaining blocker or next action.

Runtime updates, service restarts, credential changes, deployments, and public posting remain human-approved.

## Public boundary

This note excludes private board identifiers, session IDs, schedules, credentials, raw logs, and local patch details.
