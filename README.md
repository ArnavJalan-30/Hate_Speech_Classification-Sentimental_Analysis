# **Hate Speech Detection Project**

This repository contains the code, dataset, and report for the **Hate Speech Detection Project**, which classifies tweets into three categories:  
1. **Hate Speech**  
2. **Offensive Language**  
3. **Neither**  

The project explores and implements **machine learning models** such as **Logistic Regression** and **Naive Bayes** to achieve effective text classification using a preprocessed dataset of tweets.

---

## **Repository Structure**
- `labeled_data.csv`: The dataset containing labeled tweets for training and testing.
- `hate_speech_classification_final.ipynb`: Jupyter Notebook implementing data preprocessing, feature extraction, and model training for hate speech detection.
- `Hate_Speech_Detection_Report.docx`: Comprehensive report describing the project objectives, methods, results, and conclusions.

---

## **Project Overview**
### **Objective**
To classify tweets into the above three categories using **machine learning techniques** while ensuring high precision and recall, particularly in detecting hate speech.

### **Dataset**
The dataset contains:
- ~25,000 tweets.
- Each tweet is labeled as **Hate Speech**, **Offensive Language**, or **Neither**.

### **Methods Used**
1. **Preprocessing:**
   - Text data is cleaned by removing URLs, mentions, hashtags, and non-alphanumeric characters.
   - All text is converted to lowercase, and unnecessary spaces are removed.

2. **Feature Extraction:**
   - **TF-IDF Vectorization**:
     - Converts text data into numerical vectors using unigrams, bigrams, and trigrams.
     - Captures word importance based on term frequency and document frequency.

3. **Balancing Data:**
   - **SMOTE (Synthetic Minority Oversampling Technique)**:
     - Balances the dataset by generating synthetic samples for underrepresented classes.

4. **Machine Learning Models:**
   - **Logistic Regression:**
     - Uses softmax for multi-class classification.
     - Optimizes weights using gradient descent with L2 regularization to prevent overfitting.
   - **Naive Bayes:**
     - Calculates class probabilities and word likelihoods with Laplace smoothing.
     - Classifies based on the maximum posterior probability.

---

## **Results Achieved**
- **Logistic Regression**:
  - High precision = 84.7% , recall = 84.6% , and F1 score = 84.3%  for all classes.
  - Performs better than Naive Bayes due to regularization and probabilistic output.
- **Naive Bayes**:
  - Precision = 87.4% , recall = 80.99% , and F1 score = 83.33%  for all classes.
  - Simple and efficient, with good baseline performance.
  - Handles high-dimensional data effectively using Laplace smoothing.

### **Evaluation Metrics**
- **Precision**: Measures the accuracy of positive predictions.
- **Recall**: Measures the ability to identify all true positives.
- **F1-Score**: Harmonic mean of precision and recall.
- **Confusion Matrix**: Highlights true positives, true negatives, false positives, and false negatives.

---

