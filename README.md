# breast-cancer-diagnosis

1. Logistic Regression:

What it is: A statistical model employed to predict the likelihood of a binary outcome (here, malignant or benign tumor).
How it works: It maps the linear combination of input features to a probability between 0 and 1 using a sigmoid function.

2. Data Preprocessing

Standardization: This is essential for Logistic Regression. It means converting the features to have unit variance and zero mean.
Why it's important: It stops features with bigger scales from overpowering the model and assists the optimization process in converging faster.
How it's done: Utilizing StandardScaler in scikit-learn.
3. Model Training and Evaluation:

Training: The Logistic Regression model is trained on the labeled training data (features and their corresponding diagnosis). The model learns the best coefficients (β values) to reduce the discrepancy between predicted and actual results.
Evaluation Metrics:
Confusion Matrix: A table indicating the number of true positives, true negatives, false positives, and false negatives.
Accuracy: The ratio of correctly classified samples.
Precision: The ratio of true positive predictions out of all positive predictions.
Recall (Sensitivity): The ratio of true positive predictions to all actual positive samples.
F1-score: The harmonic mean between precision and recall, offering a balance between the two.
ROC AUC Score: Receiver Operating Characteristic Curve Area Under the Curve, quantifying the model's capacity for class separation.
Threshold Optimization: Determining the best probability threshold for sample classification as malignant or benign, usually through maximizing the F1-score.
4. ROC Curve and Decision Boundary

ROC Curve: Graphical representation of the performance of the model across different classification thresholds. It depicts the true positive rate (sensitivity) as a function of the false positive rate (1-specificity).
Decision Boundary: The dividing line or hyperplane between the classes in feature space. It's defined by the coefficients of the model and the selected threshold.
