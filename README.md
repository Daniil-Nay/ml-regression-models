# Notebooks
### 1-r-real_estate_saint_petersburg
[ENG] The objective of this notebook was to develop a model to estimate real estate prices in Saint Petersburg.
The dataset contained various property features, and preprocessing steps included imputation of missing values and scaling of features.  
Several models were trained and evaluated:
1. Linear Regression
2. RandomForestRegressor
3. XGBRegressor
4. ExtraTreesRegressor
5. LGBMRegressor
6. CatBoostRegressor
7. Lasso Regression
8. Stacking Regressor model 1 (It includes such models as: 1, 2 3 and 6)
9. Stacking Regressor model 2 (It includes such models as: 1 and 2)

| Model               | r^2 score - Validation |  r^2 score - Test  |
|---------------------|------------------------|--------------------|
| Linear Regression   | 0.7010                 | 0.7029             |
| RandomForest        | 0.8534                 | 0.8543             |
| XGBRegressor        | 0.8617                 | 0.8619             |
| ExtraTrees          | 0.8363                 | 0.8393             |
| LGBM                | 0.8633                 | 0.8642             |
| CatBoost            | 0.8644                 | 0.8655             |
| Lasso Regression    | 0.6988                 | 0.6989             |
| Stacking_1          | 0.8530                 | 0.8516             |
| Stacking_2          | 0.8245                 | 0.8231             |


Among the models evaluated, CatBoost and LGBM emerged as the top performers,  
delivering the highest R² scores on both validation and test sets.   
CatBoost slightly edged out LGBM, showcasing its superior performance in predicting real estate prices.   
XGBRegressor also demonstrated strong results, closely following the top two models.

To further enhance the predictive accuracy, additional hyperparameter tuning and feature engineering could be beneficial.  
Experimenting with different feature transformations, interactions, or incorporating domain-specific   
knowledge might lead to improved model performance.

