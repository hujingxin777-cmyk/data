# Data Dictionary

## Experimental stages

- `P1` / `independent`: individual judgement without social information.
- `P2` / `low_feedback`: judgement after exposure to fixed comments and like counts.
- `P3` / `high_interaction`: multi-round discussion with evolving posts, replies, and likes.
- `P3_entry`: group state at entry to the evolving discussion.
- `P3_terminal`: group state at the end of the evolving discussion.

## Core identifiers

- `experiment_family`: main experiment or supplementary experiment family.
- `scenario_name`: public-health information scenario (`influenza_a` or `mycoplasma_pneumonia`).
- `condition_name`: experimental information environment.
- `persona_name` / `agent_persona_name`: prompted cognitive profile.
- `chat_atmosphere`: initial comment climate.
- `repeat_index`: independent simulation-run identifier within a condition.
- `timestep`: discussion round.
- `agent_id`: synthetic agent identifier.

## Main outcomes and process measures

- `nsb`: negative-selection outcome, coded on the scale used by the simulation output.
- `mean_nsb`: mean negative-selection outcome for the indicated unit.
- `gcr`: group consensus rate, calculated as the larger of the negative and non-negative public-action shares.
- `ssa`: social signal asymmetry, calculated by centering and rescaling the negative-signal share around 0.5.
- `nci_comp`: composite negative-content interaction measure for static conditions.
- `scm`: state-change magnitude, calculated from the absolute change in the composite interaction score.
- `mean_entry_all_agents_nsb`: mean group outcome on entry to P3.
- `mean_terminal_all_agents_nsb`: mean group outcome at the end of P3.
- `mean_delta_all_agents_nsb`: terminal-minus-entry change in P3.
- `mean_public_thread_negative_share`: share of negative signals in the public discussion.
- `mean_latent_neg_all`: mean latent negative tendency across all agents at a timestep.
- `n_active_agents`: number of agents acting publicly in a round.
- `n_public_events`: number of visible interaction events in a round.

## File units

- Files ending in `individual_results.csv` contain individual P1/P2 observations.
- Files ending in `agent_probe_results.csv` contain agent-level P3 probe observations.
- Files ending in `public_interaction_events.csv` contain event-level public actions.
- Files ending in `run_level_summary.csv` or `p3_cell_summary.csv` contain one row per independent P3 run and experimental cell.
- Files ending in `timestep_summary.csv` contain one row per run and discussion round.
- Files ending in `summary.csv` contain condition-level descriptive summaries.

Blank fields indicate that a metric was not applicable or was not observed for that row. The released CSV files preserve the original numeric precision and missing-value encoding.
