# 📄 Telco Customer Churn Prediction

This project focuses on customer churn analysis using segmentation based on key variables from a telecom dataset.

## 📊 Variable Transformation

### 1. Re-Categorization
- **SeniorCitizen**:
  - `0` → `"J"` (Junior)
  - `1` → `"S"` (Senior)

- **Tenure** (customer tenure in months):
  - `0–6 months` → `"0-6"`
  - `7–16 months` → `"7-16"`
  - `17+ months` → `"17+"`

- **Contract**:
  - `"Month-to-month"` → `"MM"`
  - `"One year"` → `"OY"`
  - `"Two year"` → `"TY"`

### 2. Technological Products Variable
A new column named **"Technological Urunler"** was created.  
If a customer has at least one of the following services, they are marked as `"kullaniyor"` (using technology), otherwise `"kullanmiyor"` (not using):
- `OnlineSecurity`
- `OnlineBackup`
- `DeviceProtection`
- `TechSupport`

## 🎯 Segment Creation
Segments were created using the following variables:
- `SeniorCitizen`
- `Tenure`
- `Contract`
- `Technological Urunler`

## 📉 Churn Rate Calculation
Churn rates were calculated for each segment to analyze patterns and trends.

## 🛠️ Tools Used
- Python (Pandas)
- Jupyter Notebook

