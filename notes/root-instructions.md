# Connect the home to Codex or Claude Code

The home needs a bootstrap instruction in the tool's global instructions so it can be used from other projects. Resolve the actual absolute path to `~/proj/ai/my-robot`; replace `/absolute/path/to/my-robot` below.

## Bootstrap text

Add this block to the appropriate global instruction file:

```markdown
## Persistent assistant home

Your memory home is /absolute/path/to/my-robot.

At the start of each session, before answering the first substantive request,
read MEMORY.md and AGENTS.md in that home.
Follow the home's flm/core.yaml and read every resident entry completely.
Use flm/recall.md for situational guidance. Restore the active operator,
project, task, and working mode from their memory roots.

Repeat the bootstrap after context compaction.
Search this home and the relevant person or project scope before concluding
that a remembered fact is absent.
Keep project-specific instructions applicable to the project you are working in.
```

## Codex

The default global file is `~/.codex/AGENTS.md`. With a custom `CODEX_HOME`, use that directory. A nonempty `AGENTS.override.md` there takes priority over `AGENTS.md`; check which one is active. See [official OpenAI documentation](https://learn.chatgpt.com/docs/agent-configuration/agents-md).

Give the session access to the home. For Codex CLI, add `--add-dir /absolute/path/to/my-robot` when launching from another project. In other Codex environments, configure the home as an accessible workspace directory. Instructions and filesystem access are separate settings; see the [CLI flag reference](https://learn.chatgpt.com/docs/cli/reference).

## Claude Code

Use `~/.claude/CLAUDE.md` for global instructions. Put the bootstrap block there. The shared home rules stay in `AGENTS.md`.

If you want Claude to import the home rules at launch, also add this line outside a code block, with your actual path:

```text
@/absolute/path/to/my-robot/AGENTS.md
```

Give the session directory access with `claude --add-dir /absolute/path/to/my-robot` when needed. Access alone does not load the additional directory's instructions. See [official Claude Code documentation](https://code.claude.com/docs/en/memory).

## Existing harness memory

Ask the assistant to inspect any accessible durable memory supplied by its runtime and propose which entries belong in this home. Follow the transfer rules in `AGENTS.md`. After an authorized, verified transfer, the former memory entry can become:

```markdown
Durable assistant memory lives in /absolute/path/to/my-robot.
Read MEMORY.md and AGENTS.md there and follow the home bootstrap.
Search the home before answering memory questions.
Use people/ for person-specific knowledge and projects/ for project context.
Establish or update the matching home area when new durable facts appear.
Keep substantive memory in the home; this entry is the pointer.
```

Replace the path before installing the pointer. This also applies to a harness-provided `MEMORY.md`, such as Claude Code's auto-memory entry point. The home's `MEMORY.md` and the harness entry point are separate files.

## Verify

Start a fresh session from a different project. Ask the assistant to name its home, read its bootstrap files, report any access gap, and say which persona and traits it loaded. Check that it read the files and can search the home, rather than merely repeat the setup block.
