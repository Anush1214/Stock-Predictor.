# 📈 Stock Price Predictor using LSTM

A **deep learning-based Stock Price Predictor** that leverages **LSTM (Long Short-Term Memory)** networks to forecast future stock prices based on historical closing data.  
This project provides a data-driven approach to stock trend analysis using publicly available data from **Yahoo Finance**.

---

## 🧠 Project Overview

Stock markets are highly dynamic and influenced by numerous factors.  
This project demonstrates how machine learning can be applied to time series data to **analyze trends and predict future stock prices**.  

The notebook automates:
- Fetching historical stock data  
- Preprocessing and scaling data  
- Building and training an LSTM model  
- Visualizing real vs predicted stock trends  

---

## ⚙️ Tech Stack

| Category        | Technologies Used                                         |
| --------------- | --------------------------------------------------------- |
| **Language**    | Python 🐍                                                 |
| **Data Source** | Yahoo Finance (`yfinance` API)                            |
| **Libraries**   | NumPy, Pandas, Matplotlib, Scikit-learn, TensorFlow/Keras |
| **Model**       | LSTM (Sequential Neural Network)                          |
| **Interface**   | Jupyter Notebook                                          |

---

## 🧩 How It Works

### 1. Data Collection
Fetches historical stock data from Yahoo Finance for a specified ticker (e.g., `AAPL`, `TSLA`, `GOOG`).

### 2. Data Preprocessing
- Uses only the **Close** price for prediction  
- Applies **MinMax scaling** to normalize the dataset  
- Generates **60-day time sequences** for training  

### 3. Model Building
- Constructs an **LSTM-based Sequential model**  
- Uses **two stacked LSTM layers** with Dense output  
- Optimized using **Adam optimizer** and **MSE loss**  

### 4. Training & Prediction
- Splits dataset into **training and testing sets**  
- Trains the model on historical data  
- Predicts and visualizes the future trend  

### 5. Visualization
- Plots **actual vs predicted stock prices** using Matplotlib  
- Provides intuitive insight into model performance  

---

## 🚀 Getting Started

### 🔧 Installation

Clone the repository:
```bash
git clone https://github.com/Anush1214/Stock-Predictor.git
cd Stock-Predictor-main
Install the required dependencies:

pip install numpy pandas yfinance scikit-learn tensorflow matplotlib

▶️ Run the Notebook

Open Jupyter Notebook and execute:

jupyter notebook
