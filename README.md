# logistics-delivery-time-prediction_linear_regression
A predictive analytics tool designed for logistics operations to estimate package delivery times based on item sorting duration.

# Logistics Delivery Time Prediction Model

## 1. Business Problem
### 1.1. What is the business objective?
To accurately estimate total delivery time using sorting duration metrics, optimizing warehouse dispatch schedules and improving last-mile delivery efficiency.
### 1.2. Are there any constraints?
* External variables like traffic congestion and weather conditions are not captured in sorting metrics.
* Predictions apply strictly to standard regional dispatch routes.

## 2. Data Dictionary
| Feature Name | Data Type | Relevance | Description / Reason if Not Relevant |
| :--- | :--- | :--- | :--- |
| `Sorting Time` | Continuous (Float) | High (Predictor) | Time taken in minutes to sort items prior to dispatch. |
| `Delivery Time` | Continuous (Float) | High (Target Variable) | Total time taken in minutes from dispatch to final delivery. |

## 3. Data Pre-processing
* **3.1. Data Cleaning & Feature Engineering:** Verified dataset completeness, checked for timestamp consistency, and structured numerical types.
* **3.2. Outlier Treatment:** Inspected delivery delays caused by anomalies and managed outliers to stabilize variance.

## 4. Exploratory Data Analysis (EDA)
* **4.1. Summary:** Generated descriptive statistics for sorting and delivery intervals.
* **4.2. Univariate Analysis:** Explored distribution spreads of delivery times and sorting durations.
* **4.3. Bivariate Analysis:** Plotted scatter matrices to evaluate the direct correlation strength between sorting time and transit duration.

## 5. Model Building
* **5.1. Simple Linear Regression:** Established baseline performance evaluating sorting time against delivery time.
* **5.2. Transformations:** Tested logarithmic, square root, and polynomial transformations; logged comparative RMSE, R-Squared, and correlation metrics.
* **5.3. Model Selection:** Chipped away errors to select the optimal transformation model.
* **5.4. Documentation:** Detailed model equations and residual distribution plots.

## 6. Business Impact / Benefits
Streamlines supply chain management, reduces fulfillment bottlenecks, enhances dispatch planning, and improves customer satisfaction through reliable delivery time estimates.
