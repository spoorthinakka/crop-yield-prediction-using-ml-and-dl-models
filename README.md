# **Crop Yield Prediction Using Machine Learning and Deep Learning Models**

A complete implementation of crop yield prediction for the **mustard crop** using a reservoir-based dataset.
The project integrates both Machine Learning (ML) and Deep Learning (DL) approaches to forecast yield with improved accuracy and reliability.

---

## **Overview**

Accurate crop yield forecasting is a critical component of modern agricultural planning and policy formulation.
Conducted as part of an internship research initiative under the Technology Innovation Hub (TIH), Indian Statistical Institute (ISI), Kolkata, this work employs data-driven predictive modeling to analyze the influence of climatic and reservoir parameters on mustard crop yield.
By integrating regression-based Machine Learning (ML) techniques with sequential Deep Learning (DL) architectures, the study effectively captures both static and temporal dependencies within the dataset to achieve precise and reliable yield estimations.

---

## **Dataset Information**

Two datasets are available under the datasets/ directory:

- **merged_mustard_reservoir.csv** – Raw dataset containing unprocessed climatic and reservoir data.
- **cleaned_mustard_reservoir_dataset.csv** – Preprocessed dataset obtained after data cleaning, normalization, and feature selection.

Each dataset includes parameters such as rainfall, temperature, humidity, live storage, inflow, and outflow, which significantly impact yield prediction.

---

## **Models Implemented**

**Machine Learning Models**
- **Random Forest Regressor (RFR):** Baseline ensemble model for non-linear yield prediction.
- **XGBoost Regressor:** Gradient boosting algorithm that provides improved accuracy and interpretable feature importance.

**Deep Learning Models**
- **LSTM (Long Short-Term Memory):** Learns sequential dependencies and seasonal variations in reservoir and climatic data.
- **BiLSTM (Bidirectional LSTM):** Enhances LSTM by processing sequences in both forward and backward directions to improve performance.

---

## **Evaluation Metrics**

All models are evaluated using key regression performance metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R² Score)

Visual analyses such as Actual vs Predicted and Residual plots are included to assess prediction accuracy and model reliability.

---

## **Project Structure**
```
├── datasets/
│   ├── merged_mustard_reservoir.csv
│   └── cleaned_mustard_reservoir_dataset.csv
├── mustard_reservoir_yield_prediction.ipynb
├── lstm_model.ipynb
├── bilstm_model.ipynb
├── requirements.txt
├── PROJECT_SETUP.txt
├── .gitignore
└── README.md
```

---

## **Setup and Execution**

**Step 1 – Clone the repository**
```
git clone https://github.com/spoorthinakka/crop-yield-prediction-using-ml-and-dl-models.git
cd crop-yield-prediction-using-ml-and-dl-models
```

**Step 2 – Create and activate a virtual environment**
```
python -m venv venv
.\venv\Scripts\activate     # For Windows

# or

source venv/bin/activate    # For macOS/Linux
```

**Step 3 – Install dependencies**
```
pip install -r requirements.txt
```

**Step 4 – Run the notebooks**

- mustard_reservoir_yield_prediction.ipynb → RFR and XGBoost models
- lstm_model.ipynb → LSTM model
- bilstm_model.ipynb → BiLSTM model
Execute cells sequentially to train, test, and evaluate model performance.

---

## **System Requirements**

- Python 3.10 or later
- Minimum 8 GB RAM (recommended for deep learning models)
- GPU (optional) for faster model training
- Compatible with Windows, macOS, or Linux

---

## **Author**

Nakka Sai Spoorthi, 
B.Tech – CSE (AI & ML), Institute of Aeronautical Engineering (IARE)
Conducted under the Technology Innovation Hub (TIH), ISI Kolkata as part of an internship research project on crop yield prediction.
