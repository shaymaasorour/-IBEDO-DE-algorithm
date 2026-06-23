# -IBEDO-DE-algorithm
# IBEDO-DE Algorithm for ChatGPT Perception Analysis in Programming Education

This repository contains the implementation, experimental notebook, and supporting files for the study:

**Optimizing Educational Analytics by Analyzing Student Perceptions of ChatGPT in Programming Education Using Enhanced Feature Selection**

The study introduces **IBEDO-DE**, an Improved Binary Exponential Distribution Optimization algorithm enhanced with Differential Evolution for wrapper-based feature selection. The framework analyzes students' perceptions of ChatGPT in programming-related learning activities using k-Nearest Neighbors (k-NN) and Support Vector Machine (SVM) classifiers.

## Overview

The proposed framework performs the following stages:

1. Questionnaire-based data preparation.
2. Feature-subset optimization using IBEDO-DE.
3. Wrapper-based evaluation using k-NN and SVM.
4. Comparative evaluation against binary metaheuristic baselines.
5. Convergence analysis and feature-importance interpretation.
6. Post-hoc Random Forest analysis for ranking the retained features.

The experimental workflow evaluates classification accuracy, fitness value, number of selected features, standard deviation, and convergence behavior.

## Repository Contents

.
├── GPT Final results (1).ipynb
├── GPT_Final_results_with_modified_Figures_2_5.ipynb
├── KNN.rar
├── SVM.rar
├── README.md


### Main Files

* `GPT_Final_results_with_modified_Figures_2_5.ipynb`
  Main experimental notebook containing the updated convergence figures and analysis workflow.

* `GPT Final results (1).ipynb`
  Supporting notebook containing the original experimental analysis.

* `KNN.rar`
  Archive containing the k-NN-related implementation files.

* `SVM.rar`
  Archive containing the SVM-related implementation files.

## Requirements

The code was developed in Python and requires the following packages:

pip install numpy pandas matplotlib seaborn scikit-learn jupyter


Recommended environment:

Python 3.9 or later
Jupyter Notebook or JupyterLab


## Data Preparation

The notebook expects the questionnaire dataset as a CSV file named:

ChatGpt Questionnaire_New.csv

Place this file in the same directory as the notebook before execution.

The dataset should contain:

* Questionnaire attributes as input features.
* A target label in the final column.
* Encoded responses derived from the survey on students' perceptions of ChatGPT in programming-related learning activities.

The dataset is not publicly included in this repository because it contains survey-based educational data. Access may be requested from the corresponding author for research purposes.

## Running the Code

1. Clone or download this repository.

2. Extract the archived implementation files:

KNN.rar
SVM.rar


3. Place the extracted files in the same working directory as the notebook.

4. Add the questionnaire CSV file:

ChatGpt Questionnaire_New.csv


5. Open the main notebook:

GPT_Final_results_with_modified_Figures_2_5.ipynb


6. Run the notebook cells sequentially.

## Methodological Workflow

The workflow begins by loading and splitting the questionnaire data into training and testing subsets. IBEDO-DE searches for informative binary feature subsets, while the wrapper fitness function balances classification error and the proportion of selected features.

The selected feature subsets are evaluated using:

* k-Nearest Neighbors classifier.
* Support Vector Machine classifier.

A post-hoc Random Forest model is then used to estimate impurity-based importance scores for the retained features. These importance scores are used for interpretation only and are not part of the IBEDO-DE optimization objective.

## Outputs

The notebook can generate:

* Feature-selection results.
* Classification accuracy values.
* Fitness values.
* Selected feature subsets.
* Feature-importance rankings.
* Confusion matrices.
* PCA-based baseline analysis.
* Convergence curves for IBEDO and IBEDO-DE.
* Updated publication-ready figures.

## Reproducibility Notes

To reproduce the reported experiments, use the same dataset structure, train-test split settings, classifier configurations, and random seeds specified in the notebook.

Some cells contain local paths used during figure preparation. Update these paths before execution when necessary.

For example, replace local image paths such as:

python
img1_path = r"C:\Users\HP\Downloads\ChatGPT\1.png"


with paths appropriate for your local environment.

## Citation

If you use this code, please cite:

Sorour, S. E., Ahmed, H. M. M., Aljaafari, M., and Abdelkader, H. E.
Optimizing Educational Analytics by Analyzing Student Perceptions of ChatGPT in Programming Education Using Enhanced Feature Selection.




