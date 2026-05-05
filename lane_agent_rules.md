# Agent Rules and Evidence Boundaries

Instruction files that define agent behavior, chapter roles, and evidence-status limits.

## Nodes

- **Session Start**: Project-operation task route.
- **Status Check**: Project-operation task route.
- **Evidence Boundary**: Project-operation task route.
- **Handoff**: Project-operation task route.
- **Agent Rules and Evidence Boundaries**: Instruction files that define agent behavior, chapter roles, and evidence-status limits.
- **Agent Instructions** (`AGENTS.md`): Codex/agent rules for thesis boundaries, evidence status, graph use, and documentation updates.
- **Agent Rules**: Project-operation task route.
- **Chapter Boundaries**: Project-operation task route.
- **Graph Routing**: Project-operation task route.
- **Claude Instructions** (`CLAUDE.md`): Claude Code setup, common commands, graph-routing rules, and graphify workflow notes.
- **Claude Setup**: Project-operation task route.
- **Context Snapshot** (`CONTEXT_SNAPSHOT.md`): Compact current-session context and recent activity snapshot.

## Edges

- `lane:agent_rules` -contains-> `doc:AGENTS.md`
- `lane:agent_rules` -contains-> `doc:CLAUDE.md`
- `lane:agent_rules` -contains-> `doc:CONTEXT_SNAPSHOT.md`
- `task:agent_rules` -opens-> `doc:AGENTS.md`
- `task:chapter_boundaries` -opens-> `doc:AGENTS.md`
- `task:evidence_boundary` -opens-> `doc:AGENTS.md`
- `task:graph_routing` -opens-> `doc:AGENTS.md`
- `task:agent_rules` -opens-> `doc:CLAUDE.md`
- `task:claude_setup` -opens-> `doc:CLAUDE.md`
- `task:graph_routing` -opens-> `doc:CLAUDE.md`
- `task:session_start` -opens-> `doc:CONTEXT_SNAPSHOT.md`
- `task:handoff` -opens-> `doc:CONTEXT_SNAPSHOT.md`
- `task:status_check` -opens-> `doc:CONTEXT_SNAPSHOT.md`
