# Sonar Object Classification

## Overview

This project uses machine learning to classify objects detected by sonar as either "Rock" or "Mine" based on sonar signal data. The classification model is built using Logistic Regression.

## Dataset

The dataset consists of 61 columns:

- The first 60 columns represent numerical sonar signal readings.
- The 61st column (label) indicates whether the object is a "Rock (R)" or a "Mine (M)".

## Dependencies

To run this project, install the required Python libraries:

```sh
pip install numpy pandas scikit-learn
```

## Project Workflow

### Load the Dataset
- Load data from a CSV file into a Pandas DataFrame.

### Exploratory Data Analysis
- Display dataset shape and statistical summary.
- Count occurrences of each label (Rock/Mine).
- Compute mean values grouped by label.

### Data Preprocessing
- Separate features (X) and labels (y).
- Split the dataset into training (90%) and test (10%) sets.

### Model Training
- Train a Logistic Regression model on the training data.

### Model Evaluation
- Measure accuracy for both training and test datasets.

### Prediction System
- Provide a sample sonar reading as input.
- The trained model predicts whether the object is a "Rock" or "Mine".

## Running the Project in Google Colab

### Steps to Run in Google Colab

1. **Open Google Colab:** Go to [Google Colab](https://colab.research.google.com/).
2. **Upload Your Dataset:**
   - Click on the folder icon on the left panel.
   - Click Upload and select your `sonar data.csv` file.
3. **Upload Your Notebook (.ipynb file):**
   - Click File → Upload Notebook.
   - Select your `.ipynb` file and upload it.
4. **Run the Notebook:**
   - Click Runtime → Run All to execute the script.
   - Ensure the dataset path in the script matches `/content/sonar data.csv`.

## Example Prediction

### Sample Input Data

```python
input_data = (0.0453, 0.0523, 0.0843, 0.0689, 0.1183, ...)
```

### Output

```
The object is a mine
```

## Accuracy

- **Training Data Accuracy:** Displayed after training.
- **Test Data Accuracy:** Displayed after testing.

## Future Improvements

- ✅ Try different classification models (SVM, Random Forest).
- ✅ Perform feature scaling and hyperparameter tuning.
- ✅ Use deep learning models for better accuracy.

## Author

This project is developed using Python and Scikit-learn. 🚀
