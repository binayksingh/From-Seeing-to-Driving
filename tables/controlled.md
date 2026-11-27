| Factor changed | Study | Metric | Reported change | Reading |
|---|---|---|---|---|
| multicolumn{5}{@{}l}{textit{RQ1: Understanding}} |
| Geometric QA supervision (training only) | [Geo-VLA†](https://arxiv.org/abs/2608.21440) | NAVSIM PDMS ↑ | +0.4 (ReCogDrive); +1.1 (DynVLA) | Consistent but small gain |
| Spatial stream added to the VLM | [S²-VLA†](https://arxiv.org/abs/2607.13926) | NAVSIM PDMS ↑ | +3.0 over 87.1, without RL | Direct access to geometry helps |
| Language model distilled into the planner | DiMA | Long-tail trajectory error ↓ | -44% | Language knowledge transfers without inference cost |
| Driving fine-tuning of the base VLM | [CausalDriveBench†](https://arxiv.org/abs/2609.32157) | Causal accuracy ↑ | -2 to -34 points | Specialization can erode causal understanding |
| multicolumn{5}{@{}l}{textit{RQ2: Reasoning}} |
| Test-time textual reasoning | [nuReasoning†](https://arxiv.org/abs/2605.31572) | Planning; latency ↓ | No gain; 8.5× latency | Reasoning at inference mostly adds cost |
| Reasoning supervision, no text at inference | [nuReasoning†](https://arxiv.org/abs/2605.31572) | Planning | Improves | The benefit comes from the training signal |
| Reasoning fine-tuning | [nuReasoning†](https://arxiv.org/abs/2605.31572) | Counterfactual acc. ↑; 1-m hit rate ↑ | 44.7% → 81.6%; hit rate near zero | Reasoning gains do not reach the trajectory |
| Per-frame language gating | [BLUE](https://doi.org/10.18653/2026.emnlp-main.1894) | B2D SR ↑; latency ↓ | +8.9 points; 1.40 s → 0.55 s | Language helps on 14.5% of routes and hurts on 23.6% |
| Adaptive vs. always reasoning | [AdaThinkDrive†](https://arxiv.org/abs/2509.13769) | Inference time ↓ | -14% at 90.3 PDMS | Reason only when needed |
| RL on causal reasoning chains | [Alpamayo-R1†](https://arxiv.org/abs/2511.00088) | Reasoning quality; consistency ↑ | +45%; +37% | RL can align reasoning with action |
| multicolumn{5}{@{}l}{textit{RQ3: Action and training}} |
| Imitation → online RL | MindDrive | B2D DS / SR / mean ability ↑ | 75.85 → 78.04 / 49.30 → 55.09 / 49.44 → 56.94 | RL improves interactive skills most |
| SFT → GRPO | [Poutine†](https://arxiv.org/abs/2506.11234) | WOD-E2E RFS ↑ / ADE@5s ↓ | 7.91 → 7.99 / 2.94 → 2.74 | Light RL suffices after strong pre-training |
| Generative rollouts with GRPO | [GeRo†](https://arxiv.org/abs/2601.11475) | B2D DS / SR ↑ | +15.7 / +26.2 points | Closed-loop RL gives the largest gains |
| Backbone 2B → 8B | LaST-VLA | NAVSIM PDMS / EPDMS ↑ | 91.1 → 91.3 / 86.8 → 87.1 | Scaling adds little |
| VLM → gated VLM + vision-only | [DualDriveVLA†](https://arxiv.org/abs/2602.10719) | PDMS ↑; latency ↓ | 90.80 → 91.00; 1.9× faster (oracle 93.58) | The two backbones are complementary |
