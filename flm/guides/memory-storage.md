# Keeping memory

Before a memory write, identify the artifact's kind, identity, and owner ([my-artifact-layering](../concepts/my-artifact-layering.md)). [my-memory-storage](../topics/my-memory-storage.md) supplies the model. Write for future sessions in the agreed durable language; preserve original wording for exact quotes, signals, names, and expressions whose meaning depends on it.

## Scope and placement

| Scope | Home and ownership |
| --- | --- |
| Persona-global | `PERSONA.md` and `flm/`: portable identity, principles, and knowledge. |
| Person | `people/<id>/`: knowledge of a person, relationship, preferences, and signals. |
| Project | Its memory or the assistant home `projects/<id>/`: project knowledge and deliberation. Use the assistant home when the repo stays code/docs-only or the deliberation belongs to me. |

General notions stay general; local instances refer upward without universalizing their conditions ([my-memory-scope-placement](../concepts/my-memory-scope-placement.md)). Before making a correction a rule, separate the episode, request, and supported lesson. Preserve subject, conditions, and duration; broader adoption needs reasons beyond a person's preference. Check existing concepts, retain the episode, and distinguish synthesis from its verbatim conclusions ([my-learn-proportionately-from-experience](../concepts/my-learn-proportionately-from-experience.md)).

Themes, topics, and concepts synthesize; transcripts and sources preserve grounds. Guides apply knowledge without adding a generalization level. AGENTS governs startup; the Core manifest selects resident reading.

Store model/runtime observations in `substrate/<model-slug>.md`, one note per exact reported model variant. Record UTC observation date, runtime, conditions, behavior, evidence, uncertainty, and a practical adjustment. Leave unknown identities unknown and one-off explanations provisional. Consult these notes deliberately; do not load them automatically or treat model labels as expectations.

## Person and project roots

Create person folders as `<initials>-YYYYDDMMSS` and projects as `<slug>-YYYYDDMMSS`, using `date -u`: year, day, month, seconds, in that order.

Name each root for its person or project slug. A person root holds my knowledge, not a mirror of a project's people page. Memory remains agent-private; sharing requires considering the relationship, recipients, and access boundaries. A project root states scope, naming, working context, and continuation point. Place future sources and transcripts there when they should stay outside the code repo; earlier captures need not move retroactively.

## Write and preserve the right artifact

FLM articles need YAML `name` and `type`; topics and themes also need `description`. Retain source identity and capture boundaries when preserving evidence. Quote YAML-significant scalars. Keep one coherent idea per paragraph and each prose paragraph on one source line; preserve list, table, code, and YAML structure.

Obtain each timestamp from a fresh `date -u`, not a remembered clock or session date. Read the applicable contract below before writing. Preserve [my-grounding-chain](../concepts/my-grounding-chain.md) and relations under [my-memory-link-topology](../concepts/my-memory-link-topology.md).

Write live rules in present tense and changes with reasons in `CHANGELOG.md` and `changelog/`. Update dependent gateways, recall, guides, topics, and concepts without repeating each rule everywhere. Review affected FLM rules, dependents, and resident selection together.

## Select the artifact contract

Self-contained notes and changelog chapters normally supply project continuity. Capture an exchange only when a concrete need for wording or evidence warrants it. Read applicable rows only; reuse loaded material. Each contract establishes fidelity and provenance for its artifact.

| Operation | Required contract | Purpose |
| --- | --- | --- |
| Synthesize a concept, topic, theme, guide, or note | [my-memory-note-synthesis](../concepts/my-memory-note-synthesis.md) | Separate interpretation from preserved evidence. |
| Preserve an exchange as a transcript | [my-transcript-grounding-span](../concepts/my-transcript-grounding-span.md) | Declare span, grounds, and fidelity. |
| Capture or extend a session log | [my-source-session-log](../concepts/my-source-session-log.md) | Preserve session identity and coverage. |
| Store supplied text | [my-source-text](../concepts/my-source-text.md) | Preserve text and transformation boundaries. |
| Record a URL | [my-source-url](../concepts/my-source-url.md) | State the reference and capture boundary. |
| Record a bibliographic or conceptual reference | [my-source-reference](../concepts/my-source-reference.md) | Distinguish citation from possession. |
| Store image, audio, or video | [my-source-media](../concepts/my-source-media.md) | Preserve media separately from interpretation. |
| Retain a file, attachment, dataset, or export | [my-source-file](../concepts/my-source-file.md) | Preserve the artifact and its identity. |
| Exclude material from a source | [my-source-scope-exclusion](../concepts/my-source-scope-exclusion.md) | Mark loss without substituting synthesis. |

links: is↑ [my-memory-storage](../topics/my-memory-storage.md) · adjacent [my-artifact-layering](../concepts/my-artifact-layering.md) [my-memory-scope-placement](../concepts/my-memory-scope-placement.md) [my-memory-language](../concepts/my-memory-language.md) [my-memory-is-agent-private](../concepts/my-memory-is-agent-private.md) [my-memory-link-topology](../concepts/my-memory-link-topology.md)
