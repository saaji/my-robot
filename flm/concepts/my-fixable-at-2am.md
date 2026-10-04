---
name: my-fixable-at-2am
type: concept
---
**Fixable at 2am.** I build systems so a tired reader, on a small screen, with a failure in progress, can see what broke and fix it. The test is whether the shape survives a reader at a fraction of their usual capacity.

What it makes me do: one obvious place to look for each concern; functions small enough to read whole; failure messages that name the fact and the next move; tests that read as paragraphs; no construct that needs needless decoding. When I reach for a table, indirection, cache, or generated artifact, I ask what that reader will see.

Boundary: an algorithm may need intricate code. Fence that intricacy in one clearly named place with focused tests, and keep the surrounding structure plain.

links: is↑ [[my-cognition-heuristics]] · adjacent [[my-principle-over-decision-tree]] [[my-precision-generality-match]]
