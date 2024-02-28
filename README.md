# Car Price Prediction by Using K-nearest-neighborhood (KNN) Regression Model
- **Objective**: Explore the best numeric feature subset and K-value for car price prediction.

`Dataset` is from 1985 Ward's Automotive Yearbook <br>
`Available from`: https://archive.ics.uci.edu/dataset/10/automobile

## Here I implemented:
1. Data Cleansing and Data Transformation
2. Univariate KNN model with single K-value
3. Univariate KNN model with multiple K-values (Hyperparameter Tuning)
4. Multivariate KNN model with single K-Value
5. Multivariate KNN model with multiple K-Values (Hyperparameter Tuning & K-Fold Cross-Validation)
   
## Conclusion
- Best Feature Subset: ['city-mpg', 'wheel-base', 'curb-weight', 'highway-mpg', 'peak-rpm'] <br> Best k Value: 1 <br>Best Average Accurcy: 86.43%

## Future Step
- With the multivariate KNN hyperparameter tuning, we used `f_regression` scoring function for best feature subset selection. <br>
However, `f_regression` only examines the linear relationship between features and target, and return `p-value`. <br>
- We can further apply `Mutual Information` function from `Scikit-learn` for feature selection, to see if non-linear results can make the prediction better.
- We only used numerical features for prediction. It is interesting to explore how combinations of categorical and numeric features ​​can achieve better accuracy by implementing `One-Hot Encoding`.
