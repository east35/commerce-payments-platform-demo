---
title: "Authorization and Capture Redesign"
slug: "auth-capture-redesign"
status: draft
category: capability
priority: high
owner: "@sofia.martin"
ai_visible: true
phase: null
dependencies: ["provider-failover-orchestrator"]
tags: ["authorization", "capture", "checkout"]
updated_at: "2026-02-15T14:15:53.341Z"
created_at: "2026-02-15T14:15:53.341Z"
---
## Context

Current auth/capture logic causes duplicate edge cases under retries.

## Proposed Changes

- Separate auth and capture state machine
- Explicit terminal statuses
- Replay-safe webhook handling

## Acceptance Criteria

- [ ] No duplicate capture in retry simulation
- [ ] Ledger reconciliation checks pass