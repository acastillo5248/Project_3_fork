# **Project 3: notebooks**

Reducing Uncertainty in Ocean Carbon Reconstructions

Main notebook is titled Final_notebook.ipynb

Objective:
This project aims to improve the reconstruction of surface ocean partial pressure of CO₂ (pCO₂) by testing various machine learning models and methods like ffn-cnn, random forest, transformer based regression, temporal residual analysis, and different masking techniques to address the challenges posed by sparse observational data. Ocean carbon uptake is crucial for mitigating climate change, but current datasets, such as SOCAT, cover only a small fraction of the ocean, particularly in hard-to-access regions like the Southern Ocean. The goal is to reduce uncertainty in global ocean carbon flux reconstructions by improving data coverage, exploring new machine learning techniques, and analyzing temporal responses to atmospheric drivers.

Approaches:
Improving Spatial Coverage:

We simulate expanded observational coverage, especially in the Southern Ocean, to test whether increased data density reduces bias in pCO₂ reconstructions.

Models used: SOM-FFN, XGBoost, and Random Forest, Temporal Analsysis + XGB, Extended Mask + XGB.

Testing Model Alternatives:

Evaluation of tree-based models (XGBoost, RF) and deep learning models (CNNs, RNNs, Transformers) to better capture spatiotemporal dependencies.

Understanding Temporal Response:

Investigation of how surface ocean pCO₂ responds to atmospheric drivers using lagged correlation and Granger causality analysis.

Focus on identifying regional differences in carbon uptake dynamics.

Expected Outcome:
By improving spatial data density, testing alternative machine learning models, and analyzing temporal responses, this project seeks to reduce uncertainties in ocean carbon flux reconstructions, thus enhancing our understanding of long-term climate dynamics and air-sea CO₂ exchange.


Contributing
Team Contributions:
Kihyun Jye: Responsible for testing, including pre-processing data, training, and evaluating different models (ie random forests) for potential use in the final pipeline.

Yutong Uwang: Contributed to dataset exploration, model selection, and result interpretation. Assisted in the implementation of preprocessing steps and model validation.

Martin Celedon : Played a key role in the analysis of model results and performance metrics and the construction of the Temporal Response and the correlation of the optimal lag. Also contributed to the visualization and interpretation of the reconstructed data.

Alessandro Castillo: Helped in the development of the spatial and temporal analysis techniques, as well as in refining model selection and data visualization methods. Developed training and reconstruction loops as well as final visualizations. Integrated different finalized methods into single pipeline.

How to Run the Notebooks
Clone the Repository:

Use git clone https://github.com/your-github-repo.git to clone the repository.

Install Dependencies:

Install the necessary Python packages as listed in the requirements.txt.

Run the Data Notebook then Final Notebook:

After running the data notebook run the final notebook. both are in the notebooks folder. This notebook includes everything you need to train models, evaluate them, and generate the results.

Explore the Data Notebook:

If you'd like to modify or analyze the raw data, Project3_Data.ipynb will guide you through accessing the raw ESM data and preprocessing it into a format suitable for machine learning.

Future Work
Increase Data Coverage:

We plan to extend the analysis to include more ensemble members and models for a broader range of climate scenarios.

Advanced Model Techniques:

Explore other machine learning methods like neural networks or deep learning models to improve reconstruction accuracy.

Fine-tuning:

Further optimize model parameters and assess the impact of different preprocessing techniques on model performance.