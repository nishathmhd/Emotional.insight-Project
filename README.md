# Emotion Recognition from EEG Signals

## Overview

This repository contains code for analyzing and predicting emotions from EEG (Electroencephalogram) signals. The project involves data exploration, cleaning, statistical analysis, and visualizations to gain insights into the dataset. Additionally, it demonstrates the preparation of the data for machine learning, including handling outliers, exploring feature distributions, and splitting the data for training and testing. A brief statistical analysis is also performed on one of the numeric features.

## Dataset

The dataset used in this project is stored in the 'emotions.csv' file. It consists of multiple features extracted from EEG signals, such as mean values, spectral features, and more. The target variable is the 'label' column, representing the emotional state associated with each EEG recording (NEGATIVE, NEUTRAL, POSITIVE).

## Load and Explore the Data

The first step involves loading the dataset using the Pandas library and exploring its structure. The dataset contains 2132 rows and 2549 columns, with most columns being numeric features. The 'label' column is the target variable, and there are no missing values in the dataset.

## Data Cleaning

The code checks for and handles outliers in one of the features ('mean_2_a') using z-scores. This step ensures that extreme values do not adversely affect the analysis and modeling process.

## Exploratory Data Analysis (EDA)

The EDA section provides insights into the distribution of emotion labels, correlation analysis, and visualizations. Key visualizations include a countplot of emotion labels, a heatmap illustrating the correlation between features, and distribution visualizations such as histograms and box plots.

## Data Splitting

The dataset is split into training and testing sets using the train_test_split function from Scikit-learn. The split is performed with 80% of the data used for training and 20% for testing.

## Statistical Analysis

Statistical analysis is performed on a specific numeric feature ('# mean_0_a'). The mean, median, and standard deviation are calculated for each emotion label, and a box plot is generated to visualize the distribution of this feature across different emotions.

## Correlation Analysis

The correlation matrix of all numeric features is calculated and visualized using a heatmap. This analysis helps identify potential relationships between different features.

## Conclusion

This project provides a comprehensive exploration and analysis of the emotion recognition dataset, setting the foundation for further machine learning modeling and predictive tasks.

Feel free to explore the code, contribute, or use it as a reference for your own projects.
