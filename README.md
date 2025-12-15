# CogMap Paper Repository

[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.neuropsychologia.2025.109290-blue)](https://doi.org/10.1016/j.neuropsychologia.2025.109290)

Welcome to the repository for ***"Formation of allocentric representations after exposure to a novel, naturalistic, city-like, virtual reality environment"*** (also nicknamed the NPRL "CogMap Paper"). 

The project examines how individuals develop allocentric (i.e., world-centered) spatial representations after exploring a novel, virtual reality, city-like environment.

## What's Here?

This repository contains all **analysis code, figures, and statistical tests** associated with this study. 

All **data** for this paper can be found on the associated [CogMap OSF Project](https://osf.io/7dfcu/overview).

Below is an explanation of the folder structure in this repository. Feel free to reach out to the Neural Plasticity Research Lab via our [website](https://npresearchlab.com) or contact Yasmine Bassil at [ybassil@emory.edu](mailto:ybassil@emory.edu) with any questions.

## Paper Info

> Bassil, Y., Kanukolanu, A., Funderburg, E., Brown, T., & Borich, M. R. (2026). Formation of allocentric representations after exposure to a novel, naturalistic, city-like, virtual reality environment. *Neuropsychologia, 220,* 109290. https://doi.org/10.1016/j.neuropsychologia.2025.109290

**Authors**: Yasmine Bassil, Anisha Kanukolanu, Emma Funderburg, Thackery Brown, Michael R. Borich
**Affiliation**: Neural Plasticity Research Lab, Emory University  
**Contact**: Dr. Michael Borich, PhD, DPT, PT ([mborich@emory.edu](mailto:mborich@emory.edu))  
**Lab Website**: [npresearchlab.com](https://npresearchlab.com)

---

## Table of Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Data](#data)
- [Code](#code)
- [Figures](#figures)
- [Requirements](#requirements)
- [Usage](#usage)
- [Citation](#citation)
- [License](#license)

---

## Overview

This repository provides complete reproducibility materials for our study examining the formation of allocentric (i.e., world-centered) spatial representations following exposure to a novel, naturalistic, city-like virtual reality environment (*NavCity*). The study investigates how individuals develop cognitive maps and acquire spatial knowledge through immersive navigation training in an ecologically valid virtual environment.

**Key Features:**
- Complete analysis pipeline from raw data to final figures
- Statistical analysis scripts
- Publication-ready figures

---

## Repository Structure

```
CogMap-Paper/
│
├── data_analysis/            # Data processing and analysis scripts
│   └── 0_runall.ipynb        # Master script to process all raw data
│   └── 1_calculate_outcomes.ipynb  # Calculates outcome measures from raw data
│   └── 2_merge_data.ipynb    # Collects outcome measures per block per participant in one dataframe
│   └── 3_average_data.ipynb  # Averages outcome measures over blocks per participant
│   └── 4_target_data.ipynb   # Creates dataframes for overall paths per block across participants
│   └── 5_graph_data.ipynb    # Creates overhead path map figures per block across participants
│   └── 6_post_analyses.ipynb # Cleans up data based on documented errors during data collection
|
├── figure_creation/          # Scripts to generate manuscript figures
│
├── final_figures/            # Publication-ready figures (output)
│
├── stat_tests/               # Statistical analysis scripts
│
├── .gitignore
├── LICENSE
└── README.md
```

---
## Data

### `data/`

All data for this paper can be found on the associated [CogMap OSF Project](https://osf.io/7dfcu/overview).

---

## Code

### `data_analysis/`

Contains scripts for processing and analyzing raw data from the *NavCity* task and other behavioral measures. These scripts generate the outcome variables and performance metrics used in the main analyses.

### `figure_creation/`

Contains all scripts used to generate the main figures that appear in the published paper. Each script corresponds to a specific figure and produces publication-ready visualizations.

### `other_figures/`

Contains supplementary figures, exploratory analyses, and additional visualizations that may not appear in the main manuscript but were created during the analysis process.

### `stat_tests/`

Contains scripts for all statistical tests reported in the paper, including:
- Hypothesis testing
- Model comparisons
- Post-hoc analyses
- Statistical validations

### `writing/`

Contains manuscript drafts, supplementary materials, and other written components related to the paper.

---

## Related Resources

For the NavCity Toolkit (including task source code, executable files, and implementation details), please visit:
- [NavCity Toolkit Repository](https://github.com/npresearchlab/NavCity_Toolkit)

---

## Citation

If you use this code or data in your research, please cite:

> [Citation to be added upon publication]

---

## Contact

For questions or collaboration inquiries:
- **Yasmine Bassil** - [ybassil@emory.edu](mailto:ybassil@emory.edu)
- **Neural Plasticity Research Lab** - [npresearchlab.com](https://npresearchlab.com)