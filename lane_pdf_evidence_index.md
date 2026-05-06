# PDF Evidence Index

Metadata-only PDF evidence manifests linking MCP literature lookup and local graphify citation gates.

## Nodes

- **Graph Routing**: Project-operation task route.
- **Citation Audit**: Project-operation task route.
- **Graphify**: Project-operation task route.
- **Tooling**: Project-operation task route.
- **Literature Graph**: Project-operation task route.
- **PDF Evidence Index**: Metadata-only PDF evidence manifests linking MCP literature lookup and local graphify citation gates.
- **PDF Evidence Index README** (`docs/pdf_evidence_index/README.md`): Explains the metadata-only PDF evidence layer and how MCP, graphify, and Obsidian should use it.
- **Pdf Evidence**: Project-operation task route.
- **Current Cited PDF Manifest** (`docs/pdf_evidence_index/current_cited_pdf_manifest.json`): Sanitized current Chapter 2-4 citation-to-local-evidence mapping for graphify citation checks.
- **Bibliography PDF Manifest** (`docs/pdf_evidence_index/bibliography_pdf_manifest.json`): Broader bibliography-to-local-evidence metadata inventory without publishing PDFs.
- **Missing PDF Sources** (`docs/pdf_evidence_index/missing_sources.json`): Current source-location gaps from Chapter 2-4 graphify location manifests.
- **Source Recovery**: Project-operation task route.
- **PDF Evidence Index Builder** (`tools/build_pdf_evidence_index.py`): Regenerates sanitized PDF evidence metadata manifests.

## Edges

- `lane:pdf_evidence_index` -contains-> `doc:docs_pdf_evidence_index_README.md`
- `lane:pdf_evidence_index` -contains-> `doc:docs_pdf_evidence_index_current_cited_pdf_manifest.json`
- `lane:pdf_evidence_index` -contains-> `doc:docs_pdf_evidence_index_bibliography_pdf_manifest.json`
- `lane:pdf_evidence_index` -contains-> `doc:docs_pdf_evidence_index_missing_sources.json`
- `lane:pdf_evidence_index` -contains-> `doc:tools_build_pdf_evidence_index.py`
- `task:pdf_evidence` -opens-> `doc:docs_pdf_evidence_index_README.md`
- `task:citation_audit` -opens-> `doc:docs_pdf_evidence_index_README.md`
- `task:graph_routing` -opens-> `doc:docs_pdf_evidence_index_README.md`
- `task:pdf_evidence` -opens-> `doc:docs_pdf_evidence_index_current_cited_pdf_manifest.json`
- `task:citation_audit` -opens-> `doc:docs_pdf_evidence_index_current_cited_pdf_manifest.json`
- `task:graphify` -opens-> `doc:docs_pdf_evidence_index_current_cited_pdf_manifest.json`
- `task:pdf_evidence` -opens-> `doc:docs_pdf_evidence_index_bibliography_pdf_manifest.json`
- `task:literature_graph` -opens-> `doc:docs_pdf_evidence_index_bibliography_pdf_manifest.json`
- `task:graph_routing` -opens-> `doc:docs_pdf_evidence_index_bibliography_pdf_manifest.json`
- `task:pdf_evidence` -opens-> `doc:docs_pdf_evidence_index_missing_sources.json`
- `task:citation_audit` -opens-> `doc:docs_pdf_evidence_index_missing_sources.json`
- `task:source_recovery` -opens-> `doc:docs_pdf_evidence_index_missing_sources.json`
- `task:pdf_evidence` -opens-> `doc:tools_build_pdf_evidence_index.py`
- `task:tooling` -opens-> `doc:tools_build_pdf_evidence_index.py`
- `task:graph_routing` -opens-> `doc:tools_build_pdf_evidence_index.py`
