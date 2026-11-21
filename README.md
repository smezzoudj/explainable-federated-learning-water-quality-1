# Explainable Federated Learning for Surface Water Quality Forecasting Across Heterogeneous Monitoring Networks

## Overview

This repository contains the experimental notebooks and supporting materials developed for the research study:

**“An Explainable Federated Learning Framework for Surface Water Quality Forecasting Across Heterogeneous Monitoring Networks.”**

The study investigates federated learning for surface water quality forecasting across heterogeneous monitoring networks. It examines recurrent and Transformer-based models, compares them with classical machine learning baselines, and uses explainable artificial intelligence techniques to analyze model behavior.

The repository is intended to support transparency and inspection of the experimental workflow. Please consult the notebooks and the associated article for the exact implementation details and reported results.

## Research Objectives

The main objectives of this study are to:

- Develop an explainable framework for next-month surface water quality forecasting using heterogeneous multi-country monitoring data.
- Compare three learning strategies: local, centralized, and federated learning under consistent preprocessing, training, and chronological evaluation protocols.
- Benchmark classical machine learning models, including Logistic Regression, Random Forest, XGBoost, and CatBoost.
- Evaluate deep learning architectures, including Gated Recurrent Unit (GRU), Long Short-Term Memory (LSTM), and Transformer, across different learning strategies.
- Assess predictive performance using the evaluation metrics defined in the study, with particular emphasis on Macro-F1.
- Investigate model interpretability through SHAP-based global and temporal analyses to identify influential physicochemical variables and historical observations.
- Conduct ablation experiments to examine the effects of learning strategy, neural architecture, data heterogeneity, class imbalance, and repeated-value patterns on forecasting performance.
- Analyze the influence of data characteristics, model architecture, and learning strategy on forecasting performance across heterogeneous monitoring networks.

## Repository Contents

The following Jupyter notebooks are included:

| File | Purpose |
|---|---|
| `01-eda.ipynb` | Exploratory data analysis |
| `02-preprocess.ipynb` | Data preprocessing |
| `03-gru-baselines.ipynb` | GRU baseline experiments |
| `04-lstm-baselines.ipynb` | LSTM baseline experiments |
| `05-transformer-baselines.ipynb` | Transformer baseline experiments |
| `06-confusion-matrices.ipynb` | Confusion-matrix analysis |
| `07-overfitting-evidence.ipynb` | Overfitting analysis |
| `08-classical-ml-baselines.ipynb` | Classical machine learning baselines |
| `09-final-comparison.ipynb` | Final model comparison |
| `10-shap-xai.ipynb` | SHAP-based explainability analysis |
| `11-ablation-study.ipynb` | Ablation study |

Supplementary ZIP archives containing experiment outputs may also be provided in the repository.

## Experimental Workflow

The notebooks are organized around the following workflow:

1. Exploratory analysis of the dataset.
2. Data preprocessing and preparation.
3. GRU, LSTM, and Transformer baseline experiments.
4. Classical machine learning baseline experiments.
5. Confusion-matrix and overfitting analyses.
6. Explainability analysis using SHAP.
7. Ablation experiments.
8. Final comparison of the evaluated models.

Run the notebooks in numerical order where later experiments depend on files or outputs produced by earlier notebooks.

## Models and Methods

The notebooks cover the following model families and methods:

- Gated Recurrent Unit (GRU)
- Long Short-Term Memory (LSTM)
- Transformer-based models
- Classical machine learning baselines
- Federated learning experiments
- SHAP-based explainable AI
- Ablation analysis

Refer to the corresponding notebooks and the research article for the precise model configurations, federated learning setup, hyperparameters, and evaluation protocol.
## Dataset

The study uses the publicly available **A Comprehensive Surface Water Quality Monitoring Dataset (1940–2023)**, introduced by Karim et al. (2025).

- **Dataset repository:** https://figshare.com/articles/dataset/A_Comprehensive_Surface_Water_Quality_Monitoring_Dataset_1940-2023_2_82Million_Record_Resource_for_Empirical_and_ML-Based_Research/27800394
- **Dataset DOI:** https://doi.org/10.6084/m9.figshare.27800394.v2
- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

The dataset contains approximately 2.82 million observations from five countries: the United States, Canada, England, Ireland, and China, covering the period 1940–2023.

The dataset is not included in this repository. Download it from the official Figshare repository and comply with its attribution and license requirements.

Before running the notebooks, update the dataset paths to match your local environment.

## Requirements

The experiments use Python and Jupyter notebooks. Install the package dependencies required by the notebooks before execution.

A `requirements.txt` file should be provided with the exact package names and versions used for the final experiments. Do not assume that a generic list of libraries is a substitute for the verified environment.

## Running the Notebooks

1. Clone or download this repository.
2. Create and activate a Python environment.
3. Install the dependencies listed in `requirements.txt` (when provided).
4. Obtain the dataset from its authorized source.
5. Configure the dataset paths in the notebooks or configuration files.
6. Launch Jupyter Notebook or JupyterLab.
7. Execute the notebooks in numerical order, checking each notebook's input requirements.

Some notebooks may rely on intermediate files generated by earlier steps. Check the notebook instructions before running an experiment independently.

## Results

The notebooks contain the procedures and outputs for the experiments listed above. For the definitive numerical results, experimental settings, and interpretation, refer to the corresponding tables, figures, and discussion in the research article.

Ensure that the code and outputs in this repository match the version of the experiments reported in the article before citing this repository as the source of the published results.

## Reproducibility Notes

For reproducible execution:

- Use the dataset version and preprocessing procedure described in the article.
- Preserve the experimental data splits and random seeds, where specified.
- Use the documented model configurations and hyperparameters.
- Record the Python and library versions.
- Follow the notebook execution order and retain required intermediate outputs.

Any details not explicitly documented in the notebooks or configuration files should be checked against the research article.

## Citation

If you use this code, please cite the associated research article.

The bibliographic information should be completed once the article's publication details are available.

```bibtex
@article{mezzoudj2026explainable,
  title   = {{An Explainable Federated Learning Framework for Surface Water Quality Forecasting Across Heterogeneous Monitoring Networks}},
  author  = {MEZZOUDJ, Saliha and
             HADDOUDA, Sara and
             CHEBLAL, Hibatallah and
             SAADNA, Yassmina and
             Zahary, Ammar Thabit and
             KHELIFA, Meriem},
  journal = {Scientific Reports},
  year    = {2026},
  doi     = {To be assigned}
}
```

## Code Availability

The source code and experimental notebooks are made available in this repository for inspection of the computational workflow associated with the study. The repository contents and instructions should be checked against the final published version of the article.

## License

Add a `LICENSE` file specifying the terms under which this code may be used, modified, and redistributed. Do not select a license unless you have the right to grant those permissions and any institutional or co-author requirements have been checked.

## Contact

For questions about the implementation or research, use the corresponding author's contact information provided in the associated article.
