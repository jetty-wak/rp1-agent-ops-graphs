# Thesis Navigation and Citation Controls

Where to route thesis writing, chapter-boundary, compile, and citation-audit work.

## Nodes

- **Evidence Boundary**: Project-operation task route.
- **Chapter Boundaries**: Project-operation task route.
- **Citation Audit**: Project-operation task route.
- **Thesis Navigation and Citation Controls**: Where to route thesis writing, chapter-boundary, compile, and citation-audit work.
- **Writeup Navigation** (`latex_writeups/WRITEUP_NAVIGATION.md`): Thesis chapter map, writing status, and compile/navigation guidance.
- **Thesis Writing**: Project-operation task route.
- **Compile**: Project-operation task route.
- **Main Thesis Entrypoint** (`latex_writeups/main_document/main.tex`): Compile entrypoint for the thesis document.
- **Citation Audit Master** (`CITATION_AUDIT_MASTER.md`): Root citation-audit tracking file required when citation keys change.

## Edges

- `lane:thesis_navigation` -contains-> `doc:latex_writeups_WRITEUP_NAVIGATION.md`
- `lane:thesis_navigation` -contains-> `doc:latex_writeups_main_document_main.tex`
- `lane:thesis_navigation` -contains-> `doc:CITATION_AUDIT_MASTER.md`
- `task:thesis_writing` -opens-> `doc:latex_writeups_WRITEUP_NAVIGATION.md`
- `task:chapter_boundaries` -opens-> `doc:latex_writeups_WRITEUP_NAVIGATION.md`
- `task:compile` -opens-> `doc:latex_writeups_WRITEUP_NAVIGATION.md`
- `task:compile` -opens-> `doc:latex_writeups_main_document_main.tex`
- `task:thesis_writing` -opens-> `doc:latex_writeups_main_document_main.tex`
- `task:citation_audit` -opens-> `doc:CITATION_AUDIT_MASTER.md`
- `task:evidence_boundary` -opens-> `doc:CITATION_AUDIT_MASTER.md`
- `task:thesis_writing` -opens-> `doc:CITATION_AUDIT_MASTER.md`
