# Secure-Finance-Analytics-Anomaly-Detection-and-Model-Comparison.

# Anomaly Detection in Financial Transactions

This project focuses on detecting anomalies in financial transactions using various machine learning algorithms. Anomalies can represent potentially fraudulent activities, making their detection crucial for maintaining the integrity of financial systems.

## Project Overview

The main objectives of this project are:

1. **Data Preprocessing:** The dataset is cleaned, normalized, and feature-selected to prepare it for modeling.

2. **Exploratory Data Analysis (EDA):** Data visualization techniques are applied to gain insights into the distribution, trends, and patterns within the dataset.

3. **Anomaly Detection Models:** Several machine learning algorithms including Isolation Forest, Local Outlier Factor (LOF), K-Means, DBSCAN, and One-Class SVM are employed for anomaly detection.

4. **Model Evaluation:** The models are evaluated based on precision, recall, F1 score, and accuracy to determine their effectiveness in detecting anomalies.

5. **User Input Prediction:** Users can input transaction data, and the trained models predict whether the transaction is normal or an anomaly.

## Getting Started

1. Clone the repository:
 git clone https://github.com/yourusername/financial-anomaly-detection.git

2. Install the required libraries:

3. Run the main script:

## Data

The dataset utilized for this project consists of transactional information, encompassing attributes such as transaction amount, average transaction amount, frequency of transactions, and more. Below is a summary of the key features present in the dataset:

Feature	Description
Transaction_ID : Unique identifier for each transaction
Transaction_Amount : Monetary value associated with the transaction
Transaction_Volume :	Number of transactions made by each user
Average_Transaction_Amount :	Mean transaction amount computed over a specific period
Frequency_of_Transactions :	Number of transactions made by each user
Time_Since_Last_Transaction : Time duration since the last transaction
Day_of_Week :	Day of the week when the transaction occurred
Time_of_Day :	Time of day when the transaction occurred
Age :	Age of the user making the transaction
Gender :	Gender of the user making the transaction
Income :	Income level of the user making the transaction


## Results

#### Isolation Forest:

- Highest F1 Score: 1.0
- High accuracy and F1 score for both classes
  
#### One-Class SVM:
- F1 Score: ~0.04
- Moderate accuracy with a higher recall for the anomaly class
  
#### DBSCAN:
- F1 Score: ~0.04
- Very low accuracy, but the algorithm shows some capability to detect anomalies with higher recall

#### K-Means:
- F1 Score: 0.0
- Low accuracy and F1 score for the anomaly class, struggling to detect anomalies

## Conclusion

Among the models tested, the Isolation Forest algorithm show promising results in detecting anomalies in financial transactions. The choice of the best model depends on the desired trade-off between precision, recall, and F1 score.

