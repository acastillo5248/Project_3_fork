# **Project 3: notebooks**

Reducing Uncertainty in Ocean Carbon Reconstructions


Objective:
This project aims to improve the reconstruction of surface ocean partial pressure of CO₂ (pCO₂) using machine learning models to address the challenges posed by sparse observational data. Ocean carbon uptake is crucial for mitigating climate change, but current datasets, such as SOCAT, cover only a small fraction of the ocean, particularly in hard-to-access regions like the Southern Ocean. The goal is to reduce uncertainty in global ocean carbon flux reconstructions by improving data coverage, exploring new machine learning techniques, and analyzing temporal responses to atmospheric drivers.

Approaches:
Improving Spatial Coverage:

We simulate expanded observational coverage, especially in the Southern Ocean, to test whether increased data density reduces bias in pCO₂ reconstructions.

Models used: SOM-FFN, XGBoost, and Random Forest.

Testing Model Alternatives:

Evaluation of tree-based models (XGBoost, RF) and deep learning models (CNNs, RNNs, Transformers) to better capture spatiotemporal dependencies.

Understanding Temporal Response:

Investigation of how surface ocean pCO₂ responds to atmospheric drivers using lagged correlation and Granger causality analysis.

Focus on identifying regional differences in carbon uptake dynamics.

Expected Outcome:
By improving spatial data density, testing alternative machine learning models, and analyzing temporal responses, this project seeks to reduce uncertainties in ocean carbon flux reconstructions, thus enhancing our understanding of long-term climate dynamics and air-sea CO₂ exchange.


Contributing
Team Contributions:
Kihyun: Responsible for implementing the machine learning models, including pre-processing data, training, and evaluating models, as well as preparing the analysis of ocean pCO₂ reconstruction.

Sylvia: Contributed to dataset exploration, model selection, and result interpretation. Assisted in the implementation of preprocessing steps and model validation.

Martin: Played a key role in the analysis of model results and performance metrics. Also contributed to the visualization and interpretation of the reconstructed data.

Alessandro: Helped in the development of the spatial and temporal analysis techniques, as well as in refining model selection and data visualization methods.

How to Run the Notebooks
Clone the Repository:

Use git clone https://github.com/your-github-repo.git to clone the repository.

Install Dependencies:

Install the necessary Python packages as listed in the requirements.txt.

Run the Starter Notebook:

Start with Project3_Starter.ipynb to run the machine learning pipeline.

This notebook includes everything you need to train models, evaluate them, and generate the results.

Explore the Data Notebook:

If you'd like to modify or analyze the raw data, Project3_Data.ipynb will guide you through accessing the raw ESM data and preprocessing it into a format suitable for machine learning.

Future Work
Increase Data Coverage:

We plan to extend the analysis to include more ensemble members and models for a broader range of climate scenarios.

Advanced Model Techniques:

Explore other machine learning methods like neural networks or deep learning models to improve reconstruction accuracy.

Fine-tuning:

Further optimize model parameters and assess the impact of different preprocessing techniques on model performance.