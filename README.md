# Madaline (Multiple Adaptive Linear Neuron) - Lung Cancer Prediction System

This project implements a **Madaline (Multiple Adaptive Linear Neuron)** model to predict lung cancer risk based on specific features collected from individuals. The aim is to assist people in understanding their cancer risk at a low cost and make informed decisions based on their risk assessment.

## 📋 Dataset Overview

- **Purpose**: The dataset measures the effectiveness of a lung cancer prediction system.
- **Total Features**: 16
- **Total Observations**: 309
- **Target Variable**: `LUNG_CANCER` (YES=1, NO=0)

### Features:

| Feature               | Description                   | Values           |
|-----------------------|-------------------------------|------------------|
| GENDER               | Gender of the individual      | Male=1, Female=0 |
| AGE                  | Age of the individual         | Integer values   |
| SMOKING              | Smoking status                | Yes=1, No=0      |
| YELLOW_FINGERS       | Yellow fingers due to smoking | Yes=1, No=0      |
| ANXIETY              | Anxiety                       | Yes=1, No=0      |
| PEER_PRESSURE        | Peer pressure                 | Yes=1, No=0      |
| CHRONIC DISEASE      | Chronic disease presence      | Yes=1, No=0      |
| FATIGUE              | Fatigue                       | Yes=1, No=0      |
| ALLERGY              | Allergies                     | Yes=1, No=0      |
| WHEEZING             | Wheezing                      | Yes=1, No=0      |
| ALCOHOL CONSUMING    | Alcohol consumption           | Yes=1, No=0      |
| COUGHING             | Coughing                      | Yes=1, No=0      |
| SHORTNESS OF BREATH  | Shortness of breath           | Yes=1, No=0      |
| SWALLOWING DIFFICULTY| Swallowing difficulty         | Yes=1, No=0      |
| CHEST PAIN           | Chest pain                    | Yes=1, No=0      |
| LUNG_CANCER          | Lung cancer diagnosis         | YES=1, NO=0      |

---

## 🔍 Exploratory Data Analysis (EDA)

- **Visualization**: Correlation heatmaps and distribution plots were used to explore the relationships between features.
- **Key Insights**:
  - Strongest positive correlation observed between `YELLOW_FINGERS` and `ANXIETY` (0.57).
  - Dataset contains no missing values.
  - Dataset balanced for most features.

---

## ⚙️ Data Preprocessing

- One-hot encoding was applied to categorical variables (`GENDER` and `LUNG_CANCER`).
- Binary features were mapped to `0` (No) and `1` (Yes).
- Features were scaled and split into training (75%) and testing (25%) sets using `train_test_split`.

---

## 🤖 Model Implementation: Madaline

- A **Madaline Neural Network** was implemented for prediction.
- **Activation Function**: Bipolar step activation function.
- **Training Process**:
  - Weights were updated iteratively based on error correction.
  - Epoch limit: 1000
  - Learning rate: 0.01
- **Testing Process**:
  - Predictions were evaluated using the trained weights and activation logic.

---

## 📊 Results and Evaluation

- Metrics:
  - **Confusion Matrix**: Used to visualize the model’s performance.
  - **Accuracy Score**: Evaluates the model's prediction capability.
  - **Classification Report**: Provides precision, recall, and F1-score.

---

## 📚 Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - `pandas` and `numpy` for data handling.
  - `seaborn` and `matplotlib` for visualizations.
  - `scikit-learn` for preprocessing and evaluation metrics.

---

## 🚀 How to Use

1. Clone the repository and load the dataset.
2. Run the notebook to preprocess data and train the model.
3. Use the trained model to predict lung cancer risk for new individuals.

---

## 🛠️ Future Improvements

- Optimize the Madaline algorithm for better performance.
- Experiment with other neural network architectures (e.g., MLP or CNN).
- Apply feature engineering for improved insights.

---



