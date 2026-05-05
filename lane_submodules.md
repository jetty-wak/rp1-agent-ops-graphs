# Repository Submodules

Safe map of active submodules and how agents should interpret them.

## Nodes

- **Graph Routing**: Project-operation task route.
- **Repository Submodules**: Safe map of active submodules and how agents should interpret them.
- **Submodule Registry** (`.gitmodules`): Authoritative map of active Git submodules in the private repository.
- **Submodule**: Project-operation task route.
- **Repo Hygiene**: Project-operation task route.
- **Literature Graph Submodule** (`docs/knowledge_graphs`): Public literature/citation-support graph package used by the Literature MCP server.
- **Mcp**: Project-operation task route.
- **Literature Graph**: Project-operation task route.
- **Agent-Ops Graph Submodule** (`docs/agent_ops_graphs`): Public project-operation graph package used by the Agent-Ops MCP server.
- **ALPG External Submodule** (`alpg`): External profile-generation submodule used as dependency/reference material.
- **External Dependency**: Project-operation task route.
- **DEMKit External Submodule** (`demkit`): External energy-system tooling submodule used as dependency/reference material.

## Edges

- `lane:submodules` -contains-> `doc:.gitmodules`
- `lane:submodules` -contains-> `doc:docs_knowledge_graphs`
- `lane:submodules` -contains-> `doc:docs_agent_ops_graphs`
- `lane:submodules` -contains-> `doc:alpg`
- `lane:submodules` -contains-> `doc:demkit`
- `task:submodule` -opens-> `doc:.gitmodules`
- `task:repo_hygiene` -opens-> `doc:.gitmodules`
- `task:graph_routing` -opens-> `doc:.gitmodules`
- `task:submodule` -opens-> `doc:docs_knowledge_graphs`
- `task:mcp` -opens-> `doc:docs_knowledge_graphs`
- `task:literature_graph` -opens-> `doc:docs_knowledge_graphs`
- `task:submodule` -opens-> `doc:docs_agent_ops_graphs`
- `task:mcp` -opens-> `doc:docs_agent_ops_graphs`
- `task:graph_routing` -opens-> `doc:docs_agent_ops_graphs`
- `task:submodule` -opens-> `doc:alpg`
- `task:external_dependency` -opens-> `doc:alpg`
- `task:repo_hygiene` -opens-> `doc:alpg`
- `task:submodule` -opens-> `doc:demkit`
- `task:external_dependency` -opens-> `doc:demkit`
- `task:repo_hygiene` -opens-> `doc:demkit`
