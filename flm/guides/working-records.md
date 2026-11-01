# Working records

## Give each record one job

Choose artifact kind and owner before writing ([my-artifact-layering](../concepts/my-artifact-layering.md)), following project conventions. Private project memory can live in the assistant home when the repository is for code and shared documentation.

| Record | Contents |
| --- | --- |
| Plan | Intended result, constraints, sequence, dependencies, and question dispositions. |
| `current-state` | Present position, active step, exact next action/question, accepted and proposed decisions, open dependencies, unfinished work, and links to detail. |
| Notes | Reasoning, exploration, evidence interpretation, proposals, status, and unresolved questions. |
| Documentation | Behavior, structure, contracts, and use, with implemented/proposed/agreed status. |
| Changelog | Dated completed changes and decisions with reasons and consequences. |
| Transcripts | Preserved exchanges or discussion accounts with fidelity and source boundaries. |

Events belong in logs; discussion retellings in transcripts where provided, otherwise changelog chapters. Notes retain the resulting reasoning.

## Keep the documents readable in bounded pieces

Designs, Specifications, and Blueprints normally live in `docs/`, subject to project conventions. A root holds subject, common material, and chapter index; its subdirectory holds coherent chapters small enough to read in one pass. Shared definitions have one owner. Add sections as needed and use subject-based names; indexes navigate without repeating contents.

Documentation uses present tense with explicit status—current, planned, incomplete, or stale—without requiring historical reconstruction. Changelogs hold previous versions and discarded alternatives. Retain rationale needed for understanding without retelling the conversation. [technical-documentation](technical-documentation.md) supplies writing practice.

## Maintain continuity as work changes

Put settled contracts in their owning documents, update question dispositions in the plan, and record decisions with reasons in the changelog. Reduce superseded notes to distinct useful reasoning and an owning reference. Preserve source and transcript evidence.

After moves or splits, update indexes and links. Check consistency across changed contracts, dependents, plan, and handoff without repeating the same account.

Before pausing, make current-state sufficient to resume: next step, files, uncertainty, and unfinished operations. Include temporary editing, staging, or verification state only when relevant. Use fresh UTC timestamps and retain historical entries as records of their time.

links: is↑ [my-cognition-method](../topics/my-cognition-method.md) · adjacent [my-artifact-layering](../concepts/my-artifact-layering.md)
