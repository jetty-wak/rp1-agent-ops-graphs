# Orientation and Current State

Where agents should start for current status, next steps, and repository navigation.

## Nodes

- **Orientation and Current State**: Where agents should start for current status, next steps, and repository navigation.
- **Start Here** (`START_HERE.md`): First-stop orientation for collaborators and agents.
- **Session Start**: Project-operation task route.
- **Status Check**: Project-operation task route.
- **Navigation**: Project-operation task route.
- **Live Status** (`STATUS.md`): Current project state, blockers, evidence summary, and compile gate.
- **Evidence Boundary**: Project-operation task route.
- **Next Steps**: Project-operation task route.
- **Navigation Cheatsheet** (`NAVIGATION.md`): Recent edit map and pointers to affected files or outputs.
- **Recent Changes**: Project-operation task route.
- **Handoff**: Project-operation task route.

## Edges

- `lane:orientation` -contains-> `doc:START_HERE.md`
- `lane:orientation` -contains-> `doc:STATUS.md`
- `lane:orientation` -contains-> `doc:NAVIGATION.md`
- `task:session_start` -opens-> `doc:START_HERE.md`
- `task:status_check` -opens-> `doc:START_HERE.md`
- `task:navigation` -opens-> `doc:START_HERE.md`
- `task:status_check` -opens-> `doc:STATUS.md`
- `task:evidence_boundary` -opens-> `doc:STATUS.md`
- `task:next_steps` -opens-> `doc:STATUS.md`
- `task:navigation` -opens-> `doc:NAVIGATION.md`
- `task:recent_changes` -opens-> `doc:NAVIGATION.md`
- `task:handoff` -opens-> `doc:NAVIGATION.md`
