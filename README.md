# Experimental Data for LLM-Agent Negative Information Selection

This repository contains the analysis-ready experimental data associated with the manuscript **“Negative Information Selection in Evolving Online Discussions with LLM Agents.”**

The study compares three information-selection environments:

- **P1 — Individual judgement:** agents evaluate two reports without social information.
- **P2 — Static feedback:** agents observe fixed comments and like counts before choosing.
- **P3 — Evolving discussion:** agents participate in a multi-round discussion in which posts, replies, and likes become visible to later agents.

All records in this repository were generated in controlled LLM-Agent simulations. They do not contain human-participant data.

## Repository structure

```text
data/
├── main/                       # Main P1, P2, and P3 experiment
├── cognitive_and_atmosphere/  # Cognitive-profile and initial-comment-climate conditions
├── sensitivity/               # Activation-rate, population-size, update, and ablation checks
└── robustness/                # Cross-model robustness checks
metadata/
├── DATA_DICTIONARY.md          # Definitions of files, variables, and metrics
├── PROVENANCE.md               # Mapping from release files to original experiment outputs
└── SHA256SUMS.txt              # File checksums
```

## Main files

- `data/main/stage_summary_95ci.csv` reproduces the main P1–P3 stage-level descriptive statistics and 95% confidence intervals.
- `data/main/p1_p2_individual_results.csv` contains the individual P1 and P2 judgments used to calculate the static-condition summaries.
- `data/main/p3_run_level_summary.csv` contains one row per P3 independent run and scenario.
- `data/main/p3_timestep_summary.csv` contains the round-by-round P3 trajectories.
- `data/main/p3_agent_probe_results.csv` contains terminal agent-level probe outcomes.
- `data/main/p3_public_interaction_events.csv` contains the public P3 interaction events.

The remaining folders provide condition-level and run-level data for the supplementary analyses. See `metadata/DATA_DICTIONARY.md` for details.

## Reproducing the experiments

The executable simulation code, configuration template, and run instructions are maintained separately at:

<https://github.com/hujingxin777-cmyk/llm-agent-negative-information-selection>

The code repository documents the Python environment, model configuration, planning command, smoke test, and full experiment commands. API credentials are not included in either repository.

## Scope of this release

This release is designed for transparent inspection and reanalysis of the results reported in the manuscript. Large checkpoints, cached model-request logs, local environment files, figures, and superseded test runs are excluded because they are not required to reproduce the reported tables from the released analysis-ready data.

## Citation

Please cite the associated article when using these data. The full bibliographic citation and persistent article identifier will be added after publication.
