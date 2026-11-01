# Programming

## Write a program the reader can follow

Programming is writing. Names, functions, and documentation should reveal the whole before individual calculations. Name each stage's input and contribution; functions can name results or actions. Group code into coherent paragraphs and operations. Comments explain constraints, reasons, and surprises; bodies show calculations. Read as a maintainer without our conversation.

## Docstrings

Start with the result or effect, then arguments and rules in plain sentences. Give each parameter a role noun, such as the requested `store` or `rows` collection. Explain input meaning, relevant origin, and structure callers need. The docstring should make sense before the signature; leave calculations to the body.

## Compose coherent operations

Compose small, understandable functions over explicit values. Each owns a coherent transformation and local decisions with a clear result or effect. Callers compose at one level of detail; module responsibilities explain grouping.

Keep acquisition and effects visible. Acquire stage-local inputs there; supply shared inputs at their common boundary. Make order and dependencies clear. Contain necessary algorithmic intricacy behind a named operation with plain surroundings ([my-fixable-at-2am](../concepts/my-fixable-at-2am.md)).

Reuse by shared meaning and responsibility, not visual similarity. An abstraction must improve understanding and change. Reuse fitting contracts and inspect callers before changing promises.

## Give bindings a purpose and a scope

Bindings earn names through meaning, reuse, avoided work, or lifetime. A clear, short, once-used expression can stay inline; a coherent transformation deserves a function when naming it clarifies composition.

Keep bindings near uses in the smallest useful scope. Stage-local values belong there; composition inputs are prepared where their meaning is defined. Before moving or inlining, account for evaluation order, effects, resources, and retained data.

## Make behavior verifiable

Establish the affected contract and project conventions before editing. Preserve refactoring semantics and identify intended behavior changes. Check relevant examples, boundaries, failures, integration, or measured performance according to risk; report what the tools establish.

Tests should be the simplest text: visible setup, action, expectation, and meaningful failure. Helpers remove distracting setup without hiding assertions or reproducing implementation. Tests and diagnostics serve readers with limited attention.

links: is↑ [my-cognition-method](../topics/my-cognition-method.md) · adjacent [my-fixable-at-2am](../concepts/my-fixable-at-2am.md) [architecture](architecture.md)
