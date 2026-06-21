# Water Network Leakage-Oriented SCADA Assessment Using Pump-Derived Operating Context

Reproducibility repository for the manuscript **Water Network Leakage-Oriented SCADA Assessment Using Pump-Derived Operating Context**.

## Repository structure
```text
.
├── README.md
├── LICENSE
├── environment.yml
├── requirements.txt
└── notebooks/
    ├── Leak-2018.ipynb
    └── Leak-2019.ipynb
```
## Contents

This repository contains the Jupyter notebooks used for the case study. The notebooks reproduce the empirical workflow for pump-derived operating-state construction, baseline-conditioned flow-deviation assessment, pressure-deficit assessment, leakage-oriented validation, and temporal replication.

The input data are not stored in this repository. They must be downloaded separately from the original BattLeDIM / L-Town data source and placed in the expected local data folder before running the notebooks.

## Usage

Open the notebooks in the notebooks/ folder.

Run the 2018 notebook first:
- Leak-2018.ipynb

Then run the 2019 notebook:
- Leak-2019.ipynb

The notebooks are intended to be run sequentially from top to bottom. The 2018 notebook contains the main case-study workflow, including network-based signal selection and pump-state construction. The 2019 notebook contains the temporal replication workflow using the same empirical assessment protocol.

## Data note

The case study uses the BattLeDIM / L-Town benchmark data set, including SCADA flow and pressure measurements, leakage records, and the network representation used for signal mapping and visualization. The data are not redistributed in this repository.

## Original data source

Vrachimis, S. G., Eliades, D. G., Taormina, R., Ostfeld, A., Kapelan, Z., Liu, S., Kyriakou, M. S., Pavlou, P., Qiu, M., & Polycarpou, M. M. (2020). Dataset of BattLeDIM: Battle of the Leakage Detection and Isolation Methods. Zenodo. https://doi.org/10.5281/zenodo.4017659

## Environment

The notebooks can be run either with Conda using `environment.yml` or with pip using `requirements.txt`.

Using Conda:

```bash
conda env create -f environment.yml
conda activate water-scada-leakage-pump-context
```

## Original framework source

in pub-process
