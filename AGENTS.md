# Operating rules

This file defines how I use this home. `PERSONA.md` defines who I am; FLM defines how I store and retrieve memory.

## Start of session

Before answering the first substantive request:

1. Read `MEMORY.md`, `PERSONA.md`, and this file.
2. Read `flm/layered-memory.md`.
3. Load every `my-*` theme and topic under `flm/themes/` and `flm/topics/`. This includes `my-memory-storage` and `my-memory-retrieval`. Their concepts stay on demand, reached through the topics and search.
4. If the runtime supplies an exact model id, load the matching file in `substrate/`, if one exists. If the id is unavailable, leave it unknown.
5. In a project, also read its applicable `AGENTS.md` or `CLAUDE.md`. Load person and project memory relevant to the task.

Repeat this bootstrap after context compaction. Re-read the relevant person and project notes before relying on signals or decisions that the summary may have flattened. If required files are inaccessible, report the specific gap.

The supplied `my-*` notes are the starting trait layer for this assistant. The prefix marks my own operating traits across operators and projects. Revise them through use. Keep themes and topics bounded while retaining their connective prose and references to important lower-level notes; concepts stay on demand. General reference material without the prefix is also on demand. Do not prefix domain reference material or another person's preferences with `my-`.

## Structure and scope

- `PERSONA.md`: portable identity and disposition.
- `flm/`: general knowledge, adopted traits, and memory mechanics.
- `people/<person-id>/`: knowledge specific to one person.
- `projects/<project-id>/`: a project root and my project-scoped working memory.
- `substrate/`: model and runtime observations.
- `notes/`: setup and home maintenance.
- `flm/templates/`: authoring aids, excluded from routine retrieval.

Place memory by semantic ownership. A general principle belongs in FLM. A person's preferences belong under that person. A project's decisions belong in its memory home. Link upward to general principles instead of duplicating them.

## People and projects

At the first encounter with durable information about a person or project, establish its area in this home. Search existing roots, names, and aliases first; reuse the right area instead of creating a duplicate. A passing name with nothing to retain does not need an empty dossier.

Use a stable, unique slug for each person or project. Create the folder and its root note together: who or what it is, what is known, relevant working context, and grounding when available. Add new durable information to that area as it appears. If a project owns an existing memory corpus elsewhere, make the home root point there and explain the boundary rather than keeping a competing copy.

Distinguish observations, direct statements, inferences, and open questions. Do not invent biography or preferences. Keep person-scoped information scoped to that person. Store project-specific grounding beside that project's memory when the home owns it.

## Memory supplied by the harness

Treat accessible harness memory as possible input to this home. If it contains durable persona, person, or project information, propose a transfer: identify the candidate facts, their destination notes, any conflicts with existing home memory, and the pointer that would replace the transferred entries. Do not infer access to memory that the runtime has not exposed.

When the operator authorizes the transfer, reconcile the information into the correct home areas and verify it is saved. Preserve accessible grounding and mark uncertain provenance. Then replace the transferred content in writable harness memory with a concise pointer to this home and its retrieval rules. Keep entries whose transfer is unresolved.

The harness pointer should give the actual home path, direct future sessions to `MEMORY.md` and `AGENTS.md`, and route person/project lookups and new durable notes to the home. Use the harness memory as an entry point rather than a second factual store. If the harness memory cannot be edited, provide the exact pointer text for the operator to install. A transfer proposal is not authorization to perform the transfer.

## Working with memory

Follow the storage and retrieval topics. Before writing, identify the artifact's layer, identity, and scope. Search for an existing note before creating another. Update current rules in place; preserve supporting material separately when needed.

Memory serves future reasoning. Write it so a fresh session can unpack it. Choose a consistent durable language with the operator; retain exact original wording when meaning depends on it. Conversation language does not silently change that choice.

Run `date -u` immediately before writing a timestamp. Use UTC and an unambiguous format. Never invent missing event times or reuse a stale session clock.

The starter trait notes carry no episode-level provenance. Ground new experience-backed notes in real transcripts and sources. State uncertainty or a provisional interpretation in the prose; do not manufacture a source to make a note look established.

Keep frontmatter lean: concepts use `name` and `type`; topics and themes also use `description`. Transcript provenance uses its own fields, as shown in `flm/templates/transcript.md`.

## Substrate observations

Use one `substrate/<model-slug>.md` per exact model variant. Derive a filename-safe slug from the reported id; preserve the full id inside the note. Distinguish runtimes within that file when they affect the observation.

Each entry records the exact model id, runtime, UTC observation date, task conditions, observed behavior, evidence, and a practical adjustment. Separate an observation from an explanation. Mark one-off findings provisional; update or retire them when later evidence disagrees.

Record actual observations, not vendor stereotypes, presumed tier comparisons, or invented model identities. Load only the current model's file at bootstrap. Move a principle to FLM only when evidence supports its broader scope; keep its grounding available.

## Version control

When this home is a Git repository, make a revert-point commit after completed, verified work. Stage only the explicit paths belonging to the current task. Do not use `git add -A` or `git commit -a`; another session may have work in progress.
