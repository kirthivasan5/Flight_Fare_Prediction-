## 🛫 Flight Fare Prediction – Step-by-Step Overview

### 📌 Objective
Build a machine learning model to predict flight ticket prices based on historical data, helping travelers make cost-effective decisions.

---

## 🔍 Step-by-Step Process

### **Step 1: Problem Understanding**
- Flight fares fluctuate due to multiple factors like airline, route, stops, and timing.
- Goal: Predict future ticket prices using past data to assist in travel planning.

---

### **Step 2: Data Collection**
- Dataset includes 10+ features such as:
  - `Airline`, `Source`, `Destination`
  - `Date_of_Journey`, `Dep_Time`, `Arrival_Time`
  - `Duration`, `Total_Stops`, `Additional_Info`
  - Target variable: `Price`

---

### **Step 3: Data Preprocessing**
- **Missing Values**: Dropped minimal nulls in `Route` and `Total_Stops`.
- **Date Parsing**: Converted `Date_of_Journey` to `YYYY-MM-DD` format.
- **Duration Conversion**: Transformed `"2h 50m"` into total minutes.
- **Categorical Encoding**: Applied Label Encoding to convert text features into numeric format.

---

### **Step 4: Exploratory Data Analysis (EDA)**
- Used **Seaborn** and **Matplotlib** to visualize:
  - Price trends across airlines and routes
  - Impact of stops and duration on fare
  - Seasonal and time-based fare variations

---

### **Step 5: Model Building**
- Applied multiple regression models:
  - Linear Regression
  - Support Vector Machine
  - K-Nearest Neighbors
  - Decision Tree
  - **Random Forest**
  - **XGBoost**
  - **Gradient Boosting**

---

### **Step 6: Model Evaluation**
- Metrics used: **R² Score**, **MAE**, **RMSE**
- Top performers:
  - Random Forest: R² = 0.89
  - XGBoost: R² = 0.89
  - Gradient Boosting: R² = 0.89

---

### **Step 7: Conclusion**
- Achieved high accuracy in predicting flight fares.
- Demonstrated how ML can optimize pricing strategies in the travel industry.
- Gained hands-on experience in data wrangling, feature engineering, and model tuning.
