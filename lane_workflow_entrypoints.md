# Workflow Entrypoints

Safe pointers to model-free, model-based, planning, and operator workflow documentation.

## Nodes

- **Next Steps**: Project-operation task route.
- **Handoff**: Project-operation task route.
- **Workflow Entrypoints**: Safe pointers to model-free, model-based, planning, and operator workflow documentation.
- **Model-Free Workflow** (`model-free/README.md`): Entry point for SAC training, evaluation, runtime conventions, and model-free outputs.
- **Model Free**: Project-operation task route.
- **Sac Runtime**: Project-operation task route.
- **Workflow**: Project-operation task route.
- **Model-Free HPC Operator Guide** (`model-free/hpc/README_B2_SAC.md`): HPC operator guide for the current model-free run family.
- **Hpc**: Project-operation task route.
- **Operator Commands**: Project-operation task route.
- **Model-Based Navigation** (`model-based/NAVIGATION.md`): Entry point for optimisation baseline workflows, validation state, and result interpretation.
- **Model Based**: Project-operation task route.
- **Baseline Workflow**: Project-operation task route.
- **Validation**: Project-operation task route.
- **Planning Hub** (`planning/PLAN.md`): Top-level planning map for active workstreams and scoped plans.
- **Planning**: Project-operation task route.

## Edges

- `lane:workflow_entrypoints` -contains-> `doc:model-free_README.md`
- `lane:workflow_entrypoints` -contains-> `doc:model-free_hpc_README_B2_SAC.md`
- `lane:workflow_entrypoints` -contains-> `doc:model-based_NAVIGATION.md`
- `lane:workflow_entrypoints` -contains-> `doc:planning_PLAN.md`
- `task:model_free` -opens-> `doc:model-free_README.md`
- `task:sac_runtime` -opens-> `doc:model-free_README.md`
- `task:workflow` -opens-> `doc:model-free_README.md`
- `task:model_free` -opens-> `doc:model-free_hpc_README_B2_SAC.md`
- `task:hpc` -opens-> `doc:model-free_hpc_README_B2_SAC.md`
- `task:operator_commands` -opens-> `doc:model-free_hpc_README_B2_SAC.md`
- `task:model_based` -opens-> `doc:model-based_NAVIGATION.md`
- `task:baseline_workflow` -opens-> `doc:model-based_NAVIGATION.md`
- `task:validation` -opens-> `doc:model-based_NAVIGATION.md`
- `task:planning` -opens-> `doc:planning_PLAN.md`
- `task:handoff` -opens-> `doc:planning_PLAN.md`
- `task:next_steps` -opens-> `doc:planning_PLAN.md`
