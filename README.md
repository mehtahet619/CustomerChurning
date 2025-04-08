# CustomerChurning
#  Customer Churn Prediction

This project predicts whether a customer will churn (leave) based on various behavioral and demographic factors. It uses machine learning techniques with a focus on **Random Forest Classifier** along with **hyperparameter tuning**, and provides an interactive interface using **Gradio**.

---

##  Features

-  Data Preprocessing (null handling, encoding, feature selection)
-  Model Training: Random Forest Classifier with RandomizedSearchCV & GridSearchCV
-  Model Evaluation: Accuracy, confusion matrix, classification report
-  Gradio-based user interface for live predictions
-  Open-source & easy to extend

---

##  Tech Stack

- Python 3.11
- Pandas, NumPy
- Scikit-learn (RandomForestClassifier, RandomizedSearchCV, GridSearchCV)
- Matplotlib, Seaborn (for performance visualization)
- Gradio (for GUI)
- Joblib (for model saving/loading)

---

##  Model Performance

| Model Variant        | Accuracy | Wrong Predictions (out of 2000) |
|----------------------|----------|-------------------------------|
| RandomForest (RandomizedSearchCV) | 87%      | 243                          |
| RandomForest (GridSearchCV)       | 87%      | 246                          |

> Decision Tree showed signs of overfitting and was excluded from final deployment.

---

## 🚀 Run Locally

```bash
# Clone the repository
git clone https://github.com/yourusername/churn-prediction.git
cd churn-prediction

# Install dependencies
pip install -r requirements.txt

# Run the Gradio app
python app.py
