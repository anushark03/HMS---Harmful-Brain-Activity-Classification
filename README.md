This repository contains the implementation of a machine learning and deep learning pipeline for the detection and classification of harmful brain activity patterns using EEG data. This work is part of a Kaggle competition aimed at improving electroencephalography (EEG) pattern classification accuracy to aid in neurocritical care, epilepsy treatment, and drug development.

### Competition Objective
The goal is to develop models capable of classifying six key EEG patterns:

Seizure (SZ)
Generalized Periodic Discharges (GPD)
Lateralized Periodic Discharges (LPD)
Lateralized Rhythmic Delta Activity (LRDA)
Generalized Rhythmic Delta Activity (GRDA)
Other
Accurate classification of these patterns will help automate EEG analysis, reducing manual workloads for neurologists and improving patient outcomes.

### Methodology
Data Preprocessing
Data cleaning and feature extraction from EEG recordings.
Scaled numerical features for consistency across input variables.
Expert-consensus labels used as target variables for supervised learning models.
Traditional Machine Learning
Models Used:
Random Forest Classifier: Achieved ~88% accuracy on the test dataset.
Decision Tree Classifier: Achieved ~87.7% accuracy on the test dataset.
K-Nearest Neighbors: Performance analyzed with confusion matrices.
Emphasis on model interpretability and reliability.
Transition to Deep Learning
Neural Network Models:
DenseNet backbone for feature extraction from spectrograms.
Custom-built data augmentation and preprocessing pipelines.
Achieved high accuracy with structured probabilistic outputs.
Utilized spectrograms as inputs for enhanced feature representation. 

###Key Features

Random Forest Classifier:

Highly generalizable and robust model for initial insights.
Probabilistic predictions for EEG classifications.
Deep Learning Pipeline:

Augmented data strategy with MixUp and Random Cutout techniques.
DenseNet-based architecture fine-tuned for EEG spectrogram data.
Custom Preprocessing:

Automated feature extraction from .parquet files into .npy format for neural network compatibility.
Built-in caching and batching for efficient data handling.
