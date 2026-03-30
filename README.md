# Fraud-Detection-Neural-Network
Fraud Detection Neural Network

A deep learning project to detect fraudulent credit card transactions using a neural network model built with TensorFlow/Keras.

## Project Overview

This project implements a neural network classifier to identify fraudulent credit card transactions. It uses the Credit Card Fraud Detection dataset and applies data preprocessing, exploratory data analysis, and deep learning techniques to build a robust fraud detection model.

## Installation Requirements

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Required Packages

Install all dependencies using:

```bash
pip install -r requirements.txt
```

Or install individually:

```bash
# Data Processing and Analysis
pip install pandas numpy

# Data Visualization
pip install matplotlib seaborn

# Machine Learning & Preprocessing
pip install scikit-learn

# Deep Learning
pip install tensorflow keras

# Optional: For Jupyter Notebook
pip install jupyter notebook ipython
```

**Package Versions:**
- pandas >= 1.3.0
- numpy >= 1.21.0
- matplotlib >= 3.4.0
- seaborn >= 0.11.0
- scikit-learn >= 1.0.0
- tensorflow >= 2.8.0
- keras (included with tensorflow)

## 📊 Dataset

### About the Dataset
The project uses the **Credit Card Fraud Detection Dataset** containing transactions made by credit cards in September 2013 by European cardholders.

**Dataset Characteristics:**
- Total Transactions: 284,807
- Fraudulent Transactions: 492 (0.172%)
- Features: 30 (V1-V28, Time, Amount)
- Target Variable: Class (0 = Normal, 1 = Fraud)

### Dataset Download

**Option 1: Kaggle Dataset (Recommended)**
- Source: [Credit Card Fraud Detection - Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Download Instructions:
  1. Create a Kaggle account (free)
  2. Visit the dataset link above
  3. Click "Download" button
  4. Extract `creditcard.csv` to the project root directory

**Option 2: Direct UCI ML Repository**
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/492/credit+card+fraud+detection)

### Dataset File Location
Place the `creditcard.csv` file in the project root directory:
```
Fraud Detection Neural Network/
├── creditcard.csv          ← Put the CSV file here
├── Fraud_Detection_Neural_Network.ipynb
├── fraud_detection_model.h5
└── README.md
```

## Usage

### Running the Notebook

1. Activate virtual environment (if you have one):
   ```bash
   .venv\Scripts\Activate.ps1  # Windows PowerShell
   source .venv/bin/activate   # Linux/Mac
   ```

2. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open `Fraud_Detection_Neural_Network.ipynb`

4. Run all cells or execute them sequentially

### Project Structure

- **Data Loading & Exploration**: Load CSV and analyze dataset distribution
- **Data Preprocessing**: Handle class imbalance, normalize features
- **Model Building**: Neural network architecture with feedback
- **Training & Evaluation**: Train model and evaluate with multiple metrics
- **Model Evaluation**: ROC curve, confusion matrix, classification report
- **Model Saving**: Save trained model as `fraud_detection_model.h5`

##  Key Metrics

The model is evaluated using:
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)
- ROC-AUC Score
- ROC Curve Visualization

##  Model Output

The trained model is saved as:
- `fraud_detection_model.h5` - Trained neural network model

##  Notes

- This is a **highly imbalanced dataset** (frauds < 1%) - appropriate techniques are applied
- Features V1-V28 are already PCA-transformed (confidentiality)
- Model performance is evaluated with focus on recall and precision for fraud detection

## 🔗 Resources

- [TensorFlow Documentation](https://www.tensorflow.org/)
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Kaggle Competition](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Gopolang Rodney Diutlwileng
