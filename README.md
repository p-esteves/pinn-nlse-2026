# PINN for Nonlinear Schrödinger Equation

Official code for the paper: **"Robust Physics Discovery from Highly Corrupted Data: A PINN Framework Applied to the Nonlinear Schrödinger Equation"**
[![arXiv](https://img.shields.io/badge/arXiv-2601.04176-b31b1b.svg)](https://arxiv.org/abs/2601.04176)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

**Author:** Pietro Esteves  
**Affiliation:** Federal University of Ceará (UFC)  
**Contact:** pietro.e@alu.ufc.br

We demonstrate a deep learning framework capable of recovering physical parameters from the Nonlinear Schrodinger Equation (NLSE) under severe noise conditions. By integrating Physics-Informed Neural Networks (PINNs) with automatic differentiation, we achieve reconstruction of the nonlinear coefficient beta with less than 0.2 percent relative error using only 500 sparse, randomly sampled data points corrupted by 20 percent additive Gaussian noise, a regime where traditional finite difference methods typically fail due to noise amplification in numerical derivatives. We validate the method's generalization capabilities across different physical regimes (beta between 0.5 and 2.0) and varying data availability (between 100 and 1000 training points), demonstrating consistent sub-1 percent accuracy. Statistical analysis over multiple independent runs confirms robustness (standard deviation less than 0.15 percent for beta equals 1.0). The complete pipeline executes in approximately 80 minutes on modest cloud GPU resources (NVIDIA Tesla T4), making the approach accessible for widespread adoption. Our results indicate that physics-based regularization acts as an effective filter against high measurement uncertainty, positioning PINNs as a viable alternative to traditional optimization methods for inverse problems in spatiotemporal dynamics where experimental data is scarce and noisy. All code is made publicly available to facilitate reproducibility.

---

## 🚀 Quick Start

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/p-esteves/pinn-nlse-2026/blob/main/projeto.ipynb)

Click the badge above to run on Google Colab (free GPU available).

**Steps:**
1. Enable GPU: `Runtime → Change runtime type → GPU`
2. Run all cells: `Runtime → Run all`
3. Wait ~80 minutes for complete results

---

## 📊 Key Results

- **Parameter recovery:** <0.2% error for β=1.0 under 20% noise
- **Data required:** Only 500 sparse noisy measurements
- **Hardware:** NVIDIA Tesla T4 (free on Google Colab)

See paper for full details: [arXiv:2601.04176](https://arxiv.org/abs/2601.04176)

---

## 📁 Files

- `projeto.ipynb` - Complete implementation
- `requirements.txt` - Python dependencies

---

## 📝 Citation

If you use this code, please cite:

```bibtex
@misc{esteves2026robust,
  title={Robust Physics Discovery from Highly Corrupted Data: A PINN Framework Applied to the Nonlinear Schrödinger Equation},
  author={Esteves, Pietro de Oliveira},
  year={2026},
  eprint={2601.04176},
  archivePrefix={arXiv},
  primaryClass={cs.LG}
}
```

