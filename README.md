# Paradigm Zero: N-Body Simulations & Proofs

**Author:** Alexssandro N. de Oliveira  
**Status:** Open-source physics and mathematical proofs

## Overview
This repository contains the high-precision N-body simulation codes and Genetic Algorithm scripts used in the paper: **"Dynamic Coupling of Lunar Capture and Martian Migration: Evidence of a Planet 9 Flyby in the Inner Solar System"**.

The codes are designed to prove, strictly through orbital mechanics and conservation of angular momentum, that Earth's 23.5° axial tilt, the Moon's capture, and Mars's ejection to 1.52 AU are parts of a single, coupled dynamic event triggered by a ~44 Earth Mass trans-Neptunian body (Planet 9).

## Dependencies
To replicate the N-body simulations, you will need a Python environment with the following libraries:
- `rebound` (IAS15 Integrator)
- `numpy`
- `scipy` (for Genetic Algorithm optimizations and RK4)

## ⚠️ Methodological Note (The 1.29 Error Margin)
In the spirit of absolute scientific transparency and adhering to the **"Zero Modulation"** premise established in the paper, you will notice a calculated offset/error of **1.29** in the raw output data. 

**This margin of error was intentionally preserved and not artificially erased.** It was kept and methodologically adjusted within the algorithms so that peers can fully understand the raw N-body constraints, the gravitational noise of the integration, and the genuine step-by-step approach of our physics engine. We do not force perfect mathematical fits at the cost of physical reality.

---

## 📂 Repository File Guide (Execution Order)

Follow this index to understand the chronology of the simulations and replicate the findings step-by-step:

| No. | Original File Name | Phase / Scientific Purpose |
|-----|--------------------|----------------------------|
| 01 | `PROMPT MESTRE — Manifest0.txt` | **Foundation:** Rules, style, and Paradigm Zero logic. |
| 02 | `t1-codigosimulação.txt` | **Phase T-1:** Code generating the 864 N-body scenarios. |
| 03 | `output_t1.txt` | **Phase T-1:** Output proving the 3:2 original resonance. |
| 04 | `01_Fase_t-1_Relatorio_Estabilidade_Terra_Marte.txt` | **Phase T-1:** Technical report validating the origin. |
| 05 | `02_Fase_1_Cod_Scan_Amplo_Captura.py` | **Phase 1 (Moon):** Wide scan code for lunar capture. |
| 06 | `03_Fase_1_Cod_Refinamento_Captura.py` | **Phase 1 (Moon):** Refinement of the ideal capture windows. |
| 07 | `07_Fase_1_Output_Refinamento_Zonas.txt` | **Phase 1 (Moon):** Output pinpointing 127° and 300° angles. |
| 08 | `04_Fase_1_Cod_Definitivo_NCorpos.py` | **Phase 1 (Moon):** Exact moment of capture code (RK4). |
| 09 | `05_Fase_1_Output_Definitivo_NCorpos.txt` | **Phase 1 (Moon):** Output: Moon captured, Mars locked at 1.35 AU. |
| 10 | `06_Fase_1_Relatorio_Validacao_Captura_Lunar.txt` | **Phase 1 (Moon):** Proof of absence of fitting/modulation. |
| 11 | `conexãoLua_antes_a_12007.txt` | **Logical Bridge:** Kaula equations adapted; tidal rate as anchor. |
| 12 | `08_Fase_2_Cod_Validacao_Reversa_Lua.py` | **Phase 2 (Time):** Time regression code (3.8 cm/year). |
| 13 | `09_Fase_2_Output_Validacao_Reversa_Lua.txt` | **Phase 2 (Time):** Output: 12,077 years ago with < 1% error. |
| 14 | `protoplaneta-fasepre_4-marte95%.txt` | **Phase 3 (Search):** Initial Genetic Algorithm code. |
| 15 | `08_Fase_3_Output_Busca_Agente_Preliminar.txt` | **Phase 3 (Search):** Output attesting the possibility of moving Mars. |
| 16 | `10_Fase_4_Cod_Otimizacao_Flyby_Planeta9.py` | **Phase 4 (The Monster):** "V3 PLUS" Code, high-precision GA. |
| 17 | `11_Fase_4_Output_Otimizacao_Flyby.txt` | **Phase 4 (The Monster):** Output: 44.2 Earth Masses stabilizes Mars. |
| 18 | `ncorpos_5_com9.txt` | **Phase 5 (The Fury):** Final code aligning Cataclysm + Lunar Capture. |
| 19 | `12_Fase_5_Output_Cataclismo_5Corpos.txt` | **Phase 5 (The Fury):** Output: Mars ejected to 1.53 AU in 5 years. |
| 20 | `OS DOIS TITÃS- jupiter- 9 codigo.txt` | **The Epilogue:** Code (6 bodies) of Planet 9's dynamic capture by Jupiter. |

---

*“All N-body simulation source codes, integrator logs, and genetic algorithm parameters are open-source and available for peer replication.”*
