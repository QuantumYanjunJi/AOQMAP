# Algorithm-Oriented Qubit Mapping for Variational Quantum Algorithms

**This paper has been selected as an Editor's Suggestion in [Physical Review Applied](https://doi.org/10.1103/PhysRevApplied.23.034022).**

This repository implements the methods described in the paper *Algorithm-Oriented Qubit Mapping for Variational Quantum Algorithms*.

## Paper Overview

Quantum algorithms implemented on near-term devices face challenges due to noise and limited qubit connectivity, necessitating effective qubit mapping strategies. In this paper, we introduce **Algorithm-Oriented Qubit Mapping (AOQMAP)**, a novel approach designed to bridge the gap between exact and scalable mapping methods by leveraging the inherent structure of quantum algorithms.

- **Exact Methods**: These provide optimal solutions but are computationally infeasible for large circuits.
- **Scalable Methods**: Techniques like SWAP networks are fast but do not guarantee optimality.
- **AOQMAP**: Combines the strengths of both by using algorithmic features and device substructures to deliver solutions that are both **depth-optimal** and **scalable**.

AOQMAP operates in two key stages:
1. **Circuit Mapping**: Maps quantum circuits to device subtopologies (e.g., linear, T-shaped, H-shaped) to satisfy connectivity constraints.
2. **Optimal Qubit Selection and Postselection**: Uses a cost function to select the best qubits and performs postselection among execution results across subtopologies.

AOQMAP excels in handling variational quantum algorithms with fully connected two-qubit interactions. It supports common subtopologies such as:
- Linear
- T-shaped
- H-shaped

By minimizing circuit depth, AOQMAP ensures efficient execution. Benchmarking on IBM quantum devices shows remarkable improvements over existing methods like Qiskit, Tket, and SWAP networks:
- **Up to 82% reduction in circuit depth**
- **Average 138% increase in success probability**

This scalable, algorithm-specific strategy paves the way for optimizing a broader range of quantum algorithms.

## Citation
If you use AOQMAP in your work, please cite our paper:

```bibtex
@article{ji2025algorithm,
  title = {Algorithm-oriented qubit mapping for variational quantum algorithms},
  author = {Ji, Yanjun and Chen, Xi and Polian, Ilia and Ban, Yue},
  journal = {Phys. Rev. Appl.},
  volume = {23},
  issue = {3},
  pages = {034022},
  numpages = {34},
  year = {2025},
  month = {Mar},
  publisher = {American Physical Society},
  doi = {10.1103/PhysRevApplied.23.034022},
  url = {https://link.aps.org/doi/10.1103/PhysRevApplied.23.034022}
}

