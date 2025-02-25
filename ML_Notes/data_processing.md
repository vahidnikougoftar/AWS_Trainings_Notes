# Some techniques for handling Missing Data  
1. Filling in with Mean (or Median if significant outliers)
   (note that sometimes there could be strong correlation between other columns and the column with missing values, so filling with mean may not work properly)
2. Dropping (almost always the last resort)
3. Deep Learning / Regression (to predict the categorical/numerical values for the missing column)
4. MICE (Multivariate Imputation by Chained-Equations)

# Inbalanced Datasets: best approach is SMOTE (Synthetic Minority Over-sampling TEchnique):
- Artificially generate fake data for undersampled class (eg. use K-Means to find nearest neighbors and averag them to generate data points)

# handling outliers 
- find mean +/- 2sigma?
- also can use AWS Random Cut Forest Outlier Detection
