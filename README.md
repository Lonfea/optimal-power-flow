# AI for Optimal Power Flow

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Neural%20Networks-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Climate AI](https://img.shields.io/badge/Climate%20AI-Power%20Systems-2E8B57)](https://www.climatechange.ai/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A hands-on machine-learning workflow for approximating **AC Optimal Power Flow (AC-OPF)** on a five-bus electricity network. The project connects power-system optimization with PyTorch and evaluates predictions using operationally meaningful constraints—not accuracy alone.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Lonfea/optimal-power-flow/blob/main/AI_for_Optimal_Power_Flow.ipynb)

## Why this project matters

Power-system operators repeatedly solve AC-OPF to determine economically efficient generator schedules while respecting nonlinear grid constraints. Neural approximators may accelerate this process, but an apparently accurate prediction can still violate voltage, generator, or transmission limits. This tutorial therefore treats feasibility and physical consistency as first-class evaluation criteria.

## Project workflow

1. Represent a five-bus power network and formulate the AC-OPF problem.
2. Generate or load optimization-solver labels.
3. Prepare operating conditions and targets for supervised learning.
4. Train PyTorch neural networks to approximate OPF solutions.
5. Compare predictions with solver outputs.
6. Evaluate constraint violations and discuss safe deployment limits.

## Skills demonstrated

- Nonlinear optimization and AC power-flow fundamentals
- PyTorch model development and supervised learning
- Physics-aware and constraint-aware evaluation
- Energy-system data preparation
- Critical assessment of AI in safety-sensitive infrastructure

## Repository contents

- `AI_for_Optimal_Power_Flow.ipynb` — complete executable tutorial
- `data/` and supporting assets — network inputs and experiment resources
- `LICENSE` — MIT License

## Responsible use

This is an educational approximation workflow, not a production grid-control system. Operational use requires validated network models, robust feasibility recovery, uncertainty analysis, and review by qualified power-system engineers.

## Portfolio note and provenance

This repository is my portfolio fork and study implementation of the **Climate Change AI** tutorial. The tutorial design, notebook, and scientific content are credited to the original creators below. My fork preserves that attribution and provides a portfolio-oriented project overview.

### Original creators

**2023 release**

- Jorge Montalvo, Climate Change AI
- Utkarsha Agwan, University of California, Berkeley
- Panos Moutis, Climate Change AI

**2024 and 2026 revisions**

- Enming Liang
- Advising contributions from Priya L. Donti, Minghua Chen, and the CCAI Virtual Summer School Organizing Committee

## Citation

Montalvo, J., Agwan, U., Moutis, P., & Liang, E. (2026). *AI for Optimal Power Flow* [Tutorial]. Climate Change AI Summer School. https://doi.org/10.5281/zenodo.21827296

```bibtex
@misc{montalvo2026ai,
  title={AI for Optimal Power Flow},
  author={Montalvo, Jorge and Agwan, Utkarsha and Moutis, Panos and Liang, Enming},
  year={2026},
  organization={Climate Change AI},
  type={Tutorial},
  doi={10.5281/zenodo.21827296},
  booktitle={Climate Change AI Summer School},
  howpublished={\url{https://github.com/climatechange-ai-tutorials/optimal-power-flow}}
}
```

## License

Released under the [MIT License](LICENSE).