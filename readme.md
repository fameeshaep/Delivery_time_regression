**Overview**
This project predicts delivery time based on factors like vehicle type, weather, traffic level, distance, preparation time and distance.It is a regression problem aimed at improving delivery efficiency

**Dataset**
- Source: Kaggle
- Rows: 1000
- Columns: 9

**Input Features**
- Vehicle type
- Weather
- Preparation time(minute)
- Distance(km)
- Time of day
- Traffic level

**Target**
- Delivery Time(minutes)

**Technologies Used**
- Python
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn

**Exploratory Data Analysis(EDA)**
- Histogram(distribution check)
- Boxplot(outlier detection)
- Scatterplot(relationship analysis)
- Heatmap(correlation analysis)

**Key Insights**

- Distance is highly correlated with delivery time
- outliers found in distance
- skewness= 0.5

**Data Preprocessing**
- Used RobustScaler to handle outliers
- Encoding: 
 - One-hot encoding: vehicle type, Weather, Time of day
 - ordinal encoding: Traffic level
- Train-Test Split:
 - 80% Training
 - 20% Testing

**Models Used & Performance**
**Linear Regression**
- Train MSE: 132.83
- Train R2: 0.73
- Test MSE: 100.67
- Test R2: 0.77

**Decision Tree Regressor**
- Train MSE: 0
- Train R2: 1
- Test MSE: 254
- Test R2: 0.43

**Random Forest Regressor**
- Train MSE: 22.45
- Train R2: 0.95
- Test MSE: 96.87
- Test R2: 0.78

**Results**
- RandomForest Regressor is the best model with highest Test MSE (96.87) and lowest Test R2 Score(0.78)
- RandomForest Regressor captures non-linear relationships
- RandomForest Regressor is more robust than DecisionTree(which overfits)

**Key Takeaways**
- Distance is the most important feature
- Tree-based model performs better for this dataset
- RobustScaler helps handle outliers effectively

**Future Improvements**
Perform hyperparameter tuning









