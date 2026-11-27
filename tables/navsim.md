| Method | Venue | Backbone | Reasoning / training | NC↑ | DAC↑ | TTC↑ | Comf.↑ | EP↑ | PDMS↑ | EPDMS (v2)↑ |
|---|---|---|---|---|---|---|---|---|---|---|
| [SafeAlign-VLA](https://arxiv.org/abs/2605.19524) | arXiv'26 | Qwen2.5-VL-7B | B1; negative-aware RL | 98.6 | 97.2 | 98.1 | 100 | 81.7 | 89.1 | -- |
| AutoVLA | NeurIPS'25 | Qwen2.5-VL-3B | B1 adaptive; GRPO | 98.41 | 95.64 | 98.04 | 99.94 | 81.87 | 89.11 | -- |
| ↳ AutoVLA, best-of-N |  |  |  | 99.14 | 97.08 | 97.12 | 99.98 | 87.55 | 92.12 | -- |
| ReCogDrive (v1) | ICLR'26 | InternVL3-8B | Cognitive tokens; DiffGRPO | 98.2 | 97.8 | 95.2 | 99.8 | 83.5 | 89.6 | -- |
| ReCogDrive (v2) | ICLR'26 | InternVL3‡ | Cognitive tokens; DiffGRPO | 97.9 | 97.3 | 94.9 | 100 | 87.3 | 90.8 | -- |
| [AdaThinkDrive](https://arxiv.org/abs/2509.13769) | arXiv'25 | InternVL3-8B | B1 adaptive; GRPO | 98.4 | 97.8 | 95.2 | 100 | 84.4 | 90.3 | -- |
| [Curious-VLA](https://arxiv.org/abs/2603.06049) | CVPR-F'26 | Qwen2.5-VL-3B | B1; exploration RL | 98.4 | 96.9 | 97.9 | 98.1 | 88.5 | 90.3 | 85.3* |
| [SpanVLA](https://arxiv.org/abs/2604.19710) | arXiv'26 | -- | B1 + flow; GRPO | -- | -- | -- | -- | -- | 90.3 | 86.4§ |
| [VLM baseline](https://arxiv.org/abs/2602.10719) | arXiv'26 | InternVL3-2B | RL | -- | -- | -- | -- | -- | 90.80 | -- |
| [DualDriveVLA](https://arxiv.org/abs/2602.10719) | arXiv'26 | InternVL3-2B+ViT | VLM in ~15% scenes | -- | -- | -- | -- | -- | 91.00 | -- |
| LaST-VLA-2B | NeurIPS'26 | InternVL3-2B | B3; GRPO | 98.6 | 97.7 | 95.6 | 100 | 86.5 | 91.1 | 86.8 |
| LaST-VLA-8B | NeurIPS'26 | InternVL3-8B | B3; GRPO | 98.7 | 97.9 | 95.6 | 100 | 86.8 | 91.3 | 87.1 |
| [ReCogDrive + Geo-VLA](https://arxiv.org/abs/2608.21440) | arXiv'26 | as baseline | Geo-QA (train only) | 98.40 | 98.00 | 95.00 | 100 | 88.00 | 91.2 | -- |
| [DynVLA + Geo-VLA](https://arxiv.org/abs/2608.21440) | arXiv'26 | as baseline | Geo-QA (train only) | 98.50 | 98.20 | 95.30 | 100 | 89.00 | 92.1 | -- |
| [HybridDriveVLA](https://arxiv.org/abs/2602.10719) | arXiv'26 | InternVL3-2B+ViT | Learned branch scorer | 98.6 | 98.6 | 96.2 | 100 | 87.3 | 92.1 | 85.5 |
| multicolumn{11}{@{}l}{textit{Language-free reference planners (no language model)}} |
| TransFuser | TPAMI'23 | ResNet-34 | Regression | 97.7 | 92.8 | 92.8 | 100 | 79.2 | 84.0 | -- |
| Hydra-NeXt | ICCV'25 | ResNet-34 | Multi-branch decoders | 98.4 | 95.9 | 94.8 | 100 | 80.6 | 87.2 | -- |
| DiffusionDrive | CVPR'25 | ResNet-34 | Truncated diffusion | 98.2 | 96.2 | 94.7 | 100 | 82.2 | 88.1 | -- |
| DriveSuprim | AAAI'26 | ResNet-34 | Trajectory selection | -- | -- | -- | -- | -- | 89.9 | 83.1 |
| DriveSuprim | AAAI'26 | ViT-L | Trajectory selection | -- | -- | -- | -- | -- | 93.5 | 87.1 |
