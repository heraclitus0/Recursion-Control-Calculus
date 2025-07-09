# Recursion Control Calculus (RCC): Prototype and Simulation Framework

## Overview

This repository contains the first formal implementation of **Recursion Control Calculus (RCC)**—a control-theoretic framework for managing epistemic state evolution in agents exposed to stochastic volatility.

RCC introduces a symbolic and operational calculus involving:
- Recursion operators for epistemic state manipulation  
- Cumulative misalignment control fields  
- Adaptive rupture thresholds  
- Reset mechanisms to enforce epistemic coherence

The framework is built atop a formal axiomatic system and meta-theorems defining recursion control dynamics. This codebase validates RCC’s stability, responsiveness, and fault-tolerance through multiple simulation environments.

---

## Simulation Configurations

### 1. **Prototype RCC Simulation** (200 cycles)  
Tests recursion control under moderate epistemic perturbations.

- **Initial State**: 𝓥₀ = 0.5  
- **Perturbation Model**: Gaussian N(0, 0.3²)  
- **Dynamic Threshold**: Scaled by misalignment + Gaussian N(0, 0.025²)  
- **Realignment**: Triggered when Δ(t) ≤ Θ(t) via Continuity Monad  
- **Resets**: When rupture thresholds are breached  

**Outputs**:
- Evolution of the memory projection field  
- Growth of epistemic misalignment  
- Timeline of distortion and rupture events  

---

### 2. **Baseline RCC System** (500 cycles)  
Recursion under consistent volatility.

- **Perturbation**: Gaussian N(0, 0.18²)  
- **Thresholds**: Proportional to misalignment  
- **Behavior**: Continuous misalignment accumulation + rupture-triggered resets  

**Outputs**:
- Projection vs reception field evolution  
- Temporal distortion patterns  
- Misalignment accumulation curve  
- Rupture event mapping  

---

### 3. **Stress-Test RCC System** (600 cycles)  
Tests system resilience under amplified volatility.

- **Perturbation**: Gaussian N(0, 0.35²)  
- **Aggressive Misalignment Scaling**  
- **Dynamic Threshold Perturbation**  

**Outputs**:
- Projection vs reception drift  
- Cumulative distortion and rupture spread  
- Fault-line tracing of epistemic collapse events  

---

### 4. **Naïve Agent vs RCC Agent** (300 cycles)  
Comparative run to contrast linear state update (naïve) vs RCC-based control.

**Outputs**:
- Epistemic trajectories of both agents  
- Misalignment accumulation in RCC agent  
- Rupture event log (RCC agent only)  

---

## Repository Structure

Recursion-Control-Calculus/
│
├── LICENSE.txt                  
├── README.md                   
│
├── baseline_stresstest.py     
├── naive_rcc.py                
├── rcc_prototype.py            


---

## License

This project is licensed under the [MIT License](./LICENSE) © 2025 Pulikanti Sashi Bharadwaj.

