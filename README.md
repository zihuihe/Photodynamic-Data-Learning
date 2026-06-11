Data and Code for Material Learning, Performance Prediction, and Iterative Optimization

Overall:This repository contains all raw experimental data and machine learning scripts used in our study on data‑driven material discovery. The materials are organized into two main parts: the experimental data (seven Excel files) that support every figure in the paper, and three notebooks that implement the core learning, prediction, and optimization workflows.  All code and data are released to ensure full reproducibility and to facilitate further reanalysis by the community.

Experimental Data

The folder includes seven separate Excel files. Each file corresponds to the original, unprocessed measurements behind a specific figure in the paper. File names follow the figure numbering (e.g., Figure_Source_Data (Figure 1), Figure_Source_Data (Figure 3), …). Within each file you will find:

• Raw electrochemical, spectroscopic, or other characterization data as recorded during the experiments.

• Processed values that were directly used for plotting.

• Brief annotations of experimental conditions and relevant metadata.

These records allow independent verification of our results and can serve as a starting point for follow‑up studies or meta‑analyses.

Machine Learning Scripts

• model_learning.ipynb: This notebook focuses on the initial stage of the workflow: data preprocessing and quantification. It takes the raw experimental data, performs cleaning and normalisation, extracts relevant features, and quantifies key material parameters. The output is a structured dataset ready for model training and prediction.

• model_prediction.ipynb: Here we compare multiple machine learning models for predicting material performance indicators. The notebook covers feature engineering, cross‑validation, model selection, and evaluation of prediction accuracy. The final output is a reliable predictive model that estimates key properties (e.g., catalytic activity or band structure parameters) for new candidate materials.

• model_training.ipynb: This script performs iterative learning on the materials that have been screened out by the predictive model. Starting from an initial set of promising candidates, the algorithm repeatedly updates its knowledge based on new experimental feedback, refines the performance estimates, and drives the search toward better materials. The notebook documents each iteration and the resulting improvement in predicted performance.
