# **Project 3: notebooks**

IF YOU ARE IN THE ROOT DIRECTORY. PLEASE NAVIGATE TO PROJECT-STARTCODES/PROJECT3-RECONSTRUCTPCO2

Reducing Uncertainty in Ocean Carbon Reconstructions

## What notebooks to run
Main notebook is titled Final_notebook.ipynb in notebooks folder. May need to run Project3_Data notebook first. These are in notebooks folder.

## Objective:
This project aims to improve the reconstruction of surface ocean partial pressure of CO₂ (pCO₂) by testing various machine learning models and methods like ffn-cnn, random forest, transformer based regression, temporal residual analysis, and different masking techniques to address the challenges posed by sparse observational data. We take our best performing methodologies and combine them into a single pipeline in Final_notebook where the new methodology is compared against the base xgb model. The driving force behind this ressearch is that ocean carbon uptake is crucial for mitigating climate change, but current datasets, such as SOCAT, cover only a small fraction of the ocean, particularly in hard-to-access regions like the Southern Ocean. This limited data acces makes training complex models that normally require a lot of data like XGB difficult. This is why our goal is to reduce uncertainty in global ocean carbon flux reconstructions by improving data coverage, exploring novel machine learning techniques, and analyzing temporal responses to atmospheric drivers. We hope that by testing various methods then merging the best performing one's into a single pipeline that we can make up for sparse data, and improve on a base XGB model. 

## Approaches:
Improving Spatial Coverage:

- We simulate expanded observational coverage, especially in the Southern Ocean, to test whether increased data density reduces bias in pCO₂ reconstructions.

Models used for improvement tests: 

- SOM-FFN, XGBoost, and Random Forest, Temporal Analsysis + XGB, Extended Mask + XGB.

- Base Model for Comparison: Standard XGB with SOCAT mask

Testing Model Alternatives:

- Evaluation of tree-based models (XGBoost, RF) and deep learning models (CNNs, RNNs, Transformers) to better capture spatiotemporal dependencies.

Understanding Temporal Response:

- Investigation of how surface ocean pCO₂ responds to atmospheric drivers using lagged correlation and Granger causality analysis.

- Focus on identifying regional differences in carbon uptake dynamics.

Final Approach:

- We take our best performing test approaches (ie extended mask and temporal lag analysis) and create a pipeline that tests this new method against the base XGB model

## Expected Outcome:
By improving spatial data density, testing alternative machine learning models, and analyzing temporal responses, this project seeks to reduce uncertainties in ocean carbon flux reconstructions, thus enhancing our understanding of long-term climate dynamics and air-sea CO₂ exchange as well as improving upon the base xgb model. 

## Key Findings:
Our comparative analysis demonstrated that while Transformer and deep learning approaches showed promise for capturing complex spatiotemporal patterns, the combination of XGBoost with temporal lag analysis and an extended spatial mask delivered the most consistent performance improvements across all evaluation metrics. This integrated approach significantly reduced mean bias error and improved correlation across seasonal, sub-seasonal, and decadal timescales.

## Team Contributions:
Kihyun Jye: Responsible for testing, including pre-processing data, training, and evaluating different models (ie random forests) for potential use in the final pipeline.

Yutong Uwang: Contributed to dataset exploration, model selection, and result interpretation. Assisted in the implementation of preprocessing steps and model validation.

Martin Celedon : Played a key role in the analysis of model results and performance metrics and the construction of the Temporal Response and the correlation of the optimal lag. Also contributed to the visualization and interpretation of the reconstructed data.

Alessandro Castillo: Helped in the development of the spatial and temporal analysis techniques, as well as in refining model selection and data visualization methods. Developed training and reconstruction loops as well as final visualizations. Integrated different finalized methods into single pipeline.

## Other 

Install Dependencies:

Install the necessary Python packages as listed in the requirements.txt.

Run the Data Notebook then Final Notebook:

After running the data notebook run the final notebook. both are in the notebooks folder. This notebook includes everything you need to train models, evaluate them, and generate the results.

Explore the Data Notebook:

If you'd like to modify or analyze the raw data, Project3_Data.ipynb will guide you through accessing the raw ESM data and preprocessing it into a format suitable for machine learning.