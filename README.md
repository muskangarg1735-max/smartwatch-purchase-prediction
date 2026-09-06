# ⌚ Smartwatch Purchase Prediction | 87% Accuracy | 9,831 Customers

> Built ML model to predict smartwatch buyers to optimize marketing ROI.

## 📊 Dataset
- 9,831 customers, 42 features
- Target: WatchbuyInd (21.5% Buyers - Imbalanced)
- Features: Affluence, Age, Loyalty, Visits, Promos, Surveys Q1-Q10, Feedback, Product Categories

## 🔥 What I Did (Advanced)
- Fixed data leaks in CustAfflGrade, CustCluster
- Created 6 new features: Visit Velocity, Promo Velocity, Spend_Per_Tenure, Survey_Sum/Min/Max
- Handled imbalance with class_weight='balanced' + HistGradientBoosting
- Used 200 trees, max_depth=8, L2 regularization

## 🛠️ Tech Stack
Python, Pandas, Scikit-Learn, HistGradientBoosting, SMOTE, LabelEncoder

## 🏆 Results
- Accuracy: 87.06%
- Confusion Matrix: [[1793, 138], [180, 347]]
- Precision: 91% Non-Buyers, 72% Buyers
- Top Features: CustSpend, LoyalTenure, Prom12MCnt, Income, Visits

## 💡 Business Impact
Target only 21% high-potential customers = 3x better marketing ROI

## 🚀 How to Run
pip install pandas scikit-learn openpyxl imbalanced-learn
jupyter notebook SmartWatches.ipynb
