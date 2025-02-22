# Fetal Health Prediction Model

## 📌 Overview
This project is a **Fetal Health Prediction System** that uses **Machine Learning** techniques to classify fetal health based on various medical parameters. It leverages **Gradient Boosting Classifier** along with other models to predict whether a fetus is **healthy, at risk, or in distress** based on cardiotocography data.

## 🏥 Problem Statement
Fetal health monitoring is crucial during pregnancy to detect any potential risks. This project aims to **automate fetal health classification** using machine learning, which can assist doctors in early diagnosis and intervention.

## 🔧 Features
- **Loads and preprocesses the dataset** (scaling, missing value handling, and feature engineering)
- **Trains multiple ML models**, including:
  - Logistic Regression
  - Decision Tree
  - Gradient Boosting Classifier (final model)
  - Random Forest
  - K-Nearest Neighbors (KNN)
- **Performs hyperparameter tuning** using `GridSearchCV`
- **Evaluates models** using accuracy, confusion matrix, and classification reports
- **Provides a function for real-time predictions**

## 📂 Dataset
The dataset used in this project is **Fetal Health Classification** data, which contains various fetal health indicators. It consists of:
- **Features**: 21 medical parameters extracted from fetal cardiotocography tests
- **Target Variable**: `fetal_health` (1: Normal, 2: Suspect, 3: Pathological)

## 🚀 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/thetanmaymishraa/Bodhi_project.git
cd Bodhi_project
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Model
To execute the model and train it:
```bash
python fetal_health_model.py
```

## 🧑‍💻 Usage
### 📊 Training the Model
Run the script to preprocess data, train models, and evaluate their performance.

### 🩺 Making Predictions
The function `fetal_health_prediction()` takes medical parameters as input and returns a predicted fetal health category.

```python
from model import fetal_health_prediction

data = [2.85, 0.0, 0.25, 0.0, 0.0, 0.0, 0.0, 118.0, 0.54, 22.6, 106.0]
result = fetal_health_prediction(*data)
print(f"Predicted fetal health: {result}")
```

## 🌍 Live Deployment
You can access the **temporary deployed version** of this project here: **[Bodhi Fetal Health Predictor](https://bodhi-three.vercel.app/)**

## 📈 Model Performance
- **Accuracy of Gradient Boosting Classifier**: ~ **97%**
- **Confusion Matrix & Classification Report** included in results

## 🔥 Future Improvements
- Integrate **Deep Learning (Neural Networks)** for better accuracy
- Deploy as a **web or mobile application** for real-world usage
- Expand dataset to improve generalization

## 🤝 Contributing
Contributions are welcome! Feel free to fork this repository, make changes, and submit a pull request.

## 📜 License
This project is licensed under the **MIT License**.

---

### 🌟 If you find this project helpful, please ⭐ the repository!

