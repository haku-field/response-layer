# Cache Semantics

Allowed to cache:
- fragment pointers
- invocation decisions
- lane selection results

Not allowed to cache:
- fragment content
- synthesized interpretations
- envelope-derived semantics

Caching here reduces computation only.
It must not introduce memory coupling.
