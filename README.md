# Chemical-Process-Data-Science-Project
## Breast Tissue Mass Prediction using Image Features

### Project Overview

The goal of this project is to predict whether a breast tissue sample is **malignant** or **benign** based on features extracted from digitized images of breast mass tissue samples. We use a dataset that provides various characteristics of the cell nuclei from these tissue samples, and through simple statistical analysis, we aim to predict the malignancy status for each sample.

Additionally, we will explore which features are most important in determining whether a mass is malignant or benign, based on their relationship to the diagnosis.

### Dataset Summary

The dataset includes digitized images of fine needle aspirate (FNA) samples from breast mass tissue. Each sample is characterized by measurements describing the cell nuclei, and includes the following information:

* **ID Number**: A unique identifier for each sample.
* **Diagnosis**: A classification label indicating whether the mass is **malignant** or **benign**.

### Features

The dataset contains 10 features that describe the properties of the cell nuclei:

1. **Radius**: The average distance from the center to points on the perimeter of the mass.
2. **Texture**: A measure of the texture or roughness of the mass.
3. **Perimeter**: The total length of the boundary of the mass.
4. **Area**: The total number of pixels inside the boundary of the mass.
5. **Smoothness**: A measure of how smooth or irregular the boundary is.
6. **Compactness**: A measure of the compactness of the mass (calculated as perimeter squared divided by area).
7. **Concavity**: The degree of concave regions (indentations) along the boundary of the mass.
8. **Concave Points**: The number of concave portions of the mass boundary.
9. **Symmetry**: A measure of the symmetry or asymmetry of the mass.
10. **Fractal Dimension**: A measure of the complexity of the boundary of the mass.

For each of these features, three values are provided:

* **Mean**: The average value for each feature across the sample.
* **SE (Standard Error)**: The standard error of the feature's mean.
* **Largest**: The largest observed value of the feature in the sample.

### Key Objectives

1. **Prediction of Malignancy**: Using the provided features, predict whether each tissue sample is malignant or benign.

2. **Feature Importance Ranking**: Analyze which of the 10 features (and their mean, SE, or largest values) are most important in predicting the diagnosis. This will help identify which characteristics of the tissue are most indicative of malignancy.

### Methodology

1. **Data Preprocessing**:

   * Clean the dataset, handle any missing values, and standardize the data if necessary.
   * Conduct exploratory data analysis (EDA) to visualize the distributions of features and their relationship with the diagnosis.

2. **Prediction Process**:

   * Using basic statistical analysis or threshold-based rules, predict whether each mass is malignant or benign based on the available features.
   * This prediction will rely on simple comparisons of the feature values (e.g., a threshold value for radius or perimeter) or correlation between features and diagnosis.

3. **Feature Importance**:

   * Perform a ranking or statistical analysis of the features to determine which ones have the highest correlation or impact on the malignancy prediction.

4. **Results Interpretation**:

   * Analyze the prediction results to determine the accuracy of the predictions and interpret which features played the largest role in determining malignancy.

### Conclusion

The primary goal of this project is to predict the malignancy of breast tissue samples using features derived from digital images, without the use of machine learning models. The project also explores the importance of various features in determining the diagnosis of malignant versus benign tissue, providing insight into the characteristics most indicative of malignancy.

---

### Technologies and Libraries Used

* **Python** for data manipulation and analysis
* **Pandas**, **NumPy** for handling the data and performing calculations
* **Matplotlib**, **Seaborn** for visualizing data and relationships between features
* **Scikit-learn** for basic statistical analysis (if applicable for feature importance ranking)

---

### Dataset Reference

https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data/data​
