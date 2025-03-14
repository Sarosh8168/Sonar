Sonar Object Classification

Overview

This project uses machine learning to classify objects detected by sonar as either "Rock" or "Mine" based on sonar signal data. The classification model is built using Logistic Regression.

Dataset

The dataset consists of 61 columns:

The first 60 columns represent numerical sonar signal readings.

The 61st column (label) indicates whether the object is a "Rock (R)" or a "Mine (M)".

Dependencies

To run this project, you need to install the following Python libraries:

pip install numpy pandas scikit-learn

Project Workflow

Load the Dataset: The data is loaded from a CSV file into a Pandas DataFrame.

Exploratory Data Analysis:

Display dataset shape and statistical summary.

Count occurrences of each label (Rock/Mine).

Compute mean values grouped by label.

Data Preprocessing:

Separate features (X) and labels (y).

Split the dataset into training and test sets (90% training, 10% test).

Model Training:

A Logistic Regression model is trained on the training data.

Model Evaluation:

Accuracy is measured for both training and test datasets.

Prediction System:

A sample sonar reading is provided as input.

The trained model predicts whether the object is a "Rock" or "Mine".

Running the Project in Google Colab

Steps to Run in Google Colab

Open Google Colab: Go to Google Colab

Upload Your Dataset:

Click on the folder icon on the left panel.

Click Upload and select your sonar data.csv file.

Upload Your Notebook (.ipynb file):

Click File → Upload Notebook.

Select your .ipynb file and upload it.

Run the Notebook:

Click Runtime → Run All to execute the script.

Ensure the dataset path in the script matches /content/sonar data.csv.

Example Prediction

Sample input data:

input_data = (0.0453, 0.0523, 0.0843, 0.0689, 0.1183, ...)

Output:

The object is a mine

Accuracy

Training Data Accuracy: Displayed after training.

Test Data Accuracy: Displayed after testing.

Future Improvements

Try different classification models (e.g., SVM, Random Forest).

Perform feature scaling and hyperparameter tuning.

Use deep learning models for better accuracy.

Author

This project is developed using Python and Scikit-learn.
