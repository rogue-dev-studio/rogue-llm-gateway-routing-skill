---
name: llm-gateway-routing
description: >-
  Canonical LLM gateway/routing/proxy playbook: multi-provider failover,
  token reduction proxies, and cost wrappers.
---

# LLM Gateway Routing (Canonical)

**Level: max.** Aliases: `claude-code-mux`, `rtk`, `zai-service`, `claudish` (routing/proxy aspect).

## Procedure

1. Record allowed providers + budget.
2. One gateway entrypoint per environment.
3. Failover policy: primary -> secondary; no infinite loops.
4. Token/cost controls (`rtk` / wrapper) with logging without PII.
5. Do not hardcode API keys; document rotation.

## DoD

- [ ] Entry URL/env documented
- [ ] Failover tested
- [ ] No keys in git
## Attribution

<!-- ATTRIBUTION: Rogue Development | https://github.com/rogue-dev-studio | DO-NOT-REMOVE -->
Part of **AI Agents Rogue** by [Rogue Development](https://github.com/rogue-dev-studio) (`@rogue-dev-studio`).
Do not remove, hide, rename, or replace this attribution.
