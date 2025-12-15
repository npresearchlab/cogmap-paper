# CogMap Paper Repository

[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.neuropsychologia.2025.109290-blue)](https://doi.org/10.1016/j.neuropsychologia.2025.109290)

Welcome to the repository for the paper ***"Formation of allocentric representations after exposure to a novel, naturalistic, city-like, virtual reality environment"*** (also nicknamed the NPRL "CogMap Paper"). 

The project examines how individuals develop allocentric (i.e., world-centered) spatial representations after exploring a novel, virtual reality, city-like environment.

## What's Here?

This repository contains all **analysis code, figures, and statistical tests** associated with this study. 

All **data** for this paper can be found on the associated [CogMap OSF Project](https://osf.io/7dfcu/overview).

Below is an explanation of the folder structure in this repository. Feel free to reach out to the Neural Plasticity Research Lab via our [website](https://npresearchlab.com) or contact Yasmine Bassil at [ybassil@emory.edu](mailto:ybassil@emory.edu) with any questions.

## Citation & Details

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
- [Related Resources](#related-resources)
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
├── data_analysis/                    # Data processing and analysis scripts
│   ├── 0_runall.ipynb                # Master script to process all raw data
│   ├── 1_calculate_outcomes.ipynb    # Calculates outcome measures from raw NavCity data
│   ├── 2_merge_data.ipynb            # Merges outcome measures per block per participant
│   ├── 3_average_data.ipynb          # Averages outcome measures over blocks per participant
│   ├── 4_target_data.ipynb           # Creates dataframes for target paths per block
│   ├── 5_graph_data.ipynb            # Generates overhead path map visualizations
│   └── 6_distance_calc.ipynb         # Calculates distance-based navigation metrics
│
├── figure_creation/                  # Scripts to generate manuscript figures
│   └── plots/                        # Generated figure outputs
│
├── stat_tests/                       # Statistical analysis scripts
│   ├── fig3_4_5_stats.Rmd            # Statistical tests for Figures 3, 4, and 5
│   ├── fig6_stats.Rmd                # Statistical tests for Figure 6
│   ├── fig7_stats.Rmd                # Statistical tests for Figure 7
│   ├── nara_stats.Rmd                # NARA task correlation analyses
│   ├── updated demographic stats ANOVA.Rmd  # Demographic and group comparisons
│   ├── combined_anova_data.csv       # Processed data for ANOVA analyses
│   ├── combined_block_data.csv       # Block-level performance data
│   ├── combined_blocktarget_data.csv # Block and target-level data
│   ├── combined_target_data.csv      # Target-level performance data
│   ├── b3b1_nara_corr_data.csv       # NARA correlation dataset
│   ├── plots/                        # Statistical visualization outputs
│   ├── raw_results/                  # Raw statistical output files
│   └── summary/                      # Summary statistics and tables
│
├── writing/                          # Manuscript drafts and supplementary materials
│
├── .gitignore                        # Git ignore configuration
└── README.md                         # Repository documentation
```

---
## Data

### `data/`

All data for this paper can be found on the associated [CogMap OSF Project](https://osf.io/7dfcu/overview).

---

## Code

### `data_analysis/`

Contains scripts for processing and analyzing raw data from the *NavCity* task and other behavioral measures. These scripts generate the outcome variables and performance metrics used in the main analyses.

- **`0_runall.ipynb`**: Master orchestration script
  - Runs all analysis scripts (labeled 1 through 6) in sequence
  - Processes raw *NavCity* data files
  - Generates block-specific and session-averaged metrics
  - Outputs cleaned datasets for statistical analysis

**⚠️ Important**: This file contains hardcoded file paths. You must update file paths before running on your local machine. To get started, you may set the following:
  - Line 5: Set your local data directory for your data
  - Line 6: Set your local data directory for your code (scripts 0 through 6)

Outputs from analysis scripts will be located in the *parent directory* of the YA data and OA data, respectively.

**To Run the Complete Pipeline:**
1. Clone this repository
2. Install required packages (see [Requirements](#requirements))
3. Update file paths in `0_runall.ipynb`
4. Run all cells in `0_runall.ipynb`

### `figure_creation/`

Contains all scripts used to generate the main figures that appear in the published paper. Each script corresponds to a specific figure and produces publication-ready visualizations.

### `stat_tests/`

Contains scripts for all statistical tests reported in the paper, including:
- Running models
- Comparing outputs
- Post-hoc analyses
- Statistical validations

---

## Figures

### `/final_figures/`

This directory contains publication-ready figures in high-resolution formats (PNG, PDF, SVG).

All figures follow journal specifications:
- 300+ DPI resolution
- Colorblind-friendly palettes
- Clear axis labels and legends

---

## Related Resources

For the NavCity Toolkit (including task source code, executable files, and implementation details), please visit:
- [NavCity Toolkit Repository](https://github.com/npresearchlab/NavCity_Toolkit)

---

## Citation

If you use this code or data in your research, please cite:

> Bassil, Y., Kanukolanu, A., Funderburg, E., Brown, T., & Borich, M. R. (2026). Formation of allocentric representations after exposure to a novel, naturalistic, city-like, virtual reality environment. *Neuropsychologia, 220,* 109290. https://doi.org/10.1016/j.neuropsychologia.2025.109290

---

## License

**Data**: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) - Data are freely available with attribution

**Code**: [MIT License](LICENSE) - Code is freely available for reuse and modification

---

---

## Contributing

We welcome questions, bug reports, and suggestions for improvements. Please:

1. Check existing [Issues](https://github.com/npresearchlab/NavAging_Paper/issues)
2. Open a new issue with detailed description
3. For data questions, contact Dr. Michael Borich at mborich [at] emory.edu

---

## Acknowledgments

This research was supported by [funding sources]. We thank all study participants and the research team members who contributed to data collection and analysis.

---

## Additional Resources

- **Lab Website**: [npresearchlab.com](https://npresearchlab.com)
- **Preprint**: [CogMap Preprint](https://osf.io/preprints/psyarxiv/mrabn_v1)
- **OSF Project**: [OSF Data Repository](https://osf.io/7dfcu/overview)

---

**Last Updated**: December 2025  
**Repository Maintainer**: Yasmine Bassil, Neuroscience PhD Candidate, Neural Plasticity Research Lab, Emory University