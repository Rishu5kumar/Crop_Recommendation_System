# Crop Recommendation System

This project is a Crop Recommendation System using machine learning. The code leverages various classifiers to find the best model for crop prediction and provides recommendations based on the provided input values.

## Dataset

The dataset used in this project is loaded from `Crop_recommendation.csv`. It contains information on various crops along with environmental parameters such as nitrogen, phosphorous, potassium levels, temperature, humidity, pH, and rainfall.

## Requirements

- Python 3.x
- Libraries:
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - scikit-learn

To install the required libraries, run:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and check for missing or duplicate values.
   - Visualize data relationships using heatmaps and distribution plots.
  
2. **Encoding Crop Labels**:
   - Convert crop names to numerical labels for easier processing.
   
3. **Feature Selection**:
   - Define features (N, P, K, temperature, humidity, pH, rainfall) and labels.

4. **Train-Test Split**:
   - Split the data into training and testing sets with an 80:20 ratio.
   
5. **Standardization**:
   - Standardize feature values using `StandardScaler`.

6. **Model Training and Evaluation**:
   - Train multiple classification models: Logistic Regression, Naive Bayes, SVM, K-Nearest Neighbors, Decision Tree, Random Forest, Bagging, AdaBoost, Gradient Boosting, and Extra Trees.
   - Evaluate each model's accuracy on the test data.

7. **Crop Recommendation Function**:
   - Define the `recommendation` function, which takes input parameters (N, P, K, temperature, humidity, pH, rainfall) and outputs the recommended crop.

## Code Example

### Sample Input
```python
N = 40
P = 50
K = 50
temperature = 40.0
humidity = 20
pH = 100
rainfall = 100
```

### Running the Recommendation
```python
predict = recommendation(N, P, K, temperature, humidity, pH, rainfall)
```

## Output
The recommendation function will output the crop best suited for the given environmental conditions. For example:
```
"Mothbeans is the best crop to be cultivated"
```

## Usage

To use this system:
1. Load the dataset in CSV format.
2. Run the script, adjusting environmental parameters in the `recommendation` function as needed.
3. Check the output for the recommended crop.

---
