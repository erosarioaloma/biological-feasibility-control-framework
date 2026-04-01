Feasibility Control of Constrained Biological Regulation

This repository contains the computational models, simulation workflows, and datasets supporting the study:

“A Feasibility Control Law for Constrained Biological Regulation.”

Overview

This work introduces a reduced dynamical framework for biological regulation based on a dimensionless feasibility functional:

[
\Phi = \frac{\Xi (1 - \Psi)}{1 + \Lambda}
]

which governs the accessibility of stable regulated equilibria in a broad class of constrained biological systems.

Despite mechanistic differences across systems, regulatory dynamics collapse onto a common reduced parameter space defined by:

Ξ (Xi): effective regulatory gain
Λ (Lambda): burden throughput
Ψ (Psi): saturation of corrective capacity

The condition ( \Phi < 1 ) defines a feasibility boundary separating stable regulatory regimes from constraint-driven failure.

Repository Structure
├── code/               # Simulation scripts (Python, MATLAB)
├── data/
│   ├── raw/            # Original parameter sets / inputs
│   ├── processed/      # Derived datasets used in figures
│   └── *.csv           # Canonical datasets
├── figures/            # Generated figures (phase diagrams, scaling plots)
├── docs/               # Supplementary notes / derivations
├── README.md
└── requirements.txt
Reproducibility

All results in the manuscript can be reproduced directly from the provided scripts.

Requirements
Python ≥ 3.10
NumPy
SciPy
Matplotlib
(optional) MATLAB for alternate implementations

Install Python dependencies:

pip install -r requirements.txt
Running Simulations
Example: Feasibility Phase Diagram
python code/phase_diagram.py
Example: Parameter Sweep
python code/parameter_sweep.py

These scripts generate the figures corresponding to:

Feasibility phase diagrams
Stability boundaries
Parameter sensitivity analyses
Data

The repository includes:

Parameter sets for tumor–immune dynamics
Proteostasis (SOD1 folding/unfolding) datasets
Synthetic gene circuit burden models
Ecological regulatory models

All datasets are provided in CSV format and are directly used by the simulation scripts.

Scientific Context

This framework demonstrates that:

Diverse biological systems can be represented within a common control-theoretic structure
Regulatory stability is governed by constraint interactions, not system-specific kinetics alone
Failure arises as a constraint-driven transition, rather than gradual degradation

The feasibility functional ( \Phi ) acts as a reduced-order descriptor of these dynamics and defines a constraint-limited universality class for biological regulation.

Code and Data Availability

This repository is archived at:

Zenodo DOI: 10.5281/zenodo.19372265

All simulations can be reproduced directly from the provided scripts without modification.

Citation

If you use this code or data, please cite approriately. 

License

This repository is released under the MIT License.

Contact

Dr. Enrique Rosario Aloma
Barry University – School of Podiatric Medicine
Miami, Florida, USA

Notes
The framework applies to systems exhibiting finite regulatory capacity, transport limitation, and saturation effects.
The universality described is structural rather than molecular, arising from shared constraint architecture.
