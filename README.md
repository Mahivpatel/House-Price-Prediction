# 🏡 House Price Prediction  

This project implements an **end-to-end machine learning pipeline** to predict **median house values** using demographic, geographic, and socio-economic features. It demonstrates the full workflow of data preprocessing, model training, evaluation, and deployment.  

---

## 📌 Features  
- **Data Preprocessing**:  
  - Median imputation for missing values  
  - Standardization of numerical features  
  - One-hot encoding for categorical features  
  - Unified pipeline using `scikit-learn`  

- **Modeling**:  
  - Linear Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor  
  - Evaluation using RMSE & Cross-Validation  

- **Stratified Sampling**:  
  - Ensures fair train-test splits based on **income categories**  

- **Deployment Ready**:  
  - Model and preprocessing pipeline saved with **Joblib**  
  - Supports both **training mode** and **inference mode**  
  - Predictions saved automatically to `output.csv`  

---

## 🚀 Workflow  
1. Load dataset (`housing.csv`)  
2. Perform **stratified train-test split**  
3. Preprocess features through pipeline  
4. Train multiple regression models  
5. Evaluate and select the best model (**Random Forest**)  
6. Save trained model and pipeline (`model.pkl`, `pipeline.pkl`)  
7. Run inference on new data (`input.csv`) → predictions in `output.csv`  

---

## 📂 Project Structure  
```
├── main.py          # Final script (training & inference)
├── main_old.py      # Experimental script (model comparison)
├── housing.csv      # Dataset (not included here)
├── model.pkl        # Saved model (created after training)
├── pipeline.pkl     # Saved preprocessing pipeline
├── input.csv        # Input data for prediction
├── output.csv       # Predicted results
```

---

## 🛠️ Installation & Usage  

1. Clone this repository and install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

2. Run **training** (if no model exists):  
   ```bash
   python main.py
   ```

3. Run **inference** on new data:  
   ```bash
   python main.py
   ```

---

## 📊 Results  
- Random Forest Regressor achieved the **lowest RMSE**, outperforming Linear Regression and Decision Tree.  
- Provides a reliable predictive model for **real estate pricing trends**.  

---

## 📜 License  
This project is open-source and free to use for educational and research purposes.  
