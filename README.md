# RBM

This repository contains codes for training a Restricted Boltzmann Machine (RBM) to represent arbitrary ground states of the toric code.

## Overview

### File Structure
- **RBM/**: Contains standalone codes for training and verifying RBM models.
  - **RBM_search.ipynb**: This script searches for solutions using randomly generated initial parameters, aiming to avoid being stuck in local minima.
  - **RBM_verify.ipynb**: Demonstrates a specific example of the ground state: $|GS\rangle = \frac{1}{\sqrt{30}} \big(|00\rangle + 2|01\rangle + 3|10\rangle + 4|11\rangle\big)$,
    where each $|ij\rangle\$ is a basis state of the ground state. The optimization process uses PyTorch's Adam Gradient Descent method.

- **FRRBM/**: Contains the original implementation designed for Google Colab.

### Highlights
- **RBM_search** helps explore diverse solutions by initializing parameters randomly.
- **RBM_verify** focuses on verifying the representation of a specific ground state.
- Utilizes PyTorch's Adam optimizer to perform gradient descent efficiently.

## Getting Started

1. Clone this repository:
   ```bash
   git clone <repository_url>
   ```
2. Navigate to the desired folder (e.g., `RBM/` or `FRRBM/`) and open the corresponding `.ipynb` file in Jupyter Notebook or JupyterLab.
3. Run the cells to perform training or verification.

## Requirements

- Python 3.8+
- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook (optional for `.ipynb` files)
