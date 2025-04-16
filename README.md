# 🏨 Hotel Booking Cancellation Classifier  

This project predicts hotel booking cancellations using historical reservation data, offering insights to optimize hotel operations, minimize no-shows, and improve revenue forecasting. Multiple supervised machine learning models were applied, tuned, and compared to identify the best-performing classifier.

## 📊 Dataset

- **Source**: [Hotel Booking Demand Dataset on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **Features**: Includes 32 variables such as booking dates, guest details, lead time, deposit type, customer type, and more
- **Target**: `is_canceled` – 1 if booking was canceled, 0 otherwise

## 🧠 Models Used

The following classification models were trained and evaluated:
- Decision Tree (with GridSearch tuning for `max_depth`, `min_weight_fraction_leaf`, `min_impurity_decrease`)
- Bagging Classifier
- AdaBoost Classifier
- XGBoost Classifier (with learning rate tuning)
- Neural Network (MLP Classifier)

## 📈 Evaluation Metrics

All models were evaluated using test accuracy, confusion matrix, precision, recall, and F1-score due to the class imbalance.

| Model              | Test Accuracy |
|-------------------|----------------|
| XGBoost           | ~88.5%         |
| Neural Network    | ~87.9%         |
| Tuned Decision Tree | ~86.4%       |
| Bagging           | ~85.6%         |
| AdaBoost          | ~84.7%         |

## 🔍 Key Insights

- **High lead time**, **non-refundable deposits**, and **short stays** are major predictors of cancellations
- **Weekday bookings** and **single travelers** have a higher chance of cancellation
- **City hotels** have higher cancellation rates compared to resort hotels

## 💡 Business Recommendations

- **Overbooking Buffer**: Implement strategic overbooking in City Hotels with high cancellation probability.
- **Flexible Booking Campaigns**: Target refundable bookings with loyalty perks to reduce cancellations.
- **Dynamic Deposit Policies**: Tailor deposit requirements based on predicted cancellation risk.

## ⚙️ Tools & Technologies

- Python
- Scikit-learn, XGBoost
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## ✍️ Author

Mateus Parolin Gomes  
Master in Business Analytics @ Hult International Business School  
[GitHub](https://github.com/mateusparolingomes) | [LinkedIn](https://www.linkedin.com/in/mateusparolingomes/)
