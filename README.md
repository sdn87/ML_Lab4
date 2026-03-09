# ML_Lab4: Data Quality Assessment & Preprocessing

Overview:
This lab focuses on assessing data quality and applying preprocessing techniques to prepare data for machine learning models.

Tasks Completed:
 Task 1: Data Quality Assessment 
- Checked for missing values
- Identified and removed duplicates (3,854 rows)
- Verified data types
- Analyzed statistical ranges

Task 2: Missing Value Handling 
- Strategy applied: **Median Imputation**
- Reason: Robust against outliers in BMI and glucose levels
- Introduced artificial missing values for demonstration
- Successfully imputed all missing values

Task 3: Outlier Detection & Handling 
- Method: **IQR (Interquartile Range)**
- Analyzed outliers in: age, BMI, HbA1c_level, blood_glucose_level
- Removed outliers beyond 1.5 × IQR threshold
- Visualized data before and after outlier removal

 Task 4: Feature Normalization 
Applied two normalization techniques:

 Min-Max Normalization
- Scaled features to [0, 1] range
- Best for: Neural networks, bounded algorithms

Z-Score Normalization (Standardization)
- Scaled features to mean=0, std=1
- Best for: PCA, distance-based algorithms

 Task 5: Dimensionality Reduction (PCA) 
- Checked correlation matrix first
- Correlation detected between features
- Applied PCA on standardized features
- Reduced dimensions while preserving 95% variance
- Visualized principal components
