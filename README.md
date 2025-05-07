## Harmonic Zeta Sieve

Modular harmonic sieve for detecting nontrivial Riemann zeta zeros through phase-locked resonance analysis. This project provides code and data for independent verification of the harmonic sieve described in the paper:

Sadie A. Sherratt (2025).Phase-Locked Modular Resonance and the Structure of Zeta Zeros.

## 📄 Overview

This repository includes the full data bundle for the harmonic sieve model, designed to detect nontrivial Riemann zeta zeros using a phase-locked modular resonance approach. This approach leverages the interplay between base-3 and base-π logarithmic spirals to identify resonance points where zeta zeros align, without relying on statistical approximations.

Key Features:

- Fast, scalable zero detection using modular harmonic resonance.

- Precomputed datasets for efficient verification without full recalculation.

- Structured for direct use in numerical experiments and algorithm development.

---

## 📄 Contents

- **/data/** — Numpy arrays and parameter sets used in the sieve
- **/results/** — Sieve validation and false positive report
- **/zeros/** — Archive of known zeta zeros used for validation
- **README.md** — This documentation file
- **LICENSE.txt** — License for academic use

---

## 📈 Purpose

This bundle provides the datasets necessary to reproduce the harmonic sieve validation described in the paper:

- Modular drift between base-3 and base-\(\pi\) logarithmic spirals.
- Dynamic harmonic envelope structure isolating resonance points.
- Modular sieve construction confirming alignment with known zeta zeros up to high \(t\).

The datasets allow independent verification of the modular geometric model without requiring full recalculation.

---

## 📋 File Types

- `.npy` — Numpy array files storing drift, envelope, or symbolic modular quantities.
- `.txt` — Documentation or symbolic tables describing the dataset structure.
- `.txt` — List of known nontrivial zeta zeros used for empirical validation.

---

## ⚙️ Requirements

- Python 3.8+ recommended
- Library:
  - `numpy`

*No special or proprietary packages are needed to load or use the data.*

---
## Quickstart:

To load the included data files:

```python
import numpy as np

# Load the primary sieve data
sieve_data = np.load('data/sieve_parameters.txt')
zeros = np.load('zeros/zeros1.gz')

data_band = np.load('data/within_band_mask.npy')

print(f"Loaded {len(zeros)} known zeros.")
```

This snippet demonstrates loading the core sieve data and known zero files for quick inspection. For more detailed usage, refer to the accompanying paper.

---

## 📜 License

This bundle is released for non-commercial research and educational purposes only.  
Please cite the associated paper if used in derived works.

---

## 📬 Contact

For questions, updates, or related inquiries:

**Sadie A. Sherratt**  
Website: [https://sherrattmath.org](https://sherrattmath.org)  
Email: sadie@sherrattmath.org

---
