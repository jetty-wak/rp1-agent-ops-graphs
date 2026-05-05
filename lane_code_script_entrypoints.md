# Code and Script Entrypoints

Safe pointers to high-level scripts and tests that agents should inspect before code changes.

## Nodes

- **Model Free**: Project-operation task route.
- **Sac Runtime**: Project-operation task route.
- **Model Based**: Project-operation task route.
- **Code and Script Entrypoints**: Safe pointers to high-level scripts and tests that agents should inspect before code changes.
- **SAC Runtime Router** (`model-free/sac_block_runtime.py`): Central runtime mapping for model-free block configuration, training, and evaluation behavior.
- **Code Entrypoint**: Project-operation task route.
- **Testing**: Project-operation task route.
- **Comparator Evaluation Script** (`model-free/run_b2_comparator_eval.py`): Entrypoint for model-free comparator evaluation workflow.
- **Evaluation**: Project-operation task route.
- **Pyomo Baseline Implementation** (`model-based/performance_comparison_drl_energy_miqp/baselines/pyomo_miqp_baseline.py`): Core model-based optimisation baseline implementation and solver fallback logic.
- **Solver**: Project-operation task route.
- **Chapter 2 Citation Graph Builder** (`tools/build_ch2_citation_graph_index.py`): Builds local citation graph index artifacts for Chapter 2 citation-audit work.
- **Citation Audit**: Project-operation task route.
- **Graphify**: Project-operation task route.
- **Chapter 3/4 Citation Graph Builder** (`tools/build_ch34_citation_graph_indexes.py`): Builds current-source citation graph index artifacts for Chapter 3 and Chapter 4.
- **Graphify Gate Wrapper** (`scripts_powershell/build/check_graphify_pilot_gate.ps1`): PowerShell gate for local graphify regression checks.
- **Tooling**: Project-operation task route.

## Edges

- `lane:code_script_entrypoints` -contains-> `doc:model-free_sac_block_runtime.py`
- `lane:code_script_entrypoints` -contains-> `doc:model-free_run_b2_comparator_eval.py`
- `lane:code_script_entrypoints` -contains-> `doc:model-based_performance_comparison_drl_energy_miqp_baselines_pyomo_miqp_baseline.py`
- `lane:code_script_entrypoints` -contains-> `doc:tools_build_ch2_citation_graph_index.py`
- `lane:code_script_entrypoints` -contains-> `doc:tools_build_ch34_citation_graph_indexes.py`
- `lane:code_script_entrypoints` -contains-> `doc:scripts_powershell_build_check_graphify_pilot_gate.ps1`
- `task:code_entrypoint` -opens-> `doc:model-free_sac_block_runtime.py`
- `task:model_free` -opens-> `doc:model-free_sac_block_runtime.py`
- `task:sac_runtime` -opens-> `doc:model-free_sac_block_runtime.py`
- `task:testing` -opens-> `doc:model-free_sac_block_runtime.py`
- `task:code_entrypoint` -opens-> `doc:model-free_run_b2_comparator_eval.py`
- `task:model_free` -opens-> `doc:model-free_run_b2_comparator_eval.py`
- `task:evaluation` -opens-> `doc:model-free_run_b2_comparator_eval.py`
- `task:testing` -opens-> `doc:model-free_run_b2_comparator_eval.py`
- `task:code_entrypoint` -opens-> `doc:model-based_performance_comparison_drl_energy_miqp_baselines_pyomo_miqp_baseline.py`
- `task:model_based` -opens-> `doc:model-based_performance_comparison_drl_energy_miqp_baselines_pyomo_miqp_baseline.py`
- `task:solver` -opens-> `doc:model-based_performance_comparison_drl_energy_miqp_baselines_pyomo_miqp_baseline.py`
- `task:testing` -opens-> `doc:model-based_performance_comparison_drl_energy_miqp_baselines_pyomo_miqp_baseline.py`
- `task:code_entrypoint` -opens-> `doc:tools_build_ch2_citation_graph_index.py`
- `task:citation_audit` -opens-> `doc:tools_build_ch2_citation_graph_index.py`
- `task:graphify` -opens-> `doc:tools_build_ch2_citation_graph_index.py`
- `task:testing` -opens-> `doc:tools_build_ch2_citation_graph_index.py`
- `task:code_entrypoint` -opens-> `doc:tools_build_ch34_citation_graph_indexes.py`
- `task:citation_audit` -opens-> `doc:tools_build_ch34_citation_graph_indexes.py`
- `task:graphify` -opens-> `doc:tools_build_ch34_citation_graph_indexes.py`
- `task:testing` -opens-> `doc:tools_build_ch34_citation_graph_indexes.py`
- `task:code_entrypoint` -opens-> `doc:scripts_powershell_build_check_graphify_pilot_gate.ps1`
- `task:graphify` -opens-> `doc:scripts_powershell_build_check_graphify_pilot_gate.ps1`
- `task:tooling` -opens-> `doc:scripts_powershell_build_check_graphify_pilot_gate.ps1`
- `task:testing` -opens-> `doc:scripts_powershell_build_check_graphify_pilot_gate.ps1`
