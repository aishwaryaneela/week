Initially, the project aimed to predict EV costs/ratings using basic regression models with simple preprocessing. To improve the model's accuracy and robustness, I extended the project in several ways:

Enhanced Data Cleaning and Feature Engineering

Moved from simple mean imputation to median-based imputation for numerical features to reduce the effect of outliers.

Implemented label encoding for categorical variables to enable machine learning compatibility.

Applied standard scaling to numerical variables for normalization, helping improve model convergence and prediction stability.

Advanced Model Selection

Introduced the powerful XGBoost regression model, known for better performance on structured data problems.

Configured hyperparameters such as learning rate, number of estimators, and tree depth to optimize the training process.

Robust Model Evaluation Strategy

Used train-test splits ensuring model validation on unseen data.

Evaluated model performance with both Mean Squared Error (MSE) and R-squared (R²) metrics to comprehensively assess prediction quality.

Visualization and Interpretability

Added feature importance visualizations, allowing insights into which EV attributes impact cost predictions the most.

Created actual vs predicted value plots to visualize model accuracy graphically.

Model Persistence

Saved the trained model using joblib, enabling reuse without retraining and facilitating deployment scenarios.

These extensions collectively helped transform a basic regression task into a robust predictive modeling solution with better accuracy, explainability, and usability.

