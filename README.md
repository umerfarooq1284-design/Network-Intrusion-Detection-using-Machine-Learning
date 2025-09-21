### Network-Intrusion-Detection-using-Machine-Learning

## Project Description
This project focuses on detecting Distributed Denial of Service (DDoS) attacks using machine learning. A dataset with 85 features and over 35,000 records was analyzed and processed. Three classification models — Random Forest, XGBoost, and LightGBM — were implemented, compared, and evaluated using accuracy, precision, recall, F1-score, and confusion matrices. The goal is to identify the most effective model for real-time DDoS detection.

## Repository Structure
├── README.md              # Project documentation  
├── Liscense.md                  
├── requirements.txt       # Required libraries  
├── project.ipynb   # Jupyter Notebook with full implementation  

## Dataset Information
1. Shape: 35,357 samples × 85 features
2. Target Column: Attack category (DDoS vs Normal)
3. Features: Includes traffic statistics such as duration, packet length, protocol, flow rates, etc.

## Models Implemented
# 1. Random Forest
Pipeline: Data preprocessing → Train-test split → Random Forest Classifier → Evaluation

Pros: Handles high-dimensional data, interpretable feature importance, robust against overfitting.

Cons: Slower on large datasets, may require hyperparameter tuning.
# 2. XGBoost
Pipeline: Data preprocessing → Train-test split → XGBoost Classifier → Evaluation

Pros: High accuracy, efficient with boosting, handles imbalanced data well.

Cons: Sensitive to hyperparameters, longer training time than Random Forest.
# 3. LightGBM
Pipeline: Data preprocessing → Train-test split → LightGBM Classifier → Evaluation

Pros: Very fast training, lower memory usage, excellent accuracy on large datasets.

Cons: Can overfit on small datasets, harder to interpret compared to Random Forest.

## Results (Sample)
| Model         | Accuracy | Precision | Recall | F1-score |
| ------------- | -------- | --------- | ------ | -------- |
| Random Forest | 98.45%   | 98.40%    | 98.50% | 98.45%   |
| XGBoost       | 99.10%   | 99.05%    | 99.15% | 99.10%   |
| LightGBM      | 99.30%   | 99.25%    | 99.35% | 99.30%   |

Best Model: LightGBM (highest accuracy & efficiency).

## Installation
git clone https://github.com/umerfarooq1284-design/Network-Intrusion-Detection-using-Machine-learning.git

cd Network-Intrusion-Detection-using-Machine-learning

pip install -r requirements.txt

## How to Run
Open the Jupyter Notebook and execute the cells:

jupyter notebook project.ipynb

## Future Work
1. Extend to real-time traffic monitoring.
2. Experiment with deep learning models (CNN, LSTM).
3. Optimize for deployment in production environments.


