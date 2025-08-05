# Superstore Customer Response Prediction

This project analyzes customer data from a superstore to predict whether a customer will respond to a marketing campaign.  
It includes extensive data preprocessing, exploratory data analysis (EDA), feature engineering, and predictive modeling using logistic regression and random forest.

## 📊 Project Overview
We work with a dataset containing demographic, purchase history, and campaign response variables. The goal is to identify key factors that influence a customer’s likelihood to respond.

## 🔍 Key Steps
1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Removed outliers
   - Converted skewed numerical variables to categorical bins
   - Created new features (e.g., `Age`, `Total_Spent`, `customer_tenure_months`)
   - Recoded categorical variables for clarity

2. **Exploratory Data Analysis (EDA)**
   - Histograms for numerical variables
   - Stacked bar charts for categorical features vs. campaign response
   - Boxplots for numerical features by response
   - Correlation analysis

3. **Feature Selection**
   - Random Forest importance ranking
   - Stepwise model refinement

4. **Modeling**
   - Logistic Regression (with and without interaction terms)
   - Random Forest for feature importance
   - ROC curve analysis and threshold selection
   - Cross-validation for performance estimation

5. **Evaluation**
   - Accuracy, Sensitivity, Specificity
   - ROC-AUC comparison between models
   - Confusion matrix analysis

## 📈 Results
- Best-performing model: Logistic Regression with interaction between `customer_tenure_months` and `Order_Recency`
- ROC-AUC: ~0.778
- Slight performance improvement with interaction term, but simpler model has similar accuracy

## 📂 Files
- `superstore_data.csv` – Input dataset (not included in repo)
- `analysis.Rmd` – R Markdown file containing all analysis and visualizations
- `CodeBook` – Data Dictionary
- `Superstore_Customer_Prediction_Slide.pptx` - Presentation Slides

## 🛠 Technologies Used
- **R** (tidyverse, caret, randomForest, e1071, gbm, sjPlot, corrplot, ROCR)
- **R Markdown** for documentation

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/superstore-customer-response-prediction.git
