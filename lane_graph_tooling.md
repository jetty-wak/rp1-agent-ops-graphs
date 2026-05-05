# Graph Tooling and MCP Routing

MCP server wiring, local graph gates, and generated graph artifacts.

## Nodes

- **Graph Routing**: Project-operation task route.
- **Citation Audit**: Project-operation task route.
- **Graphify**: Project-operation task route.
- **Tooling**: Project-operation task route.
- **Mcp**: Project-operation task route.
- **Literature Graph**: Project-operation task route.
- **Graph Tooling and MCP Routing**: MCP server wiring, local graph gates, and generated graph artifacts.
- **MCP Server Map** (`.mcp.json`): Local MCP configuration for project graph servers.
- **Graphify Query Policy** (`tools/graphify_pilot_queryset_policy.md`): Governance policy for local graphify query sets and regression gates.
- **Agent-Ops Graph Builder** (`tools/build_agent_ops_graphs.py`): Builder for this sanitized agent-operations MCP graph package.
- **Literature Graph README** (`docs/knowledge_graphs/README.md`): Documentation for the existing literature and citation-support graph package.

## Edges

- `lane:graph_tooling` -contains-> `doc:.mcp.json`
- `lane:graph_tooling` -contains-> `doc:tools_graphify_pilot_queryset_policy.md`
- `lane:graph_tooling` -contains-> `doc:tools_build_agent_ops_graphs.py`
- `lane:graph_tooling` -contains-> `doc:docs_knowledge_graphs_README.md`
- `task:mcp` -opens-> `doc:.mcp.json`
- `task:graph_routing` -opens-> `doc:.mcp.json`
- `task:tooling` -opens-> `doc:.mcp.json`
- `task:graphify` -opens-> `doc:tools_graphify_pilot_queryset_policy.md`
- `task:citation_audit` -opens-> `doc:tools_graphify_pilot_queryset_policy.md`
- `task:tooling` -opens-> `doc:tools_graphify_pilot_queryset_policy.md`
- `task:mcp` -opens-> `doc:tools_build_agent_ops_graphs.py`
- `task:graph_routing` -opens-> `doc:tools_build_agent_ops_graphs.py`
- `task:tooling` -opens-> `doc:tools_build_agent_ops_graphs.py`
- `task:mcp` -opens-> `doc:docs_knowledge_graphs_README.md`
- `task:literature_graph` -opens-> `doc:docs_knowledge_graphs_README.md`
- `task:graph_routing` -opens-> `doc:docs_knowledge_graphs_README.md`
