# Twitter Sentiment Analysis — LSTM & RNN

> 🎓 Final Graduation Project | Route Academy — AI Track

---

## Overview

This project analyzes tweets and classifies their sentiment into three categories:
- **Positive (0)**
- **Negative (2)**  
- **Neutral (1)**

Two deep learning models were built and compared: **LSTM** and **RNN**, both trained on a real-world Twitter dataset of 60,000+ tweets.

---

## Project Structure

```
├── Data/               # Raw and processed CSV datasets
│   ├── data.csv
│   ├── data_new.csv
│   ├── twitter_training.csv
│   ├── X_train_data.csv
│   ├── X_test_data.csv
│   ├── y_train_data.csv
│   └── y_test_data.csv
│
├── Notebook/           # Jupyter notebooks
│   ├── Preprocessing (1).ipynb   # Data cleaning & preprocessing
│   └── Project_LSTM&RNN.ipynb    # Model building & training
│
├── Output/             # Saved trained models
│   ├── model_LSTM.h5
│   └── model_RNN.h5
│
└── README.md
```

---

## Workflow

1. **Data Preprocessing** — Cleaning tweets, removing nulls and duplicates, tokenizing text
2. **Feature Engineering** — Tokenization + Padding sequences
3. **Class Balancing** — Using class weights to handle imbalanced labels
4. **Model Building** — Two sequential models with stacked LSTM / RNN layers + Dropout regularization
5. **Training & Evaluation** — Trained with Adam optimizer, sparse categorical cross-entropy loss

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| TensorFlow / Keras | Model building |
| Pandas / NumPy | Data manipulation |
| Scikit-learn | Preprocessing & evaluation |
| Matplotlib / Seaborn | Visualization |

---

## Models

### LSTM Model
- 4 stacked LSTM layers (128 → 256 → 256 → 64 units)
- Embedding layer + Dropout (0.5)
- L1/L2 regularization

### RNN Model
- 4 stacked SimpleRNN layers (128 → 256 → 256 → 64 units)
- Embedding layer + Dropout (0.5)
- L1/L2 regularization

---

## About

This project was developed as the **Final Graduation Project** for the **AI Track at Route Academy**. It covers the full pipeline from raw data to trained models, with a focus on text sequence modeling.

---

*Built with dedication and a lot of training epochs* ☕
