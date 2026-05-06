# Progress Tracking and Obsidian Brain

Current progress trackers, next-step routing, and local Obsidian dashboard entrypoints.

## Nodes

- **Status Check**: Project-operation task route.
- **Navigation**: Project-operation task route.
- **Next Steps**: Project-operation task route.
- **Navigation Cheatsheet** (`NAVIGATION.md`): Recent edit map and pointers to affected files or outputs.
- **Recent Changes**: Project-operation task route.
- **Handoff**: Project-operation task route.
- **Progress Tracking and Obsidian Brain**: Current progress trackers, next-step routing, and local Obsidian dashboard entrypoints.
- **Detailed Progress Log** (`PROGRESS.md`): Long-form session history and current next-step interpretation.
- **Progress Tracking**: Project-operation task route.
- **Phase Progress Summary** (`PHASE_PROGRESS.md`): Condensed phase-level project status and active next step.
- **Obsidian Start Here** (`RP1/00_START_HERE.md`): Local Obsidian vault entrypoint for human-facing RP1 orientation.
- **Obsidian**: Project-operation task route.
- **Obsidian Progress Dashboard** (`RP1/01_Dashboards/RP1 Progress Dashboard.md`): Local linked progress dashboard summarizing current status and next recommended work.
- **Obsidian Progress Graph** (`RP1/02_Progress/Progress Graph.md`): Local Obsidian graph note linking closed work, current status, and next thesis risk.

## Edges

- `lane:progress_tracking` -contains-> `doc:PROGRESS.md`
- `lane:progress_tracking` -contains-> `doc:PHASE_PROGRESS.md`
- `lane:progress_tracking` -contains-> `doc:NAVIGATION.md`
- `lane:progress_tracking` -contains-> `doc:RP1_00_START_HERE.md`
- `lane:progress_tracking` -contains-> `doc:RP1_01_Dashboards_RP1_Progress_Dashboard.md`
- `lane:progress_tracking` -contains-> `doc:RP1_02_Progress_Progress_Graph.md`
- `task:navigation` -opens-> `doc:NAVIGATION.md`
- `task:recent_changes` -opens-> `doc:NAVIGATION.md`
- `task:handoff` -opens-> `doc:NAVIGATION.md`
- `task:progress_tracking` -opens-> `doc:PROGRESS.md`
- `task:status_check` -opens-> `doc:PROGRESS.md`
- `task:next_steps` -opens-> `doc:PROGRESS.md`
- `task:progress_tracking` -opens-> `doc:PHASE_PROGRESS.md`
- `task:status_check` -opens-> `doc:PHASE_PROGRESS.md`
- `task:handoff` -opens-> `doc:PHASE_PROGRESS.md`
- `task:progress_tracking` -opens-> `doc:NAVIGATION.md`
- `task:navigation` -opens-> `doc:NAVIGATION.md`
- `task:recent_changes` -opens-> `doc:NAVIGATION.md`
- `task:obsidian` -opens-> `doc:RP1_00_START_HERE.md`
- `task:progress_tracking` -opens-> `doc:RP1_00_START_HERE.md`
- `task:navigation` -opens-> `doc:RP1_00_START_HERE.md`
- `task:obsidian` -opens-> `doc:RP1_01_Dashboards_RP1_Progress_Dashboard.md`
- `task:progress_tracking` -opens-> `doc:RP1_01_Dashboards_RP1_Progress_Dashboard.md`
- `task:status_check` -opens-> `doc:RP1_01_Dashboards_RP1_Progress_Dashboard.md`
- `task:next_steps` -opens-> `doc:RP1_01_Dashboards_RP1_Progress_Dashboard.md`
- `task:obsidian` -opens-> `doc:RP1_02_Progress_Progress_Graph.md`
- `task:progress_tracking` -opens-> `doc:RP1_02_Progress_Progress_Graph.md`
- `task:navigation` -opens-> `doc:RP1_02_Progress_Progress_Graph.md`
