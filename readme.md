\#Delivery Time Prediction



\##Overview

This project predicts \*\*delivery time\*\* based on factors like vehicle type, weather, traffic level, distance, preparation time and distance

It is a \*\*regression problem\*\* aimed at improving delivery efficiency



\##Dataset

\-Source: Kaggle 

\-Rows: 1000

\-Columns: 9



\###Input Features:

\-Vehicle type

\-Weather

\-Preparation time(minute)

\-Distance(km)

\-Time of day

\-Traffic level



\###Target:

\-Delivery Time(minutes)



\###Technologies Used

\-Python

\-Scikit-learn

\-Pandas

\-Matplotlib

\-Seaborn



\##Exploratory Data Analysis(EDA)

\-Histogram(distribution check)

\-Boxplot(outlier detection)

\-Scatterplot(relationship analysis)

\-Heatmap(correlation analysis)



\###Key Insights:

\-\*\*Distance\*\* is highly correlated with delivery time

\-outliers found in distance

\-skewness= 0.5



\##Data Preprocessing

\-Used \*\*RobustScaler\*\* to handle outliers

\-Encoding: 

&#x20;-One-hot encoding: vehicle type, Weather, Time of day

&#x20;-ordinal encoding: Traffic level

\-Train-Test Split:

&#x20;-80% Training

&#x20;-20% Testing



\##Models Used \& Performance



\### Linear Regression

\-Train MSE: 

\-Train R2:

\-Test MSE:

\-Test R2:



\### Decision Tree Regressor

\-Train MSE:

\-Train R2:

\-Test MSE:

\-Test R2:



\### Random Forest Regressor

\-Train MSE:

\-Train R2:

\-Test MSE:

\-Test R2:



\## Best Model: Random Forest Regressor

\### Why it is best:

\-Highest \*\*Test R2 Score()\*\*

\-Lowest \*\*Test MSE ()\*\*

\-Captures \*\*non- linear relationships\*\*

\-More \*\*robust\*\* than Decision Tree(which overfits)



\##Key Takeaways

\-Distance is the most important feature

\-Tree-based model performs better for this dataset

\-RobustScaler helps handle outliers effectively



\##Future Improvements

\-Perform hyperparameter tuning









