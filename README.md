# ✈️ Flight Delay Analysis & Prediction

A comprehensive machine learning project focused on analyzing and predicting flight delays using historical airline and airport data. This project was developed as part of the  **SocBiz Project (IITR)**.
---

## 🎯 Objective

To leverage data science techniques to:
- Identify patterns and causes behind flight delays
- Predict whether a flight will be delayed (classification)
- Predict the expected delay in minutes (regression)
- Provide actionable strategies for delay mitigation

---

## 📊 Project Workflow

### 🧪 1. Exploratory Data Analysis (EDA)
- **Monthly Delay Trends**: Analyzing how delays vary over time
- **Top Airlines & Airports**: Identifying those with the highest delay rates
- **Seasonality**: Measuring seasonal impact on delay patterns
- **Delay Cause Analysis**: Investigating delays due to weather, carrier, security, NAS, etc.
- **Correlation Heatmap & Distributions**: Understanding feature relationships

---

### 🛠️ 2. Feature Engineering
- `delay_rate`: % of flights delayed
- `avg_delay`: average delay per flight
- `carrier_prop`, `weather_prop`: delay contribution by type
- `carrier_his`, `airport_his`: historical delay data
- Categorical encoding for airlines and airports

---

### 🤖 3. Modeling

#### 🟢 Classification: Will a flight be delayed?
- **Model Used**: Random Forest Classifier
- **Technique**: SMOTE used to balance classes before training
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1 Score

#### 🔵 Regression: Predict how long the delay will be
- **Model 1**: Linear Regression  
  - MAE: 7.20  
  - MSE: 236.01

- **Model 2**: XGBoost Regression ✅  
  - MAE: 67.65 minutes  
  - RMSE: 91.80 minutes  
  - R² Score: 0.71

---

## 💼 Actionable Recommendations

1. **Improve Ground Operations**  
   Focus on late aircraft and carrier-related delays via tighter turnaround and buffer scheduling.

2. **Schedule Optimization**  
   Reallocate flights away from peak congestions and high-delay airports based on seasonal trends.

3. **Carrier & Airport Accountability**  
   Use historical metrics to flag underperformers and implement corrective initiatives.

4. **Real-time Communication**  
   Enhance passenger experience with alerts and digital rebooking during weather/NAS delays.

5. **Dynamic Resource Allocation**  
   Adjust staff and gate assignments during peak seasons using predictive insights.

---

## 🧾 Files Included

- `airlines.ipynb`: Full Python notebook with code and analysis
- `socbiz_project_deck.pdf`: Final project presentation
- `Airline_Delay_Cause.csv`: Training dataset
- `Download_column_definition`: Definition for the columns in the dataset


