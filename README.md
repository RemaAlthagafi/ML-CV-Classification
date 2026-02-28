<<<<<<< HEAD
# CV Classification using Machine Learning

## **Problem Statement**
This project automates the classification of resumes (CVs) into predefined job categories using machine learning techniques. The goal is to improve the efficiency of HR processes by automating the initial resume screening stage.

## **Dataset**
- **Source**: [Resume Classification Dataset](https://www.kaggle.com/datasets/nitinsen001/resume-classification-dataset-for-nlp-and-ml)
- The dataset contains resumes with job categories and candidate details.
- **Challenges**: The dataset is multi-class and exhibits imbalance across categories.

## **My Contributions**
- **Data Preprocessing**: I cleaned the dataset by handling missing values, filtering out unrealistic experience values, and normalizing labels.
- **Model Development**: I built and trained machine learning models to classify resumes into job categories. I utilized **SBERT** for semantic text embeddings and **Logistic Regression** for classification. Additionally, I applied **SMOTE** to handle class imbalance.

## **Objectives**
1. **Resume Classification**: Automatically categorize resumes into predefined job categories using semantic text representations.
2. **Fairness & Bias Assessment**: Evaluate and correct unfair bias across experience levels (junior, mid, senior).

## **Approach**

### **Pipeline A – Resume Classification (SBERT + Logistic Regression + SMOTE)**
- **SBERT** (all-MiniLM-L6-v2) for generating 384-dimensional embeddings.
- **SMOTE** for oversampling minority classes.
- **Logistic Regression** classifier with class balancing.
- Evaluation using **Precision**, **Recall**, **F1-score**, and **ROC-AUC**.

### **Pipeline B – Fairness Assessment (TF-IDF + SVM + Fairlearn)**
- **TF-IDF** (unigrams + bigrams) for text representation.
- **Linear SVM** for classification.
- **Fairness metrics** including demographic parity and equalized odds.

## **Workflow**
1. **Load and clean dataset**  
2. **Encode labels** and split dataset into training/testing sets  
3. **Branch into**:
    - **SBERT → SMOTE → Logistic Regression** for classification  
    - **TF-IDF → SVM → Fairness Assessment**
4. **Output predictions** and **fairness metrics** for evaluation.

## **Results**
- **SBERT Classifier**:
    - **Accuracy**: ≈ 0.73
    - **Macro F1-score**: ≈ 0.66
    - **ROC-AUC**: ≈ 0.97
- **Fairness**: Significant improvement in categories with balanced data.

## **Conclusion**
This project demonstrates that combining semantic embeddings with machine learning pipelines improves both classification accuracy and fairness in resume screening. Future work can focus on expanding datasets and exploring advanced fairness techniques to ensure a more equitable model.
=======
# ML-CV-Classification
This project automates resume classification into job categories using machine learning.
>>>>>>> 4792e1e565ecb2a70215932fce55871dc2722785
