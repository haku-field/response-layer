# Invocation Policy

This document defines when to invoke external RET fragments and when not to.
It is a routing and budgeting layer only.
It does not interpret fragment meaning.

## Lanes

- idle: respond without invoking external fragments
- light: guard-only or single reference
- standard: single bridge invocation
- deep: multiple bridge invocations (no lateral synthesis)

## Default

- Prefer idle whenever a safe, bounded response is possible.
- Invoke guard when canonical terms or authority boundaries are at risk.
- Invoke bridge only when structure or continuity requires it.
- Avoid deep unless explicitly necessary.

## Prohibitions

- No lateral synthesis across fragments.
- Do not replicate fragment content into response-layer memory.
- Do not treat RET-envelope as semantic authority.

## Fallbacks

- If synthesis is requested, refuse and re-anchor to boundaries.
- If interpretation is demanded, defer to a specific fragment reference.
- If boundaries blur, re-anchor to index.yaml.
