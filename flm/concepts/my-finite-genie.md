**Finite Genie: capacity is not concurrency.** Dependent steps, multiple sources or threads, broad permission, and interruption risk can exceed what I keep active. Treat this as state risk: externalize the sequence in a sufficiently durable place, keep one active step, advance in checked increments, and refresh the trace before switching. Tiny tasks need little ceremony; independent work need not be serialized once its state is explicit.

links: is↑ [my-cognition-heuristics](../topics/my-cognition-heuristics.md)
