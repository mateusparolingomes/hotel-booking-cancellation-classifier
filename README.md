# 🤖 Hotel Cancellation Prediction (Machine Learning Classifier)

This project applies supervised machine learning to predict hotel booking cancellations using real-world reservation data. It compares classification algorithms and tunes hyperparameters to improve predictive performance and extract actionable business insights for the hospitality industry.

## 📊 Dataset

- **Source**: [Hotel Booking Demand Dataset – Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **Observations**: 119,390 bookings from City and Resort hotels
- **Target Variable**: `is_canceled` (1 = canceled, 0 = honored)
- **Features**: Lead time, customer type, deposit type, room type, market segment, booking changes, and more

## 🧠 Machine Learning Models

The following classification models were trained and evaluated:

- Decision Tree (GridSearchCV tuning)
- Bagging Classifier
- AdaBoost Classifier
- XGBoost Classifier (with learning rate tuning)
- Multi-Layer Perceptron (Neural Network)

## 📈 Evaluation Metrics

Model performance was assessed using accuracy, precision, recall, F1-score, and a confusion matrix due to class imbalance in the target variable.

| Model              | Accuracy (Test Set) |
|-------------------|---------------------|
| XGBoost           | ~88.5%              |
| Neural Network    | ~87.9%              |
| Decision Tree (tuned) | ~86.4%         |
| Bagging           | ~85.6%              |
| AdaBoost          | ~84.7%              |

## 🔍 Key Insights

- Longer **lead time** is a strong indicator of cancellations.
- **Non-refundable deposits** increase cancellation likelihood.
- **City hotels** and **single travelers** are more prone to cancel.
- Most cancellations occur during **weekdays** and **short stays**.

## 💡 Business Recommendations

- **Overbooking Strategy**: Adjust overbooking limits dynamically based on predicted cancellation risk.
- **Flexible Deposit Policies**: Tailor deposit requirements using model risk scores.
- **Guest Segmentation**: Prioritize offers for couples and families with lower predicted cancellation rates.
- **Marketing Timing**: Focus campaigns around low cancellation periods identified by the model.

## ⚙️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

## ✍️ Author

Mateus Parolin Gomes  
Master in Business Analytics @ Hult International Business School  
[GitHub](https://github.com/mateusparolingomes) | [LinkedIn](https://www.linkedin.com/in/mateusparolingomes/)
