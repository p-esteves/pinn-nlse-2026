# PINN for Nonlinear Schrödinger Equation

Official code for the paper: **"Robust Physics Discovery from Highly Corrupted Data: A PINN Framework Applied to the Nonlinear Schrödinger Equation"**
[![arXiv](https://img.shields.io/badge/arXiv-2601.04176-b31b1b.svg)](https://arxiv.org/abs/2601.04176)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

**Author:** Pietro Esteves  
**Affiliation:** Federal University of Ceará (UFC)  
**Contact:** pietro.e@alu.ufc.br

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

