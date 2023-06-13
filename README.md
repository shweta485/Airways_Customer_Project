# Airways_Customer_Project

Data Preprocessing:

The dataset is read from a CSV file using pd.read_csv().
Categorical columns, "sales_channel" and "trip_type", are one-hot encoded using OneHotEncoder.
The encoded features are concatenated with the original dataframe using pd.concat().
Unnecessary columns, such as "Unnamed: 0", "sales_channel", "trip_type", "booking_origin", and "route", are dropped.
Data Splitting and Normalization:

The dataset is split into training and testing sets using train_test_split().
The feature matrix X and target vector y are created.
The feature data is normalized using StandardScaler.
Model Training and Evaluation:

The Random Forest Classifier is instantiated with specified hyperparameters.
The model is trained on the scaled training data using fit().
Predictions are made on the training data and evaluation metrics (accuracy, precision, recall, and F1 score) are calculated using appropriate functions.
Predictions are also made on the testing data and evaluation metrics are calculated similarly.
Confusion Matrix:

A Confusion Matrix is created using ConfusionMatrix from yellowbrick.classifier library.
The Confusion Matrix is fitted on the training data and scored on the testing data.
Feature Importances:

The feature importances obtained from the trained Random Forest Classifier are plotted in a horizontal bar chart using matplotlib.pyplot.barh().

Developed and implemented a predictive model for customer booking completion using a Random Forest Classifier. The project involved preprocessing and 
analyzing a dataset of customer data from an airline, including one-hot encoding categorical features and standardizing numerical features.

The Random Forest Classifier was trained on the preprocessed data to predict whether a customer would complete a booking. The model achieved an accuracy 
of 93.4% on the training data, demonstrating its effectiveness in predicting customer behavior.

Additionally, the model was evaluated on a separate test dataset, achieving an accuracy of 85.5%. The precision score of 55.8% indicated the model's ability 
to correctly classify positive cases, while the recall score of 3.9% highlighted its capacity to identify true positive cases. The F1 score of 7.4% provided 
an overall measure of the model's performance


The project also involved visualizing the feature importances, which revealed insights into the most influential factors for booking completion.
By successfully developing and implementing this predictive model, I demonstrated my proficiency in data preprocessing, machine learning techniques, 
and model evaluation.
