# CPU/GPU Quantum Simulator Benchmark: Experimental Dataset

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC--BY--4.0-lightgrey.svg)](LICENSE)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21189705.svg)](https://doi.org/10.5281/zenodo.21189705)

This repository contains the complete experimental datasets accompanying the paper

> **Application-Oriented Evaluation of CPU/GPU Quantum Simulators: From Canonical Quantum Circuits to Molecular Simulation**

The repository provides the raw benchmark outputs used to generate every figure, table, and statistical analysis presented in the manuscript.

---

# Repository Structure

```
qsim-benchmark-data/
│
├── data/
│   ├── exp1_ghz/
│   │   ├── nvidia_fp32_ghz_results.csv
│   │   ├── nvidia_fp64_ghz_results.csv
│   │   ├── nvidia_qpp-cpu_ghz_results.csv
│   │   ├── qiskit_aer_ghz_results.csv
│   │   └── qiskit_svs_ghz_results.csv
│   │
│   ├── exp2_qft_mirror/
│   │   ├── cudaq_qft_mirror.csv
│   │   └── qiskit_qft_mirror.csv
│   │
│   ├── exp3_vqe_h2/
│   │   └── vqe_h2.csv
│   │
│   ├── exp4_vqe_ansatz/
│   │   ├── cudaq_vqe_uccsd_benchmark_results.csv
│   │   ├── cudaq_vqe_lcnot_uccsd_benchmark_results.csv
│   │   ├── qiskit_vqe_uccsd_benchmark_results.csv
│   │   └── qiskit_vqe_lcnot_uccsd_benchmark_results.csv
│   │
│   ├── exp5_sampling_hchains/
│   │   ├── cudaq_sampling_lcnot_uccsd_benchmark_results.csv
│   │   └── qiskit_sampling_lcnot_uccsd_benchmark_results.csv
│   │
│   └── exp6_n2_pes/
│       ├── N2_cc-pvdz_cudaq_qsci_rbm_lcnot_uccsd_cas10_16_results.csv
│       └── N2_cc-pvdz_cudaq_pes_sqd_lcnot_uccsd_cas10_16_results.csv
│
├── HARDWARE.md
├── environment.yml
├── requirements.txt
├── LICENSE
└── CITATION.cff
```

---

# Dataset Contents

The repository contains benchmark data from six experimental studies.

| Experiment | Description |
|------------|-------------|
| **Experiment 1** | GHZ-state simulation performance on CPU and GPU backends |
| **Experiment 2** | Quantum Fourier Transform (QFT) mirror-circuit benchmarking |
| **Experiment 3** | Variational Quantum Eigensolver (VQE) for molecular hydrogen using CUDA-Q and CUDAQ-X |
| **Experiment 4** | UCCSD and LCNOT-UCCSD ansatz benchmarking across CUDA-Q and Qiskit |
| **Experiment 5** | Quantum circuit sampling benchmarks using LCNOT-UCCSD circuits |
| **Experiment 6** | Nitrogen (N₂) potential energy surface calculations using SQD and QSCI workflows |

The CSV files contain the raw measurements used for statistical analysis and figure generation in the accompanying publication.

---

# Software Environment

The software environment used to generate these datasets is provided through

- `environment.yml`
- `requirements.txt`

to facilitate reproducibility.

---

# Hardware

Detailed hardware specifications for every benchmark are provided in

```
HARDWARE.md
```

This includes CPU, GPU, and memory information used throughout the study.

---

# License

This dataset is distributed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

See the `LICENSE` file for details.

---

# Citation

If you use this dataset in your research, please cite both the accompanying publication and this archived dataset.

**Dataset DOI**

https://doi.org/10.5281/zenodo.21189705

GitHub provides a formatted citation via the **"Cite this repository"** button, while Zenodo provides BibTeX, RIS, and other citation formats.

---
