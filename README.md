# Predictive-Machine-Maintenance-Using-Machine-Learning
# Predictive Maintenance Using Machine Learning

## Project Overview

This project focuses on developing a machine learning system that predicts potential machine failures using operational and sensor data.

The goal is to identify patterns in machine operating conditions that may indicate an upcoming failure. This can help support condition monitoring, reduce unexpected equipment downtime, and improve maintenance planning.

The project uses the **AI4I 2020 Predictive Maintenance Dataset**, obtained from Kaggle.

## Objectives

- Explore and understand predictive maintenance data.
- Perform data cleaning and preprocessing.
- Analyse the relationship between machine operating conditions and failures.
- Train and evaluate different machine learning classification models.
- Compare model performance, particularly in detecting machine failures.
- Explore future deployment as a software application and, eventually, a hardware-based monitoring system.

## Dataset

**Dataset:** AI4I 2020 Predictive Maintenance Dataset

**Source:** [Kaggle – AI4I 2020 Predictive Maintenance Dataset](https://www.kaggle.com/datasets/stephanmatzka/predictive-maintenance-dataset-ai4i-2020)

The dataset contains machine operating information, including:

- Air temperature
- Process temperature
- Rotational speed
- Torque
- Tool wear
- Machine type

The target variable is `Machine failure`, which indicates whether a machine failure occurred.

The failure-mode indicator columns were excluded from the predictive features to avoid target leakage.

**Note:** The AI4I 2020 dataset is synthetic. Results obtained from it do not, by themselves, demonstrate performance on real industrial machines.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook / Google Colab

## Machine Learning Models

The following classification models have been implemented and evaluated:

1. Logistic Regression
2. Random Forest Classifier
3. XGBoost Classifier

The dataset is highly imbalanced, with significantly more normal operating records than failure records. Therefore, model evaluation focuses on precision, recall, F1-score, and the confusion matrix, rather than accuracy alone.

## Preliminary Results

The current XGBoost baseline produced the following failure-class results:

| Metric | Validation | Test |
|---|---:|---:|
| Precision | 0.82 | 0.88 |
| Recall | 0.63 | 0.59 |
| F1-score | 0.71 | 0.71 |

These are preliminary results using the current model configuration and default classification threshold. Further experimentation and optimisation are ongoing.

## Project Status

**Current stage:** Data preprocessing, model training, and baseline evaluation.

Planned improvements include:

- Hyperparameter optimisation.
- Further investigation of class imbalance.
- Feature engineering and feature importance analysis.
- Classification threshold optimisation.
- Model evaluation and comparison.
- Development of a predictive maintenance application.
- Future integration with sensors and embedded hardware for real-time machine monitoring.

## Future Vision

The long-term goal is to develop a practical predictive maintenance system that can receive machine operating data from sensors, process the data using a trained machine learning model, and provide early warnings when operating conditions suggest an increased risk of failure.

This will involve connecting machine learning with embedded systems and hardware technologies.

## Author

**Hammed Taiwo Nurudeen**

Mechatronics Engineering Student  
Interested in Machine Learning, Robotics, and Embedded Systems.
