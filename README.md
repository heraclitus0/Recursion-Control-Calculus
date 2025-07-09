Recursion Control Calculus: Prototype and Simulation Framework
Overview
This repository provides a formal implementation of the Recursion Control Calculus (RCC) framework for managing epistemic state evolution in AI systems exposed to stochastic perturbations. RCC introduces a calculus of recursion operators, cumulative misalignment control fields, dynamic rupture thresholds, and epistemic state reset mechanisms.

The implementation empirically validates the theoretical control properties derived from the RCC formal axiomatic system and corresponding meta-theorems.

The repository includes three principal simulation configurations:

Prototype Recursion Control Simulation (200 cycles)

Baseline Recursion System (500 cycles)

Stress-Test Recursion System (600 cycles)

Naïve Agent vs. RCC Agent Comparative Simulation (300 cycles)

Each simulation environment tests recursion system resilience under controlled and amplified volatility, confirming the RCC framework’s operational stability and control-theoretic guarantees.

Repository Structure
.
├── rcc_prototype.py               # 200-cycle prototype RCC simulation
├── baseline_stresstest.py         # Baseline and stress-test recursion systems
├── naive_rcc.py                   # Naïve vs RCC agent comparative simulation
├── output_images/                 # Directory for result plots
└── README.md                      # Documentation
Simulation Descriptions
Prototype Recursion Control Simulation
A 200-cycle demonstration of RCC recursion control dynamics under moderate epistemic volatility.
Key parameters:

Initial epistemic state: 𝓥₀ = 0.5

Reception perturbation: Gaussian N(0, 0.3²)

Dynamic rupture threshold scaling by cumulative misalignment and Gaussian noise N(0, 0.025²)

Recursion realignments are performed via a Continuity Monad operator when distortion Δ(t) ≤ Θ(t), with resets to baseline when ruptures occur.

Outputs:

Memory projection field evolution

Cumulative epistemic misalignment growth

Distortion and rupture event timeline

Baseline Recursion System
A 500-cycle recursion control simulation under moderate perturbation conditions.
Key parameters:

Reception perturbation: Gaussian N(0, 0.18²)

Dynamic rupture threshold scaling proportional to misalignment

Continuous misalignment accumulation and rupture-triggered resets

Outputs:

Memory projection field vs reception field

Distortion over time

Cumulative epistemic misalignment growth

Projected divergence and rupture occurrences

Stress-Test Recursion System
A 600-cycle recursion control simulation under amplified epistemic volatility.
Key parameters:

Reception perturbation: Gaussian N(0, 0.35²)

Aggressive misalignment scaling and dynamic rupture threshold perturbation

Outputs:

Memory projection field vs reception field

Distortion over time

Cumulative epistemic misalignment growth

Projected divergence and rupture occurrences

Naïve vs RCC Agent Comparative Simulation
A 300-cycle comparative simulation contrasting a naïve agent with a linear state update rule against a RCC agent employing recursion control calculus.

Outputs:

Epistemic state evolution for both agents

Cumulative epistemic misalignment for the RCC agent

Rupture event log for the RCC agent

License
MIT License

Copyright (c) 2025 Pulikanti Sashi Bharadwaj

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.