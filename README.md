# Housing_Horizon
This project involves housing classification using the "ParisHousingClass.csv" dataset. It starts with data exploration and preprocessing to handle missing values. A Decision Tree classifier with a max depth of 4 and entropy criterion is trained. The model is evaluated using a 70-30 train-test split, focusing on classification accuracy.
Here’s a structured explanation and key topics that you can include in your **README** file for GitHub based on the project files:

---

# Paris Housing Classification Project

## Overview
This project focuses on classifying housing data using the "ParisHousingClass.csv" dataset. The objective is to predict the category of houses based on various features. The project utilizes Python’s data manipulation and machine learning libraries to perform exploratory data analysis, preprocessing, and model training using a Decision Tree classifier.

## Project Structure
- **data/**: Contains the dataset used in this project (`ParisHousingClass.csv`).
- **notebooks/**: Jupyter notebooks used for data exploration, preprocessing, and model development.
- **models/**: Directory for storing trained models (optional).
- **README.md**: Project description and documentation.

## Key Features
- Data loading and exploratory data analysis (EDA) to understand dataset structure.
- Preprocessing techniques such as handling missing values and feature engineering.
- Decision Tree classifier used to predict housing categories.
- Model training with a 70-30 train-test split to evaluate model performance.

## Installation
To run the project, ensure you have the following libraries installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Dataset
The dataset (`ParisHousingClass.csv`) contains features such as area, number of rooms, and more, used to classify housing categories. Ensure the dataset is placed in the `data/` directory.

## Usage
1. Clone the repository.
2. Install the required libraries.
3. Run the notebook to explore and preprocess the dataset.
4. Train the model and evaluate it on test data.

### Example Commands:
```python
import pandas as pd
df = pd.read_csv('data/ParisHousingClass.csv')
# Exploratory Data Analysis
df.info()
df.isnull().sum()
# Model Training
clf = DecisionTreeClassifier(max_depth=4, criterion='entropy')
clf.fit(X_train, y_train)
```

## Model
- **Classifier**: Decision Tree
- **Hyperparameters**: max_depth=4, criterion='entropy'
- **Train-Test Split**: 70% training, 30% testing

## Results
The model performance can be measured using accuracy and other metrics (e.g., confusion matrix, precision, recall).

## Future Work
- Experiment with different classification algorithms (e.g., Random Forest, SVM).
- Optimize hyperparameters to improve model performance.
- Add cross-validation and feature importance analysis.

## Contributing
Feel free to submit issues or pull requests to improve the project.

---
