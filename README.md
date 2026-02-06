# HEDA-HF-UPPAAL
Formal Verification Models and Queries for HEDA-HF Digital Twin Architecture (UPPAAL)

This repository contains the UPPAAL model and statistical model checking (SMC) experiments for the HEDA-HF system, developed for formal verification and probabilistic analysis in the context of heart failure decision support.

## 📁 Directory Structure
HEDA-HF-UPPAAL/
├── models/
│ ├── heda_model.xml # Main UPPAAL model file
│ └── heda_declarations.txt # Global declarations
├── queries/
│ ├── MC_queries.q # Model checking properties Safety;Liveness,robusteness
│ └── SMC_queries.q # Probabilistic model checking  properties
│ 
├── results/
│ ├── Outputs.txt # Textual summary of  results
│ └── screenshots/
│ ├── fig6_simulation.png # Example simulation trace
│ └── fig7_smc_result.png # SMC distribution output
├── scripts/
│ ├── run_smc_config.json # Example SMC configuration
│ └── example_trace.xta # Optional simulation script
├── LICENSE
└── README.md

## 🧪 Usage
- Open the `models/heda_model.xml` in **UPPAAL SMC**.
- Use the query files in `queries/` to perform verification:
  - Safety: deadlock-freedom, safe transitions
  - Timing: latency constraints (e.g., MAX_ALERT_DELAY)
  - Liveness: eventual responses
  - Probabilistic: bounded-time event probabilities
- Results are reproducible with UPPAAL SMC's statistical settings.

## 📊 Data and Code Availability
- All model files and queries are included in this repository.
- Simulation traces and screenshots are provided under `results/`.
- The repository is meant for reproducibility and research transparency.

  ## ⚠️ Disclaimer
This repository includes verification models only. No real patient data is shared. The UPPAAL software must be used under its respective license.
## ⚠️ Disclaimer

This repository includes verification models only. No real patient data is shared. The UPPAAL software must be used under its respective license.
