#  Customer Churn Prediction

This project predicts whether a customer will churn (leave) based on various behavioral and demographic factors. It uses machine learning techniques with a focus on **Random Forest Classifier** along with **hyperparameter tuning**, and provides an interactive interface using **Gradio**.

![Image](https://github.com/user-attachments/assets/f5bbf261-7bd8-4c74-8a03-b593d4303e9c)

---
## About Dataset

Taken from https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling

This dataset contains info on **10,000 bank customers**, used to predict **customer churn** (whether a customer will leave the bank). It includes demographic, financial, and account activity features.

### Features:
- `CreditScore`, `Geography`, `Gender`, `Age`, `Tenure`
- `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`
- `Exited` → Target (1 = customer left, 0 = stayed)

 **Clean data**  
 Balanced feature variety  
 Ideal for classification models & churn prediction

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

## Live Demo at:https://mehtahet619-customerchurn.hf.space/

## 🚀 Run Locally

```bash
# Clone the repository
git clone https://github.com/yourusername/churn-prediction.git
cd churn-prediction

# Install dependencies
pip install -r requirements.txt

# Run the Gradio app
python app.py




