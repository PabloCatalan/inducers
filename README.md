# Bayesian Estimation of Efflux Pump Inducers Data on Antimicrobial Resistance

This repository contains the code and data necessary to perform Bayesian inference on the manuscript Catalán et al. 2026 ..., specifically focusing on the estimation of parameters related to antibiotic growth inhibition and MIC (Minimum Inhibitory Concentration) modeling.

## 🔬 Methodology

We use **Bayesian inference** to estimate the posterior distribution of parameters defined in the study's core equations.

### Key Features:

* **Inference Engine:** We employ the **NUTS (No-U-Turn Sampler)** algorithm.
* **Framework:** Implementation is handled via **PyMC**, a state-of-the-art probabilistic programming framework.
* **MIC Calculation:** For visualization and analysis (e.g., Figure 3), the MIC is treated as the midpoint between the highest concentration allowing growth and the lowest concentration inhibiting it.
* *Example:* If growth occurs at  but not at , the MIC is estimated as .



---

## 🚀 Getting Started

The analysis is provided in a Python Notebook (`.ipynb`). To ensure the Bayesian samplers run correctly, we recommend using the provided Conda environment file.

### Prerequisites

You will need [Conda]() (or Miniconda) installed on your system.

### Installation & Setup

1. **Clone the repository:**
```bash
git clone https://github.com/pablocatalan/inducers.git
cd inducers

```


2. **Create the environment from the file:**
```bash
conda env create -f environment.yml

```


3. **Activate the environment and run the notebook:**
```bash
conda activate pymc_env
jupyter notebook

```



---

## 📊 Results

The code in this repository reproduces:

* **Figure 1B:** Parameter posterior distributions.
* **Figure 3:** MIC estimations based on laboratory observations.

## 📚 Citation

If you use this code or the PyMC framework, please cite:

> Abril-Pla O, Andreani V, Carroll C, et al. (2023). **PyMC: A Modern and Comprehensive Probabilistic Programming Framework in Python.**

---

## ✉️ Contact

**Pablo Catalán** GitHub: [@pablocatalan]()

[README file generated using Gemini AI]
