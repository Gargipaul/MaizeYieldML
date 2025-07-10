# MaizeYieldML 🌽

A machine learning pipeline for predicting yield-related traits in maize using RandomForest and XGBoost regressors, with SHAP-based feature importance analysis.

## 📊 Project Overview

This project includes:
- Training RandomForest and XGBoost models on maize phenotype data
- SHAP analysis to interpret model predictions
- Feature selection to simplify models
- Comparison of full vs. simplified models
- Saving models and SHAP outputs for reuse

## 🧪 Key Features
- SHAP for model explainability
- RMSE and R² performance metrics
- Plot saving and feature ranking
- Cleaned feature names for model compatibility

## 📁 Project Structure

```
📁 MaizeYieldML/
│
├── 📁 data/             # Raw input data (not uploaded)
├── 📁 output/           # SHAP plots, top features, predictions
├── 📁 models/           # Saved models (XGBoost, RandomForest)
├── 📁 notebooks/        # Jupyter Notebooks for model training & analysis
├── 📁 src/              # Optional: Python utility functions
│
├── 📄 README.md         # Project documentation
├── 📄 requirements.txt  # Python package dependencies
└── 📄 .gitignore         # Files excluded from version control

```
## 📁 Data Source  
The datasets used in this project are sourced from the **Genomes to Fields (G2F) Initiative**, which provides publicly available phenotypic, genotypic, environmental, and metadata from maize field trials across North America.

Specifically, this project utilizes data from the **2022 field season**, released as part of the G2F Genotype × Environment (G×E) prediction competition. Data include environmental covariates, genotypes, phenotypes, and metadata.

📚 Citation:  
> Lima, D. C., Washburn, J. D., Varela, J. I., et al. (2023).  
> *Genomes to Fields 2022 Maize Genotype by Environment Prediction Competition.*  
> BMC Research Notes, 16:148.  
> [https://doi.org/10.1186/s13104-023-06421-2](https://doi.org/10.1186/s13104-023-06421-2)

📎 Access:  
[https://www.genomes2fields.org/resources/](https://www.genomes2fields.org/resources/)




## 🔧 Setup Instructions

1. Clone the repo:
   git clone https://github.com/YOUR_USERNAME/MaizeYieldML.git
   cd MaizeYieldML
2. Install dependencies:
   pip install -r requirements.txt
3. Open and run the Jupyter notebook in /notebooks.

```
| Model                     | RMSE  | R² Score |
| ------------------------- | ----- | -------- |
| RandomForest (Full)       | 14.70 | 0.7923   |
| RandomForest (Simplified) | 15.09 | 0.781    |
| XGBoost (Full)            | 16.75 | 0.7302   |
| XGBoost (Simplified)      | 16.88 | 0.726    |

```

## 🔧 Setup Instructions

1. Clone the repo:
   git clone https://github.com/YOUR_USERNAME/MaizeYieldML.git  
   cd MaizeYieldML  
2. Install dependencies:  
   pip install -r requirements.txt  
3. Open and run the Jupyter notebook in /notebooks.


## 📄 License
This project is open-source under the MIT License.

## 🤝 Acknowledgements
This work contributes to advancing ML-based phenotyping in plant science.  
Special thanks to the **Genomes to Fields (G2F) Initiative** for providing the maize dataset used in this project.  
SHAP interpretation was key to identifying important phenotypic drivers.





