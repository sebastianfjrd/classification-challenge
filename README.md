# classification-challenge
Internet Service Provider (ISP)
Challenge Background
The objective of this challenge is to improve the email filtering system for an Internet Service Provider (ISP) by accurately detecting spam emails. To achieve this, two supervised machine learning models were developed and evaluated: a Logistic Regression model and a Random Forest model. The dataset provided contains various features extracted from emails, with a target variable indicating whether the email is spam (1) or not spam (0).

Methodology
The process involved several key steps:

Data Preparation: The dataset was imported and examined to ensure accuracy.
Data Splitting: The data was divided into training and testing sets to evaluate model performance.
Feature Scaling: StandardScaler was used to normalize the feature data, ensuring that all features contribute equally to the model training.
Model Training and Evaluation:
A Logistic Regression model was trained and its performance was evaluated.
A Random Forest model was trained and its performance was evaluated.
Comparison and Conclusion: The accuracy of both models was compared to determine the better performing model.
Detailed Findings
Data Preparation
The dataset was successfully imported from the provided source, containing 58 columns and 4601 rows.
The target variable, spam, was separated from the feature set, resulting in X (features) and y (target).
Data Splitting
The data was split into training (75%) and testing (25%) sets using train_test_split.
The training set had 3450 samples, and the testing set had 1151 samples.
Feature Scaling
Feature scaling was applied using StandardScaler to ensure all features had a mean of 0 and a standard deviation of 1.
Logistic Regression Model
The Logistic Regression model was trained using the scaled training data.
Model predictions on the testing data resulted in an accuracy score of 92.88%.
Random Forest Model
The Random Forest model was trained using the scaled training data with 500 estimators.
Model predictions on the testing data resulted in an accuracy score of 96.52%.
Prediction and Results
Initial Prediction: Before training the models, it was predicted that the Random Forest model would perform better due to its complexity and ability to capture non-linear relationships in the data.

Results:

Logistic Regression Accuracy: 92.88%
Random Forest Accuracy: 96.52%
Conclusion:
The Random Forest model outperformed the Logistic Regression model, as initially predicted. The superior performance of the Random Forest model is attributed to its ensemble nature and capability to handle complex interactions among features, making it more effective at detecting spam emails.

Recommendations
Given the higher accuracy of the Random Forest model, it is recommended to implement this model in the ISP's email filtering system to enhance spam detection and improve customer satisfaction by minimizing the number of spam emails reaching their inboxes. Further improvements can be explored by fine-tuning model parameters and incorporating additional features to boost model performance even more.
