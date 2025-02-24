Presentation link: https://prezi.com/p/ry74hpf3jdlz/speed-dataing-analyzing-predictive-models/#ai-flow/details

1. Importing & Setup:

Sets up the environment by importing libraries, downloading the dataset, and loading the data.
2. Cleaning:

Prepares the raw data by cleaning up string columns, converting columns to numeric types, handling missing values, and dropping columns.
3. Divide into Target and Variables:

Separates the dataset into the target variable ("match") and features, applies one-hot encoding.
4. Train/Test Split:

Divides the dataset into training and testing sets to evaluate the models.
5. Normalized by MinMaxScaler:

Scales the numerical features using MinMaxScaler for algorithms that benefit from feature scaling.
6. KNN Classifier Test:

Trains and evaluates a basic K-Nearest Neighbors model using the scaled data.
7. Create a Correlation Heatmap:

Visualizes correlations between all features using a heatmap to understand data relationships.
8. Discard Strongly Correlated Columns:

Removes highly correlated features to reduce redundancy and potential multicollinearity.
9. Sort variables by their absolute

Sorts variables by their absolute correlation to the target, removing the least correlated ones.
10. Create Reduced Training and Testing

Splits data again using the reduced feature set from the previous feature selection steps.
11. Normalize Reduced Data:

Scales the reduced feature set using MinMaxScaler.
12. Fit KNNClassifier to Reduced Data:

Trains and evaluates a K-Nearest Neighbors model using the reduced and scaled feature set.
13. Create a Correlation Heatmap of

Visualizes the correlation in the reduced feature set.
14. Logistic Regression on Reduced Data:

Trains and evaluates a Logistic Regression model using the reduced feature set.
15. Decision Tree Classifier on Reduced

Trains and evaluates a Decision Tree model with limited depth, also visualizes the tree.
16. Ensemble Methods:

Implements and evaluates several ensemble methods: Bagging, Pasting, Random Forest, AdaBoost, and Gradient Boosting.
17. Summary Stats:

Compiles the performance metrics of all models into a table for comparison.
18. Nice Chart: - Creates a barplot showing the performance of all the models.

19. Hyperparameter Tuning:

Uses GridSearchCV to tune the Gradient Boosting model, and evaluates it, visualizes the performance of the last two models.
