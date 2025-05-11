# RiskProfile-Unsupervised-Learning-for-Obesity-Pattern-Detection

RiskProfile is a data science project that applies unsupervised learning techniques to identify and classify obesity patterns based on lifestyle, physical, and behavioral factors. The project successfully implements Principal Component Analysis (PCA) for dimensionality reduction and K-means clustering to categorize individuals into distinct obesity categories: Healthy Weight, At Risk (Overweight), Obese, and Severely Obese.
Key Features

Data Preprocessing: Comprehensive feature engineering including binary encoding, ordinal encoding, and one-hot encoding for categorical variables
Standardization: Appropriate scaling of numeric features to ensure equal contribution to clustering
Dimensionality Reduction: PCA implementation to reduce feature space while preserving variance
Cluster Analysis: K-means clustering with optimal cluster selection using the Elbow Method
Obesity Classification: Categorization of clusters into clinically relevant categories (Healthy Weight, At Risk/Overweight, Obese, Severely Obese)
Visualization: 2D representation of obesity categories in principal component space

Dataset
The dataset includes a variety of features related to obesity risk factors:

Demographic Information: Gender, Age
Physical Measurements: Height, Weight
Health History: Family history with overweight
Dietary Habits: High-calorie food consumption, vegetable consumption, meal frequency, snacking habits
Lifestyle Factors: Physical activity level, technology usage time, smoking status
Consumption Patterns: Water intake, alcohol consumption
Transportation: Primary mode of transportation

Methodology
Data Preprocessing

Binary encoding for yes/no variables
Ordinal encoding for ranked categorical variables
One-hot encoding for nominal categorical variables
Standardization of numeric features with different scales

Feature Reduction
Principal Component Analysis (PCA) was applied to reduce the dimensionality of the dataset while preserving the maximum variance, allowing for more efficient clustering and better visualization.
Clustering
K-means clustering was performed on the reduced feature set. The optimal number of clusters (k=4) was determined using the Elbow Method, which analyzes the relationship between the number of clusters and the within-cluster sum of squares (inertia).
Obesity Categorization
Clusters were analyzed based on their centroid characteristics to classify them into clinically relevant obesity categories:

Healthy Weight
At Risk (Overweight)
Obese
Severely Obese

Results
The analysis successfully identified four distinct clusters corresponding to different obesity categories. Each cluster represents a unique combination of physical attributes, lifestyle choices, and behavioral patterns that contribute to weight status. The visualization clearly shows separation between the four categories in the PCA space, validating our clustering approach.
Technologies Used

Python 3.8+
Pandas for data manipulation
Scikit-learn for PCA and K-means implementation
Matplotlib and Seaborn for visualization
