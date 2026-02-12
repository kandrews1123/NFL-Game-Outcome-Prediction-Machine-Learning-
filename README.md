# NFL-Game-Outcome-Prediction-Machine-Learning-

## 📌 Objective

The primary objective of this project is to **predict NFL game outcomes** by determining the winner between the **home team (X)** and the **away team (Y)**.

The models leverage **historical game data, weekly player statistics, and team-level metrics** to improve prediction accuracy and identify the key factors that influence win probability.

---

## 💡 Motivation

Predicting NFL game outcomes has significant value for:

* Sports analytics professionals
* Fantasy football managers
* Bettors and sportsbooks
* NFL teams and coaching staff

By combining advanced machine learning techniques with detailed performance data, this project provides insights into **which factors most strongly drive winning outcomes**.

---

## 📊 Data

The dataset includes:

* Weekly NFL team statistics
* Player-level performance metrics
* Advanced analytics such as Expected Points Added (EPA)
* Historical game results

Feature engineering was applied to transform raw statistics into predictive inputs suitable for classification models.

---

## 🧠 Modeling Approach

To evaluate both linear and nonlinear modeling strategies, three classification models were implemented and compared:

### 🔹 XGBoost (Nonlinear Model)

* Captures complex feature interactions
* Achieved **81% accuracy**
* Best-performing model

### 🔹 Logistic Regression (Linear Model)

* Baseline classification model
* Lower performance compared to XGBoost

### 🔹 LASSO (L1-Regularized Logistic Regression)

* Used for feature selection and sparsity
* Did not perform well relative to nonlinear methods

---

## 🛠 Feature Engineering & Model Comparison

* Engineered features from weekly team and player statistics
* Compared linear vs. nonlinear approaches
* Evaluated feature importance to understand win drivers
* Assessed model bias and predictive limitations

The comparison highlights how **nonlinear relationships play a significant role in NFL game outcomes**.

---

## 🔍 Key Findings

### ✅ Model Performance

* **XGBoost achieved the highest accuracy (81%)**
* Logistic Regression and LASSO underperformed
* The dataset appears better suited for nonlinear modeling techniques

### 📈 Important Features

* **Score** was the most important feature in the XGBoost model, which is expected since the final score determines the winner.
* Logistic and LASSO models did not use score as a predictor, which likely introduced bias and contributed to weaker performance.
* **Receiving EPA (Expected Points Added)** ranked in the top three most important variables across all models.

### 🏈 Insight on Receiving EPA

Receiving EPA measures how well a team performs relative to expectations on a play-by-play basis through its receivers.

This reinforces an important football insight:

> Strong receiver performance — such as explosive plays, high yardage gains, and touchdowns — significantly increases the probability of winning.

---

## 🚀 Applications

This framework can be extended to:

* Real-time win probability modeling
* Betting and sportsbook analytics
* Fantasy matchup projections
* Team strategy and opponent analysis
* Automated prediction dashboards

---

## 📌 Conclusion

The results demonstrate that **nonlinear machine learning models (XGBoost) outperform traditional linear methods** for NFL outcome prediction.

Game outcomes are influenced by complex feature interactions that linear models struggle to capture. Advanced metrics such as **Receiving EPA** provide strong predictive signals and reinforce the importance of offensive efficiency in determining wins.

---

