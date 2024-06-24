# Asthma Diagnosis: Comparative Analysis of Machine Learning Models

## 🎯 Goal

The aim of this project is to compare various machine learning models for predicting asthma diagnoses using a dataset from Kaggle.

## 🧵 Dataset

The original dataset can be found at the following link:

[Asthma Disease Dataset on Kaggle](https://www.kaggle.com/datasets/rabieelkharoua/asthma-disease-dataset/data)

For the filtered dataset used in this notebook, refer to: `asthma_disease_data.csv`

### Citation

@misc{rabie_el_kharoua_2024,  
  title={🌬️ Asthma Disease Dataset 🌬️},  
  url={https://www.kaggle.com/dsv/8669080},  
  DOI={10.34740/KAGGLE/DSV/8669080},  
  publisher={Kaggle},  
  author={Rabie El Kharoua},  
  year={2024}  
}

## 🧮 What I Had Done!

### Data Cleaning and Preprocessing

Here's the revised part of the README:

1. **Load the dataset:** Imported the data into a pandas DataFrame for manipulation and analysis.
2. **Remove unnecessary columns:** Removed 'PatientID' and 'DoctorInCharge' as they were redundant.
3. **Handle missing values:** Explored if any missing value.
4. **Ensure appropriate data formats:** Verified that all columns have the correct data types (e.g., integers, floats, strings).

### Exploratory Data Analysis (EDA)

1. **Summarize the dataset with descriptive statistics:** Provided an overview of the data distribution using mean, median, and standard deviation.
2. **Plot distributions:** Used histograms and boxplots to visualize the distribution of numerical variables and identify outliers.
3. **Analyze relationships:** Created a correlation matrix to examine relationships between variables and used scatter and bar plots to explore these relationships further.

Here is the revised section in markdown format:

## Feature Selection and Engineering

1. **Convert to categorical data types:** Converted 'AgeGroup' and 'BMICategory' columns to categorical data types.
2. **Label encoding:** Applied label encoding to categorical variables.
3. **Feature selection:** Selected top features using SelectKBest with Chi-Square.
4. **Class balancing:** Balanced the target class using ADASYN.
5. 
### Model Selection and Training

1. **Split data into training and testing sets:** Divided the dataset into training (e.g., 80%) and testing (e.g., 20%) subsets to evaluate model performance.
2. **Choose classification algorithms:** Selected models like SVM, Decision Tree, Random Forest, XGBoost, KNN, and neural networks for their effectiveness in handling classification tasks.

### Model Evaluation

1. **Evaluate performance using metrics:** Assessed models using Accuracy, Precision, Recall, F1-Score to understand their accuracy.
2. **Compare model performance:** Analyzed and compared the evaluation metrics to select the best-performing model.

## 🚀 Models Implemented

1. Support Vector Machine (SVM)
2. Decision Tree
3. Random Forest
4. XGBoost
5. K-Nearest Neighbors (KNN)
6. PyTorch Neural Network
7. Numpy-based Neural Network

## 📚 Libraries Needed

```plaintext
pandas==2.0.3
numpy==1.24.3
matplotlib==3.7.1
seaborn==0.12.2
scikit-learn==1.2.2
xgboost==1.7.5
imbalanced-learn==0.10.1
tqdm==4.65.0
torch==2.0.1
```

Install the required packages using the following command:

```bash
pip install -r requirements.txt
```

## 📈 Performance of the Models Based on Accuracy Scores

### Support Vector Machine (SVM)
Accuracy: 64.71%

### Decision Tree
Accuracy: 89.77%

### Random Forest
Accuracy: 95.20%

### XGBoost
Accuracy: 94.98%

### K-Nearest Neighbors (KNN)
Accuracy: 67.43%

### PyTorch Neural Network
Test Accuracy: 94.99%

### Numpy-based Neural Network
Accuracy: 95.20%

## 📢 Conclusion

- **Best Performing Model:** Random Forest and Numpy-based Neural Network with an accuracy of 95.20%.
- **Second Best:** PyTorch Neural Network with a test accuracy of 94.99%.
- **Models like SVM and KNN showed lower performance, indicating challenges in handling the minority class (1).**

### Recommendations

To enhance performance on the minority class, strategies such as adjusting class weights, using techniques like oversampling or synthetic data generation, and exploring more sophisticated neural network architectures could be beneficial. Additionally, fine-tuning hyperparameters and conducting more extensive feature engineering might further improve model outcomes.

---
✒️ Swayam Patil
---