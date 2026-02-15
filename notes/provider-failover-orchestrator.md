---
title: "Provider Failover Orchestrator"
slug: "provider-failover-orchestrator"
status: active
category: infrastructure
priority: high
owner: "@omar.haddad"
phase: null
dependencies: ["payments-reliability-vision"]
tags: ["psp", "failover", "resilience"]
updated_at: "2026-02-15T03:01:53.949Z"
created_at: "2026-02-15T03:01:53.949Z"
---
## Scope

Route transactions to secondary provider on primary degradation.

## Rules

- Trigger by rolling error budget breach
- Maintain issuer-country routing constraints
- Preserve idempotency keys across retries

## Current State

Primary path production-ready, fallback path in staged rollout.