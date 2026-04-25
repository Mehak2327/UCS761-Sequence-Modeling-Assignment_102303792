# 📊 Sequence Modeling Assignment – UCS761

## 👩‍🎓 Student Details

* **Name:** Mehak
* **Roll Number:** 102303792
* **Course:** UCS761 – Sequence Modeling

---

## 📌 Project Overview

This project implements a **time-series forecasting pipeline from scratch** as part of the UCS761 coursework.
The goal is to understand how sequence models utilize past information to predict future values and analyze their performance.

---

## ⚙️ Personalized Parameters

Derived using roll number (102303792):

* **Window Size:** 15
* **Prediction Horizon:** 3
* **Hidden Size:** 14

---

## 🧠 Models Implemented

### 1. MLP (Baseline)

* Treats input as a flat vector
* No sequence awareness
* Used for comparison

### 2. Custom RNN (From Scratch)

* Implemented manually using linear layers
* Uses hidden state to capture temporal dependencies
* Does NOT use `nn.RNN`

### 3. LSTM (Prebuilt)

* Handles long-term dependencies better
* Used for comparison

### 4. Transformer (Prebuilt)

* Captures global dependencies using attention
* Used for comparison

---

## 📊 Datasets Used

### 1. Synthetic Dataset

* Generated using sine wave + noise
* Helps understand model behavior clearly

### 2. Electricity Dataset

* Real-world time series dataset
* Loaded locally from CSV
* Preprocessed using:

  * Missing value handling
  * Normalization (MinMaxScaler)

---

## 🔄 Pipeline Workflow

1. Data Loading
2. Preprocessing
3. Windowing (Sliding Window Technique)
4. Chronological Train-Test Split
5. Model Training
6. Evaluation
7. Visualization

---

## 📈 Evaluation Metrics

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

---

## 📉 Visualizations

* Training Loss Curve
* Prediction vs Actual Graphs
* Separate plots for multi-step predictions

---

## 🔬 Ablation Study

Experiments conducted with:

| Window Size | Description        |
| ----------- | ------------------ |
| 7           | Reduced context    |
| 15          | Optimal (baseline) |
| 30          | Increased context  |

### 🔍 Observations:

* Smaller window → insufficient context → poor performance
* Larger window → noise + overfitting
* Optimal window → balanced performance

---

## ⚠️ Model Limitations

* Error accumulation in multi-step prediction
* RNN struggles with long-term dependencies
* Performance drops on real-world noisy data

---

## 🚀 How to Run

1. Open the notebook in Google Colab
2. Upload the dataset (CSV file)
3. Run all cells sequentially
4. View results and plots

---

## 📌 Key Learnings

* Importance of sequence modeling
* Difference between MLP and RNN
* Impact of window size
* Challenges in real-world forecasting

---

## 🙌 Acknowledgment

This assignment was completed under the guidance of **Sukhpal Singh**,
Research Associate, Computer Science Department,
Thapar Institute of Engineering & Technology (TIET).

---
