# Elevated-Lab-Internship-Task5
Exploratory Data Analysis. Extract insights using visual and statistical exploration.

# 🚢 Titanic Dataset - Comprehensive Exploratory Data Analysis
> **A data analyst approach to understanding survival patterns in the Titanic disaster through comprehensive statistical analysis and visualization.**

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [🔍 Key Findings](#-key-findings)
- [📊 Dataset Information](#-dataset-information)
- [🛠️ Installation & Setup](#️-installation--setup)
- [📁 Project Structure](#-project-structure)
- [🚀 Usage](#-usage)
- [📈 Analysis Steps](#-analysis-steps)
- [📊 Visualizations](#-visualizations)
- [🎯 Machine Learning Insights](#-machine-learning-insights)
- [📄 Reports](#-reports)
- [🤝 Contributing](#-contributing)
- [📧 Contact](#-contact)

## 🎯 Project Overview

This project provides a **comprehensive exploratory data analysis** of the famous Titanic dataset, focusing on understanding the factors that influenced passenger survival during the 1912 disaster. Using advanced statistical techniques and data visualization, we uncover patterns that align with historical accounts while providing actionable insights for predictive modeling.

### 🌟 **Why This Analysis Matters**
- **Historical Validation**: Statistical patterns confirm documented historical events
- **Data Science Learning**: Demonstrates best practices for EDA methodology  
- **Feature Engineering**: Provides insights for machine learning model development
- **Business Intelligence**: Offers actionable recommendations based on data-driven insights

## 🔍 Key Findings

### 🎯 **Critical Survival Insights**
| Factor | Finding | Statistical Significance |
|--------|---------|-------------------------|
| **Overall Survival** | 38.4% survival rate | - |
| **Gender Impact** | Women: 74.2% vs Men: 18.9% | p < 0.001 ⭐⭐⭐ |
| **Class Hierarchy** | 1st: 62.9% → 2nd: 47.3% → 3rd: 24.2% | p < 0.001 ⭐⭐⭐ |
| **Age Factor** | Children < 18 had significantly higher rates | p < 0.001 ⭐⭐⭐ |
| **Family Size** | Optimal: 2-4 members (50-70% survival) | p < 0.05 ⭐ |

### 📊 **Advanced Insights**
- **1st Class Women**: 96.8% survival rate (nearly perfect)
- **3rd Class Men**: 13.5% survival rate (lowest group)
- **Family Dynamics**: Solo travelers had ~30% survival vs 50%+ for small families
- **Title Analysis**: "Master" (boys) had 57.5% survival showing child priority

## 📊 Dataset Information

**Source**: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)  
**Size**: 891 passengers × 12 features  
**Target Variable**: Survived (0 = No, 1 = Yes)

### 📋 **Features Overview**
| Feature | Type | Description | Missing % |
|---------|------|-------------|-----------|
| `PassengerId` | Integer | Unique passenger identifier | 0% |
| `Survived` | Integer | Survival (0 = No, 1 = Yes) | 0% |
| `Pclass` | Integer | Ticket class (1, 2, 3) | 0% |
| `Name` | String | Passenger name | 0% |
| `Sex` | String | Gender (male, female) | 0% |
| `Age` | Float | Age in years | 19.9% ⚠️ |
| `SibSp` | Integer | # siblings/spouses aboard | 0% |
| `Parch` | Integer | # parents/children aboard | 0% |
| `Ticket` | String | Ticket number | 0% |
| `Fare` | Float | Passenger fare | 0% |
| `Cabin` | String | Cabin number | 77.1% ❌ |
| `Embarked` | String | Port of embarkation | 0.2% |

## 🛠️ Installation & Setup

### **Prerequisites**
```bash
Python 3.7+
Jupyter Notebook
```

### **Clone Repository**
```bash
git clone https://github.com/yourusername/titanic-eda-analysis.git
cd titanic-eda-analysis
```

### **Install Dependencies**
```bash
pip install -r requirements.txt
```

### **Required Libraries**
```python
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scipy>=1.7.0
jupyter>=1.0.0
```

## 📁 Project Structure

```
titanic-eda-analysis/
│
├── 📊 data/
│   ├── train.csv                 # Training dataset
│   └── test.csv                  # Test dataset (optional)
│
├── 📓 notebooks/
│   ├── 01_data_exploration.ipynb          # Initial data exploration
│   ├── 02_comprehensive_eda.ipynb         # Full EDA analysis
│   └── 03_feature_engineering.ipynb      # Feature engineering insights
│
├── 📜 scripts/
│   ├── eda_analysis.py           # Complete EDA script
│   └── generate_pdf_report.py    # PDF report generator
│
├── 📈 visualizations/
│   ├── survival_analysis.png     # Key survival charts
│   ├── demographic_analysis.png  # Age, gender, class charts  
│   └── correlation_heatmap.png   # Feature correlations
│
├── 📄 reports/
│   ├── Titanic_EDA_Report.pdf    # Comprehensive PDF report
│   └── executive_summary.md      # Executive summary
│
├── 🔧 utils/
│   └── helper_functions.py       # Utility functions
│
├── 📋 requirements.txt           # Dependencies
├── 📖 README.md                 # This file
└── ⚖️ LICENSE                   # MIT License
```

## 🚀 Usage

### **Option 1: Jupyter Notebook (Recommended)**
```bash
# Start Jupyter Notebook
jupyter notebook

# Open notebooks/02_comprehensive_eda.ipynb
# Run all cells to reproduce analysis
```

### **Option 2: Python Script**
```bash
# Run complete EDA analysis
python scripts/eda_analysis.py

# Generate PDF report
python scripts/generate_pdf_report.py
```

### **Option 3: Interactive Analysis**
```python
import pandas as pd
from scripts.eda_analysis import TitanicEDA

# Load data and run analysis
analyzer = TitanicEDA('data/train.csv')
analyzer.run_complete_analysis()
analyzer.generate_insights()
```

## 📈 Analysis Steps

### **🔍 Phase 1: Data Understanding**
- [x] Dataset structure and feature types
- [x] Data quality assessment  
- [x] Missing value patterns
- [x] Basic statistical summaries

### **📊 Phase 2: Univariate Analysis**
- [x] Target variable distribution
- [x] Feature distributions
- [x] Outlier detection
- [x] Data type optimization

### **🔗 Phase 3: Bivariate Analysis**  
- [x] Survival rates by key features
- [x] Statistical significance testing
- [x] Correlation analysis
- [x] Cross-tabulation insights

### **🎯 Phase 4: Multivariate Analysis**
- [x] Feature interactions
- [x] Advanced segmentation
- [x] Multi-dimensional patterns
- [x] Complex relationships

### **🔧 Phase 5: Feature Engineering**
- [x] Title extraction from names
- [x] Family size categorization  
- [x] Age group creation
- [x] Deck information extraction

## 📊 Visualizations

<div align="center">

### **Survival Overview**
![Survival Analysis](visualizations/survival_overview.png)

### **Demographic Patterns** 
![Demographics](visualizations/demographics.png)

### **Feature Correlations**
![Correlations](visualizations/correlation_matrix.png)

</div>

### **📈 Key Visualizations Include:**
- Survival distribution (overall and by segments)
- Age and gender demographic analysis
- Passenger class impact visualization
- Family size survival patterns
- Embarkation port analysis  
- Feature correlation heatmap
- Multi-dimensional interaction plots

## 🎯 Machine Learning Insights

### **🔧 Feature Engineering Recommendations**

#### **Primary Features**
```python
primary_features = [
    'Sex',           # Strongest predictor
    'Pclass',        # Clear hierarchy  
    'Age',           # After imputation
    'Fare',          # Socioeconomic proxy
    'FamilySize'     # Engineered feature
]
```

#### **Engineered Features**
```python
# Title categories
titles = {
    'Mr': 'Mr',
    'Miss': 'Miss', 
    'Mrs': 'Mrs',
    'Master': 'Master',
    'Other': ['Dr', 'Rev', 'Col', ...]
}

# Age groups  
age_groups = {
    'Child': 0-17,
    'Adult': 18-64, 
    'Senior': 65+
}

# Family categories
family_cats = {
    'Alone': 1,
    'Small': 2-4,
    'Large': 5+
}
```

### **⚖️ Modeling Considerations**

#### **Class Imbalance Handling**
- **Challenge**: 61% died vs 39% survived
- **Solutions**: SMOTE, class weights, stratified sampling
- **Metrics**: Focus on precision, recall, F1-score, AUC-ROC

#### **Recommended Models**
1. **Random Forest** - Handles interactions well
2. **Gradient Boosting** - High performance 
3. **Logistic Regression** - Interpretable baseline
4. **Ensemble Methods** - Combine multiple approaches

#### **Validation Strategy**
```python
# Stratified K-Fold cross-validation
from sklearn.model_selection import StratifiedKFold
skf = StratifiedKFold(n_splits=5, shuffle=True, random_state=42)
```

### **🎯 Report Highlights**
- Statistical significance testing results
- Business insights and historical validation
- Machine learning recommendations
- Data quality assessment
- Feature engineering strategies

## 🔬 Statistical Analysis

### **Hypothesis Testing Results**
| Test | Feature | P-Value | Result |
|------|---------|---------|---------|
| Chi-square | Gender × Survival | < 0.001 | ✅ Highly Significant |
| Chi-square | Class × Survival | < 0.001 | ✅ Highly Significant |  
| T-test | Age difference | < 0.001 | ✅ Significant |
| T-test | Fare difference | < 0.001 | ✅ Significant |

### **Effect Sizes**
- **Gender**: Very large effect (Cramér's V = 0.54)
- **Passenger Class**: Large effect (Cramér's V = 0.34)
- **Age**: Medium effect (Cohen's d = 0.31) 
- **Fare**: Medium effect (Cohen's d = 0.47)

## 🏆 Key Achievements

- ✅ **100% reproducible analysis** with documented methodology
- ✅ **Statistical validation** of all major findings  
- ✅ **Historical accuracy** confirmed through domain research
- ✅ **Business-ready insights** with actionable recommendations
- ✅ **Production-ready code** with proper documentation
- ✅ **Multiple output formats** (Jupyter, PDF, HTML)

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### **🔍 Areas for Contribution**
- Additional feature engineering techniques
- Advanced visualization methods  
- Model implementation and comparison
- Documentation improvements
- Code optimization

## 📧 Contact

**Aakash Rajivale** - [@rajivaleaakash](https://github.com/rajivaleaakash) - your.email@example.com

