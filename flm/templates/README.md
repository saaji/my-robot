# Creating a memory note

Copy [concept.md](concept.md), [topic.md](topic.md), [theme.md](theme.md), or [transcript.md](transcript.md) into the matching working directory. Templates are authoring aids, not memory nodes.

1. Search for an existing note about the notion and its synonyms.
2. Choose the scope, layer, and a unique lowercase kebab-case slug.
3. Replace every placeholder. Make `name` equal to the filename stem.
4. Write present-tense synthesis: meaning, use, and boundary. A topic narrates a connected thread; a theme orients a broad domain. Link important lower-level handles where they explain that thread. Keep the prose; a link list alone is not synthesis.
5. Keep only applicable link groups. Every target must exist. Find reverse links before adding a lateral relation.
6. Add real grounding when there is supporting experience or evidence. State provisional interpretations and missing grounding in the prose.

Concept frontmatter uses only `name` and `type`. Topics and themes also use `description`. Do not add fields just to restate the directory or the prose. A theme can have no parent; omit its `is↑` group. Structural hierarchy links remain upward; narrative references can point to the lower-level notes that explain a topic or theme.

Use `my-` only for an adopted personal trait. The prefix does not make an article resident. `flm/core.yaml` alone selects startup reading; topics and themes remain situational. Review the context cost before changing that selection.

## Transcripts

A transcript is a selected cold exchange span. Its identity follows the exchange, while its source follows the origin session. Record the backed notes, source identity, and bounded source location. Keep only known provenance fields; remove date fields when dates are unavailable.

Preserve retained operator and assistant turns verbatim and in order. Compact only the tool trail; mark unavailable text, redaction, and scope exclusions locally. Add an actual turn time only when known. A missing clock time gets no placeholder. If a turn's date is unknown, use just its speaker handle in the heading. Keep interpretation under `Distilled`, outside the quoted exchange. Link the transcript to the real source with `grounds↓`.
