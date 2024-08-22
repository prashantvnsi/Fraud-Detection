# Insurance Fraud Detection Project

## Project Overview

This project focuses on developing a robust predictive model for an insurance company to assess the likelihood or level of risk a customer poses regarding potential fraud. The model aims to strike a balance between accurately identifying fraudulent claims and minimizing the referral of genuine claims, which can lead to customer loss and additional costs for the company.

## Project Objectives

The specific objectives of this project include:

1. **Data Pre-processing**:
   - Handle noise, remove irrelevant attributes, address missing values, and mitigate class imbalance in the dataset to ensure high-quality input for model training.
  
2. **Model Building and Training**:
   - Develop two distinct predictive models using Random Forest and K-Nearest Neighbors (KNN), ensuring they are trained on pre-processed data and free from overfitting.

3. **Performance Evaluation**:
   - Assess the models using key performance metrics such as Precision, Recall, F1 Score, and Balanced Accuracy. The goal is to maintain a balanced error rate of 5%, though this might not be fully achievable.

4. **Loss Quantification**:
   - Develop a pricing model to quantify potential losses from misclassifications, and assess the impact of false positives and false negatives on the company's financials.

5. **Documentation and Presentation**:
   - Document the analysis process and present the findings in a Jupyter notebook with embedded code, along with a formal report outlining the methodology, results, and recommendations.

## Data Preprocessing

The dataset underwent comprehensive preprocessing steps:

- Noise removal and irrelevant attribute filtering.
- Handling of missing values.
- Mitigation of class imbalance using appropriate techniques.

## Modeling Techniques

Two modeling techniques were used:

1. **Random Forest**:
   - Employed hyperparameter tuning to optimize the model's performance.
   - **Metrics**:
     - **Balanced Accuracy**: 0.8684
     - **Class N**: Precision - 0.9222, Recall - 0.9614, F1-score - 0.9414
     - **Class Y**: Precision - 0.8787, Recall - 0.7754, F1-score - 0.8239

2. **K-Nearest Neighbors (KNN)**:
   - Hyperparameter tuning was applied to improve prediction accuracy.
   - **Metrics**:
     - **Balanced Accuracy**: 0.8907
     - **Class N**: Precision - 0.9353, Recall - 0.9666, F1-score - 0.9507
     - **Class Y**: Precision - 0.8980, Recall - 0.8148, F1-score - 0.8544

## Model Comparison and Results

- Both models were compared based on the above metrics.
- ROC (Receiver Operating Characteristic) curves were generated to visualize the performance of each model.
- The performance of the KNN model slightly outperformed the Random Forest model in terms of Balanced Accuracy and F1-score for the positive class (Class Y).

## Conclusion

- Both models provided valuable insights into predicting fraudulent claims.
- The KNN model showed a slight edge over Random Forest in terms of overall accuracy and precision-recall balance.
- The project successfully demonstrated the application of machine learning techniques to real-world insurance fraud detection, offering a foundation for further refinement and deployment in production environments.

## How to Run

1. Clone the repository.
2. Install the required libraries. Import statements will help.
3. Run the Jupyter notebook to view the analysis and results.

## Future Work

- Further refine the models to improve precision for the positive class.
- Explore additional algorithms and ensemble methods to enhance prediction accuracy.
- Implement the model in a real-time environment to assess its performance with live data.
