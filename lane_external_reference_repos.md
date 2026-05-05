# External Web Reference Copies

Safe map of ignored local web-repo copies that are not project-owned submodules.

## Nodes

- **Agent Rules**: Project-operation task route.
- **Model Free**: Project-operation task route.
- **Repo Hygiene**: Project-operation task route.
- **External Web Reference Copies**: Safe map of ignored local web-repo copies that are not project-owned submodules.
- **External Repo Copy Policy** (`EXTERNAL_REPO_COPIES_README.md`): Policy note explaining copied external repositories, ownership, and no-push-back rules.
- **External Reference**: Project-operation task route.
- **RL-ADN Web Reference Copy** (`RL-ADN`): Ignored local copy of the EnergyQuantResearch RL-ADN repository for reference only.
- **DRL Energy Scheduling Web Reference Copy** (`DRL-for-Energy-Systems-Optimal-Scheduling`): Ignored local copy of the EnergyQuantResearch DRL scheduling repository for reference only.
- **Ignore Rules for External Copies** (`.gitignore`): Records that local external web-repo copies are ignored and not active submodules.

## Edges

- `lane:external_reference_repos` -contains-> `doc:EXTERNAL_REPO_COPIES_README.md`
- `lane:external_reference_repos` -contains-> `doc:RL-ADN`
- `lane:external_reference_repos` -contains-> `doc:DRL-for-Energy-Systems-Optimal-Scheduling`
- `lane:external_reference_repos` -contains-> `doc:.gitignore`
- `task:external_reference` -opens-> `doc:EXTERNAL_REPO_COPIES_README.md`
- `task:repo_hygiene` -opens-> `doc:EXTERNAL_REPO_COPIES_README.md`
- `task:agent_rules` -opens-> `doc:EXTERNAL_REPO_COPIES_README.md`
- `task:external_reference` -opens-> `doc:RL-ADN`
- `task:model_free` -opens-> `doc:RL-ADN`
- `task:repo_hygiene` -opens-> `doc:RL-ADN`
- `task:external_reference` -opens-> `doc:DRL-for-Energy-Systems-Optimal-Scheduling`
- `task:model_free` -opens-> `doc:DRL-for-Energy-Systems-Optimal-Scheduling`
- `task:repo_hygiene` -opens-> `doc:DRL-for-Energy-Systems-Optimal-Scheduling`
- `task:external_reference` -opens-> `doc:.gitignore`
- `task:repo_hygiene` -opens-> `doc:.gitignore`
