# Human Activity Recognition using data from Smartphones
This project is a part of the CAPSTONE course during my Master's at Penn State University.

#### -- Project Status: [Completed]

## Project Objective
The purpose of this project is to classify Human Activities based on data collected from the accelerometer and gyroscope sensors of a smartphone. The focus of this project will be on finding the optimum number of features for the classification task followed by a comparison of traditional ML techniques.

### Partner
* Parva Jain
* Dominic Thomas

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization

### Technologies
* Python
* Jupyter

## Project Description
* **Goal:** The goal of the project was to find which traditional ML technique performs better for the classification of human activities based on accelerometer and gyroscope data from smartphones.
* **Data Source:** [Kaggle](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones)
* **Data Preparation:** As the dataset has 571 features with no inconsistencies or missing values no actual data cleaning was required.
* **Dimension Reduction:**
  * For dimension reduction, we have tried two techniques, namely Factor Analysis and Principal Component Analysis (PCA).
  * Out of which PCA performed significantly better than Factor Analysis. As a result, we decided to proceed with PCA.
  * Using PCA we were able to reduce 571 features into 9 components which explained 79.6458% of the variation in data
* **Modeling:** For the classification task we chose two traditional and two ensemble machine learning techniques namely Multinomial Logistic Regression, Support Vector Machine(SVM), Random Forest Classifier, and XGBoost Classifier.
* **Outcome:** Results from the 4 models average around 86% accuracy with a variance of 1% suggesting that models are good enough for classification purposes with Multinomial Logistic Regression performing better by 0.5%.

## Needs of this project
- data exploration/descriptive statistics
- data processing/cleaning
- dimension reduction
- statistical modeling
- writeup/reporting

## Getting Started
1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](/Data/) within this repo.    
3. Scripts for finding the optimal number of principal components for classification tasks are kept [here](/PCA/).

## Featured Notebooks
* [Base](/HAR_base.ipynb) This is the base notebook for the project.
* [PCA_Evaluation](/PCA/PC_Evaluation.ipynb) This notebook contains code for generating accuracies of different models (chosen for this project) for a range of principle components and storing them in log_file(/PCA/pca_log.txt).
* [PCA_Graph](/PCA/PC_Graph.ipynb) This notebook contains code to generate the PC graph (accuracy of selected models vs no. of principle components) which can be used to choose the optimal no. of principle components for the classification task.

## Contact
Feel free to contact me with any questions via [LinkedIn](https://www.linkedin.com/in/akshay2718/)