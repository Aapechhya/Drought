# Mustang Hydroclimatic Analysis

Reproducible analysis code for assessing hydroclimatic variability, trends, drought conditions, and projected drought changes in Mustang, Nepal.

## Analysis workflow

Run the notebooks in the following order:

1. `01_precipitation_bias_correction.ipynb`
2. `02_temperature_bias_correction.ipynb`
3. `03_temperature_trend_analysis.ipynb`
4. `04_historical_drought_indices.ipynb`
5. `05_cmip6_drought_projections.ipynb`
6. `06_ERA5Land_Comparison_FIXED.ipynb`

## Repository structure

```text
.
├── notebooks/
│   ├── 01_precipitation_bias_correction.ipynb
│   ├── 02_temperature_bias_correction.ipynb
│   ├── 03_temperature_trend_analysis.ipynb
│   ├── 04_historical_drought_indices.ipynb
│   └── 05_cmip6_drought_projections.ipynb
        `06_ERA5Land_Comparison_FIXED.ipynb`
├── data/
│   ├── raw/
│   ├── observations/
│   ├── processed/
│   └── cmip6/
├── results/
├── requirements.txt
├── CITATION.cff
├── LICENSE
├── .gitignore
└── README.md
```

Large input datasets and generated results are intentionally excluded from this repository. See the Data availability section below.

## Requirements

Python 3.10 or newer is recommended.

Install the required packages with:

```bash
pip install -r requirements.txt
```

The notebooks can then be opened and executed with Jupyter Notebook or JupyterLab.

## Data availability

The analysis uses observational, reanalysis, and CMIP6 climate datasets. These datasets are not redistributed in this repository where their respective data-use or distribution conditions do not permit redistribution.

Users should obtain the required source datasets from their original providers and place them in the corresponding directories under `data/`.

The exact input filenames and expected directory locations are specified in the configuration cells of the notebooks.

## Reproducibility

This repository contains the analysis workflow and code used to process the climate data and calculate the reported results. Because the source datasets are maintained by their respective data providers, users should download the appropriate versions of those datasets before running the workflow.

## Citation

If you use this code, please cite the repository using the information in `CITATION.cff`.

A DOI will be added automatically by Zenodo after the GitHub repository is connected and a release is archived.

## License

The code in this repository is released under the MIT License. See `LICENSE` for details.
