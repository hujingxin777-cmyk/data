# Data Provenance

The release files are unchanged copies of final analysis outputs, renamed and organized for public use. No numerical values were edited during packaging.

| Release location | Original experiment output | Purpose |
|---|---|---|
| `data/main/stage_summary_95ci.csv` | `main_static_ternary_r300_2026-07-22` | Main P1–P3 stage summary |
| `data/main/p1_p2_individual_results.csv` | `main_static_ternary_r300_2026-07-22` | Individual P1/P2 judgments |
| `data/main/p3_*` | `main_300_formal_r1_30` | Thirty-run, 300-agent P3 main experiment |
| `data/cognitive_and_atmosphere/p1_p2_condition_summary.csv` | `static_ternary_r300_batched30_sd_2026-08-01` | Cognitive-profile and comment-climate P1/P2 summaries |
| `data/cognitive_and_atmosphere/p3_*` | `论文汇报_300人最终整合_2026-06-06` | Cognitive-profile and comment-climate P3 outputs |
| `data/sensitivity/main_activation_rate_*` | Corresponding activation-rate output directories | Activation-rate checks |
| `data/sensitivity/main_scale_*` | Corresponding population-size output directories | Population-size checks |
| `data/sensitivity/main_transfer_*` and `main_fixed_schedule_*` | Corresponding sensitivity output directories | Internal-update and activation-schedule checks |
| `data/sensitivity/main_ablation_*` | Corresponding ablation output directories | Interaction-channel ablations |
| `data/robustness/*_main_r10` | Corresponding model output directories | Cross-model robustness checks |
| `data/robustness/model_robustness_summary.csv` | `模型鲁棒性实验汇总_2026-07-13.csv` | Combined robustness summary |

The original workspace also contains checkpoints, cached model requests, diagnostic logs, plotting outputs, and superseded trial runs. Those files are deliberately excluded from this analysis-ready release.
