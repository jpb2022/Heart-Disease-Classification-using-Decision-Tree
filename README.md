# Heart Disease Classification using Decision Tree

## 📌 Project Overview
This project focuses on building a Decision Tree Classifier to predict the presence of heart disease in patients based on their health-related features. The performance of the model is enhanced through Cost Complexity Pruning and K-Fold Cross-Validation, resulting in a decision tree with strong predictive capabilities:

- ✅ Accuracy for patients without heart disease: 76.9%
- ❤️ Accuracy for patients with heart disease: 81.0%

## 🎯 Objective
Given a dataset of patient health records, the objective is to construct and evaluate a decision tree that classifies heart disease with an overall accuracy ≥ 70%.

## 🔍 Methodology & Approach
The project follows this structured approach:

1. **📦 Import Libraries & Load Dataset**
   - Load necessary Python libraries and the heart disease dataset

2. **📊 Exploratory Data Analysis (EDA)**
   - Understand feature distributions
   - Detect missing values
   - Visualize patterns and correlations

3. **🧹 Data Preprocessing**
   - Handle missing values
   - Encode categorical variables
   - Scale/normalize numerical features if required

4. **🌳 Initial Decision Tree Model**
   - Train a basic Decision Tree classifier
   - Evaluate its initial performance

5. **✂️ Cost Complexity Pruning (CCP)**
   - Prune the tree to prevent overfitting
   - Choose optimal ccp_alpha based on performance

6. **🔁 K-Fold Cross-Validation**
   - Validate model robustness using k-folds (k=5)

7. **📈 Improved Model Evaluation**
   - Assess final performance on unseen data
   - Compare with baseline

## 🧠 Results Summary
The improved decision tree demonstrates strong performance:
- No Heart Disease: 76.9% accuracy
- Heart Disease Present: 81.0% accuracy
- Overall Performance: Satisfies the 70% accuracy requirement

## 📚 Dataset
The dataset used is the Heart Disease Dataset from the UCI Machine Learning Repository. It contains attributes such as:
- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol levels
- And more

## ✍️ Author
**Er. Jitendra Kumar**  
AI Researcher  
🎓 M.Tech, IIT Kanpur  
🎓 B.Tech, NIT Surat

---

## Project Structure
The Jupyter notebook contains the following main sections:

1. **Data Loading and Initial Inspection**
   - Importing libraries
   - Loading dataset from UCI repository
   - Initial data exploration

2. **Exploratory Data Analysis**
   - Summary statistics
   - Data visualizations (scatter plots, histograms, box plots)
   - Correlation analysis

3. **Data Preprocessing**
   - Handling missing values
   - Feature engineering
   - One-hot encoding of categorical variables

4. **Model Building**
   - Initial decision tree implementation
   - Cost complexity pruning
   - K-fold cross-validation
   - Final model evaluation

5. **Results and Interpretation**
   - Confusion matrix analysis
   - Decision tree visualization
   - Performance metrics

---

## Key Findings
1. **Data Quality**: The dataset contained missing values represented by "?" which were imputed with mode values.
2. **Feature Importance**: Chest pain type (CP) was the most important feature in the decision tree.
3. **Model Improvement**: Pruning improved accuracy from 61.5%/70.3% to 76.9%/81.1% for negative/positive cases respectively.
4. **Cross-Validation**: K-fold CV helped select the optimal pruning parameter (ccp_alpha = 0.0159).

---

## How to Use This Notebook
1. Clone the repository
2. Install required libraries (pandas, numpy, matplotlib, seaborn, scikit-learn)
3. Run the Jupyter notebook sequentially
4. Experiment with different ccp_alpha values to see their effect on model performance

---

## Future Improvements
- Experiment with ensemble methods (Random Forest, Gradient Boosting)
- Perform more detailed feature importance analysis
- Try different imputation strategies for missing values
- Implement class balancing techniques if needed

---

## Acknowledgments
- UCI Machine Learning Repository for the dataset
- Scikit-learn documentation for implementation guidance
