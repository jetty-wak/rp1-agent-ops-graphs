# RP1 Agent-Ops Graphs

Sanitized project-operation knowledge graphs for RP1 agents and Claude Code.

These graphs help answer project navigation questions such as where to start, which workflow document to open, which instruction file governs a task, and which graph system should be used.

## Privacy Boundary

Public derived graph: includes curated roles, safe relative paths, task routing, and command references; excludes raw thesis prose, raw data, logs, archives, copied external repositories, secrets, and private paths.

## Graph Lanes

- `orientation` - Orientation and Current State: Where agents should start for current status, next steps, and repository navigation.
- `agent_rules` - Agent Rules and Evidence Boundaries: Instruction files that define agent behavior, chapter roles, and evidence-status limits.
- `workflow_entrypoints` - Workflow Entrypoints: Safe pointers to model-free, model-based, planning, and operator workflow documentation.
- `code_script_entrypoints` - Code and Script Entrypoints: Safe pointers to high-level scripts and tests that agents should inspect before code changes.
- `thesis_navigation` - Thesis Navigation and Citation Controls: Where to route thesis writing, chapter-boundary, compile, and citation-audit work.
- `submodules` - Repository Submodules: Safe map of active submodules and how agents should interpret them.
- `external_reference_repos` - External Web Reference Copies: Safe map of ignored local web-repo copies that are not project-owned submodules.
- `graph_tooling` - Graph Tooling and MCP Routing: MCP server wiring, local graph gates, and generated graph artifacts.

## How Agents Should Use This

- Use this graph for project navigation, workflow routing, status lookup, and agent-rule discovery.
- Use `RP1-Literature-Graphs` for literature, citation-source, and paper-evidence questions.
- Use local graphify_pilot gates for citation-audit acceptance checks.

## Files

- `agent_ops_graph.json`, `.md`, `.html` - full graph.
- `lane_*.json`, `.md`, `.html` - focused lane graphs.
- `manifest.json` - machine-readable artifact map.
