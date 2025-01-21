# Classification
Logistic Regression: A simple model for binary and multi-class classification based on logistic regression.

K-Nearest Neighbors (KNN): A non-parametric method where classification is based on the majority vote of neighbors.

Support Vector Machine (SVM): A powerful classification algorithm that finds the optimal hyperplane to separate classes.

Decision Tree: A model that splits the data based on feature values to make decisions.

Random Forest: An ensemble method that creates multiple decision trees and combines their results for improved accuracy.

Naive Bayes: A probabilistic classifier based on Bayes' theorem, typically effective with text data or independent features.

Gradient Boosting: An ensemble technique that builds strong models by iteratively correcting the mistakes of weak learners.
# Regression
# Feature Engineering:

Scaling: We applied StandardScaler to scale the features, which is essential for algorithms like Support Vector Regressor (SVR) and K-Nearest Neighbors (KNN).
Polynomial Features: We added polynomial features (degree 2) using PolynomialFeatures to capture more complex relationships between features.
Hyperparameter Tuning:

We used GridSearchCV to tune hyperparameters for Random Forest and XGBoost models. You can easily expand this for other models if needed.
Cross-Validation:

We used 5-fold cross-validation with cross_val_score to calculate the mean squared error (MSE) for each model, which helps to understand how well the model generalizes.
Evaluation:

For each model, we computed the Mean Squared Error (MSE) and R-squared (R²) to assess performance.
The results are stored in a DataFrame (results_df) for easy comparison.
Visualization:

We created a bar chart comparing the R-squared (R²) values across models, which helps to identify the best-performing models visually.
