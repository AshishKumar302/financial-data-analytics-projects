📊 Financial Data Analytics Projects – IBA Karachi

This repository contains two academic projects completed as part of the Financial Data Analytics course at IBA Karachi. The projects demonstrate analytical thinking, data modeling, and insights generation using real-world case studies and datasets.

📘 Midterm Project – Elon Musk vs OpenAI: For Whose Profit?

Type: Strategic Case Study & Presentation

Tools: PowerPoint, Desk Research, Industry Reports

🧠 Summary:
This project analyzed the evolving dynamics between Elon Musk and OpenAI, exploring the ethical, strategic, and commercial implications of OpenAI's transition from a nonprofit to a capped-profit organization. We critically examined how investor involvement and proprietary AI development created friction with the organization's original mission.

⭐ Key Insights:
Identified tensions between AI transparency and corporate control.

Evaluated Musk’s criticism of OpenAI's shift toward closed-source, profit-driven strategies.

Highlighted global regulatory implications for ethical AI governance.

📌 Deliverables:
Case Study Analysis Presentation (Midterm-Presentation.pdf)

Summary of key ethical and strategic debates in AI development


🔐 Final Project - Ethereum Wallet Fraud Detection using XGBoost & Optuna

This project aims to detect suspicious Ethereum wallet addresses based on their transaction behavior. Using a dataset of ~10,000 wallet addresses with 51 features, we built a high-performing fraud detection model by applying advanced feature engineering and hyperparameter tuning.

📊 Data Overview

The dataset includes transactional records of Ethereum wallets, capturing behavioral patterns such as:

Total and average Ether sent/received

Number of unique addresses interacted with

Transaction timing and frequency

The target variable is FLAG, where 1 indicates suspicious activity.

Preprocessing included:

Dropping irrelevant index columns

Handling missing values

Type conversion for categorical features

Scaling numeric values using MinMaxScaler

🧪 Modeling Approach
Baseline Comparison:
We tested six algorithms (including Random Forest, LightGBM, and XGBoost) and found top-performing models. However, initial results showed signs of data leakage and overfitting.

Algorithm Selection:
We selected XGBoost for its proven track record in fraud detection (e.g., PayPal) and strong performance in academic research.

Hyperparameter Tuning:
Leveraged Optuna to run 100 optimization trials for XGBoost, tuning:

max_depth, learning_rate, subsample, colsample_bytree, gamma, reg_alpha, and reg_lambda

Evaluation metric: ROC-AUC via 5-fold cross-validation

🧠 Feature Engineering & Insights

Developed new behavioral features to better capture fraudulent patterns:

address_interaction_concentration: measures if funds are repeatedly sent to a single address (possible funneling)

dormancy_activity_ratio: flags accounts that become highly active after long dormancy

sent_received_imbalance: detects disproportionate transaction behavior

ERC20_token_diversity: captures the number of token types used by a wallet

Feature importance analysis revealed that engineered features significantly contributed to predictive power.

📈 Final Model Performance

The enhanced XGBoost model, trained on engineered features and fine-tuned using Optuna, demonstrated strong and balanced performance across key fraud detection metrics:

Accuracy: 94.52%

Precision: 87.61%

Recall: 87.61%

F1 Score: 87.61%

ROC-AUC: 0.9828

Cross-Validated F1 Score: 0.8680 ± 0.0096

🔍 Confusion Matrix (Enhanced Model)

Predicted: 0	Predicted: 1

Actual: 0 (Non-Fraud)	✅ 1479 (True Negatives)	❌ 54 (False Positives)

Actual: 1 (Fraud)	❌ 54 (False Negatives)	✅ 382 (True Positives)

✅ Per-Class Accuracy:

Non-Fraud (Class 0): 96.48%

Fraud (Class 1): 87.61%

These results highlight the model’s effectiveness in detecting fraudulent behavior while minimizing false alarms, making it well-suited for real-world blockchain fraud detection tasks.

