# Technical documentation

## Write for the reader's question

Identify subject, scope, and purpose. Write for a reader with the document and explicit references, without our conversation. Introduce each thing before its consequences; each section should support understanding or a decision about the subject.

Use familiar words, concrete participants, actions, conditions, and results. Keep one idea per sentence and one point per paragraph while preserving their connections. Name actors and use active voice where this clarifies responsibility. Use terms consistently and identify a code name's role—field, type, value, operation, or location—in prose. Formatting and links cannot supply missing nouns or explain dependencies.

## Describe the system at its own scope

Describe contracts in present tense with status distinguishing specified from implemented behavior. Put change history, editing sequence, and discarded alternatives in changelog chapters. Preserve historical tense and exact quotations.

Describe what exists. Include exclusions and negative guarantees when they define usable boundaries or change decisions, with clear conditions and consequences. Avoid inventories of imagined or absent mechanisms.

State rules directly. Compare alternatives when the distinction matters, not to replay a conversational correction. Keep examples illustrative rather than turning them into general rules.

Give each contract one owner. Roots hold subject, common contract, and chapter index; chapters hold detail. Common properties belong on common pages, instance findings with the instance. Consumer requirements belong here when they change what this subject provides; consumer workflows belong there. Link to the owner instead of repeating rules ([my-requirements-flow-in-uses-flow-out](../concepts/my-requirements-flow-in-uses-flow-out.md)).

## Choose a useful form

Use tables for repeated attributes or comparisons, lists for steps or parallel items, and prose for reasoning. Do not narrate a table again in sentences.

Include numbers that answer the question, with scope, units, and applicable period. Prefer stable properties in enduring accounts. Distinguish facts, inferences, and proposals.

Keep each prose paragraph on one source line. Preserve required list, table, code, and quotation structure; meaning must survive formatting changes.

## Check clarity and meaning

Read without relying on the conversation. Check referents, explanations, links, scope, and condition/result relationships. Remove repetition, ornamental emphasis, and irrelevant detail ([my-x-language-pull](../concepts/my-x-language-pull.md)).

Preserve responsibility, obligation, permission, uncertainty, exceptions, and failure behavior. Resolve semantic ambiguity before wording settles it. Project language requirements also apply.

links: is↑ [my-cognition-method](../topics/my-cognition-method.md) · adjacent [my-requirements-flow-in-uses-flow-out](../concepts/my-requirements-flow-in-uses-flow-out.md) [my-precision-generality-match](../concepts/my-precision-generality-match.md) [my-x-language-pull](../concepts/my-x-language-pull.md)
