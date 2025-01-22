# Telco Customer Churn Analysis 📊

## Overview
This project analyzes customer churn patterns in a telecommunications company using machine learning and data visualization techniques. The analysis aims to identify key factors contributing to customer churn and provide actionable insights for retention strategies.

## Time Investment ⏱️
**Total Time: 4 hours**
- Data preprocessing and cleaning: ~1 hour
- Visualization and analysis: ~1.5 hours
- Model building and evaluation: ~1 hour
- Documentation and reporting: ~0.5 hours

## Dataset Information 📑
- **Source**: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Records**: 7,032 customers
- **Features**: 21 predictor variables
- **Target Variable**: Customer churn (Yes/No)
- **Churn Rate**: 26.6%

## Technical Requirements 🛠️
```python
# Install required packages
!pip install fpdf matplotlib seaborn scikit-learn pandas numpy fpdf2
```

### Required Libraries
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import classification_report, confusion_matrix
from fpdf import FPDF
```

## Analysis Steps 📈

### 1. Data Preprocessing
- Converted TotalCharges to numeric format
- Handled missing values
- Created dummy variables for categorical features
- Scaled numerical features

### 2. Key Findings 🔍

#### Demographics Analysis
- **Gender Impact**: 
  - Similar churn rates across genders (26-27%)
  - No gender-specific retention strategies needed

- **Senior Citizens**: 
  - Higher churn rate among seniors
  - Represent 15% of customer base
  - Need specialized retention programs

#### Service Analysis
- **Internet Service**: 
  - Fiber optic: Highest churn (40-45%)
  - DSL: Moderate churn (20-25%)
  - No internet: Lowest churn (15%)

- **Contract Type**: 
  - Month-to-month: Highest risk (55% churn)
  - One-year: Moderate risk (15-20% churn)
  - Two-year: Lowest risk (10% churn)

#### Financial Analysis
- Higher monthly charges correlate with increased churn
- Median charges:
  - Churned customers: ~$80
  - Retained customers: ~$65

### 3. Model Performance 🎯
```python
Classification Report:
              precision    recall  f1-score   support
           0      0.82      0.89      0.85     1033
           1      0.59      0.44      0.51      374
    accuracy                          0.77     1407
   macro avg      0.70      0.67      0.68     1407
weighted avg      0.76      0.77      0.76     1407
```

## Recommendations 💡

### Immediate Actions
1. **Service Quality**
   - Improve fiber optic reliability
   - Create senior citizen packages
   - Implement early-warning system
   - Develop first-year engagement program

2. **Pricing Strategy**
   - Review high-charge segments
   - Implement tiered pricing
   - Create loyalty discounts

3. **Service Enhancement**
   - Strengthen technical support
   - Regular quality assessments
   - Proactive customer outreach

## Future Work 🚀

### Advanced Analytics
- Real-time churn prediction system
- Customer lifetime value analysis
- Automated reporting system

### Data Collection Needs
- Customer satisfaction metrics
- Service quality indicators
- Competitor pricing information

## Output Files 📁
**TelcoChurnAnalysis.pdf**
   - Comprehensive analysis report
   - Visual insights
   - Detailed recommendations


## Business Impact 💼
- Potential reduction in customer churn
- Improved customer satisfaction
- Enhanced revenue retention
- Better resource allocation for retention efforts
