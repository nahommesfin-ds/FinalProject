# 🛌 The Interplay of Occupational Stress, Lifestyle Factors, and Sleep Quality
### A Data-Driven Public Health Analysis of Sleep Disorders

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**Author**: Nahom Mesfin | **Institution**: George Washington University, Milken Institute School of Public Health

---

## 📋 Project Overview

This comprehensive data science project investigates the multifaceted relationships between **lifestyle factors**, **occupational stress**, **physiological metrics**, and **sleep health outcomes**. Using advanced statistical analysis and machine learning, this research identifies the strongest predictors of sleep disorders within a working population of 374 professionals.

### 🎯 Research Questions

1. **Is there a significant difference in sleep duration** between individuals with and without sleep disorders?
2. **Is there a strong association between BMI Category and sleep disorder presence?**
3. **Which variables are the strongest predictors** of sleep disorder onset?

---

## 👨‍💼 About the Author

**Nahom Mesfin** is a dedicated **Data Scientist and Public Health Analyst** with a passion for leveraging data science to address critical health challenges in occupational and population health settings.

### 🎓 Background
- **Current Role**: Ungraduate Student in Health Data Science
- **Institution**: George Washington University, Milken Institute School of Public Health
-
### 💻 Technical Expertise
- **Programming Languages**: Python, R, SQL
- **Data Analysis**: Statistical testing (ANOVA, Chi-Square, Mann-Whitney U), Hypothesis Testing, Regression Analysis
- **Machine Learning**: Classification, Logistic Regression, ROC/AUC Analysis, Feature Engineering
- **Libraries**: pandas, scikit-learn, statsmodels, seaborn, matplotlib, NumPy, SciPy
- **Data Visualization**: Publication-quality graphics, heatmaps, diagnostic plots, interactive visualizations
- **Tools**: Jupyter Notebook, VS Code, Git, GitHub

### 🔬 Research Interests
- Occupational health and workplace wellness programs
- Sleep science, circadian rhythms, and sleep disorders
- Predictive modeling for chronic disease prevention
- Health equity and population health disparities
- Data-driven policy recommendations
---

## ✨ Key Findings

✅ **Sleep Duration is a Critical Marker**
- Individuals without sleep disorders sleep significantly longer (median difference, p < 0.05)
- Non-parametric Mann-Whitney U test confirmed strong evidence

✅ **BMI Category is Strongly Associated with Disorders**
- Statistically significant association found (χ² test, p < 0.001)
- Supports epidemiological literature on obesity and sleep apnea

✅ **Occupational Stress is a Dominant Predictor**
- Stress level emerged as the strongest lifestyle predictor of sleep quality degradation
- Consistent across multiple statistical models (OLS, Logistic Regression)

✅ **Multi-Factorial Nature of Sleep Health**
- Sleep disorders result from complex interplay of physical (BMI, heart rate, age) and psychological (stress) factors
- Logistic regression model demonstrates high predictive accuracy

---

## 📊 Dataset

**Source**: [Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset) - Kaggle Open Data

**Sample Size**: 374 working professionals  
**Design**: Cross-sectional study  

### Key Variables
| Variable | Type | Description |
|----------|------|-------------|
| Age | Continuous | Years |
| Gender | Categorical | Male/Female |
| Occupation | Categorical | Professional category |
| Sleep Duration | Continuous | Hours per day |
| Sleep Quality | Ordinal | 1-10 rating |
| Stress Level | Ordinal | 1-10 rating |
| BMI Category | Categorical | Normal/Overweight/Obese |
| Heart Rate | Continuous | BPM |
| Daily Steps | Continuous | Steps per day |
| **Sleep Disorder** | **Categorical** | **Primary Outcome** |

---

## 🛠️ Technologies & Methods

### Core Libraries
- **pandas** - Data manipulation
- **NumPy** - Numerical computing
- **SciPy** - Statistical functions
- **scikit-learn** - Machine learning models
- **statsmodels** - Advanced regression & ANOVA
- **matplotlib** & **seaborn** - Visualization

### Statistical Methods
✓ Shapiro-Wilk Test (Normality)  
✓ Levene's Test (Variance Homogeneity)  
✓ Mann-Whitney U Test (Non-parametric median comparison)  
✓ One-way ANOVA + Tukey HSD (Post-hoc analysis)  
✓ ANCOVA (Controlled comparison)  
✓ Pearson's Chi-Square (Categorical association)  
✓ Pearson & Spearman Correlation  

### Predictive Models
✓ Multiple OLS Regression (Sleep quality prediction)  
✓ Binary Logistic Regression (Disorder classification)  
✓ ROC/AUC Analysis  
✓ Feature Importance Ranking  

### Significance Level
All tests evaluated at **α = 0.05** (5% significance threshold)

---

## 📁 Project Structure

```
FinalProject/
├── README.md                               # Project documentation
├── requirements.txt                        # Python dependencies
├── FinalProject.ipynb                      # Main analysis notebook
└── .gitignore                              # Git ignore file
```

**Notebook Contents** (11 comprehensive sections):
1. Title & Project Metadata
2. Library Imports & Configuration
3. Introduction & Background
4. Methods & Study Design
5. Statistical Formulations
6. Exploratory Data Analysis (EDA)
7. Inferential Statistics & Hypothesis Tests
8. Predictive Modeling (OLS & Logistic Regression)
9. Discussion & Interpretation
10. Conclusions & Recommendations
11. References (13 peer-reviewed sources)

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- pip or conda
- Jupyter Notebook or VS Code

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/nahommesfin-ds/FinalProject.git
cd FinalProject
```

**2. Create a virtual environment (recommended)**
```bash
# Using venv
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Or using conda
conda create -n finalproject python=3.9
conda activate finalproject
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Launch Jupyter Notebook**
```bash
jupyter notebook FinalProject.ipynb
```

Or open directly in VS Code with Jupyter extension enabled.

### Data Setup

**Important**: Update the data path in the notebook to your local location:

```python
# Cell 8: Data Import
df = pd.read_csv(r'YOUR_PATH\Sleep_health_and_lifestyle_dataset.csv')
```

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset).

---

## 📖 How to Use This Notebook

1. **Run cells sequentially** starting from the top
2. **Cell 2**: Loads all visualization libraries
3. **Cell 3**: Loads statistical libraries
4. **Cell 8**: Imports and preprocesses data
5. **Cells 9-20**: Exploratory analysis and visualizations
6. **Cells 21-30**: Hypothesis testing and inferential statistics
7. **Cells 31+**: Predictive modeling and final analysis

All cells are well-commented and organized by section for easy navigation.

---

## 🔍 Key Results Summary

### Hypothesis Testing Results

| Test | Finding | P-Value |
|------|---------|---------|
| Shapiro-Wilk (Normality) | Rejected | < 0.001 |
| Levene's (Variance) | Rejected | < 0.05 |
| Mann-Whitney U | Significant | < 0.001 |
| Chi-Square (BMI × Disorder) | Significant | < 0.001 |
| ANOVA (BMI × Sleep Duration) | Significant | < 0.001 |

### Model Performance
- **Logistic Regression**: High predictive accuracy demonstrated via ROC/AUC curve
- **OLS Model**: Strong explanatory power for sleep quality
- **Feature Importance**: Stress level, age, and BMI identified as top predictors

---

## 💡 Recommendations

### For Public Health Officials
1. **Develop integrated workplace wellness programs** addressing stress reduction + weight management
2. **Target high-risk professions** (healthcare, engineering, corporate)
3. **Implement evidence-based sleep hygiene education**

### For Employers
- Prioritize **occupational stress interventions**
- Combine **nutritional support with fitness programs**
- Monitor sleep quality as health indicator in employee wellness

### For Future Research
- Conduct **longitudinal studies** to establish causality
- Examine **specific occupational categories** in depth
- Evaluate **intervention effectiveness** for sleep disorder prevention
- Explore **temporal relationships** and sleep trend patterns

---

## 📚 References

1. Medic G, et al. Short- and long-term health consequences of sleep disruption. *Nat Sci Sleep*. 2017;9:151-161.
2. Hirshkowitz M, et al. National Sleep Foundation's sleep time duration recommendations. *Sleep Health*. 2015;1(1):40-43.
3. Chattu VK, et al. The Global Problem of Insufficient Sleep and Its Serious Public Health Implications. *Healthcare (Basel)*. 2018;7(1):1.
4. Peppard PE, et al. Increased prevalence of sleep-disordered breathing in adults. *Am J Epidemiol*. 2013;177(9):1006-1014.
5. Senaratna CV, et al. Prevalence of obstructive sleep apnea in the general population. *Sleep Med Rev*. 2017;34:70-81.
6. Akerstedt T, et al. Work load and work hours in relation to disturbed sleep and fatigue. *J Psychosom Res*. 2002;53(1):585-588.
7. Linton SJ, et al. The effect of the work environment on future sleep disturbances. *Sleep Med Rev*. 2015;23:10-19.
8. Knutson KL, et al. The metabolic consequences of sleep deprivation. *Sleep Med Rev*. 2007;11(3):163-178.
9. Grandner MA, et al. Sleep: important considerations for cardiovascular disease prevention. *Curr Opin Cardiol*. 2016;31(5):551-565.
10. Chattu VK, et al. Global problem of insufficient sleep. *Healthcare (Basel)*. 2018;7(1):1.

[See full references in FinalProject.ipynb]

---

## 📊 Data Visualization Examples

This notebook includes:
- **Density histograms** with disorder status overlay
- **Violin plots** for sleep quality distribution
- **Correlation heatmaps** of numeric variables
- **Pair plots** showing multivariate relationships
- **Box plots** for group comparisons
- **Residual diagnostic plots** for model validation
- **ROC/AUC curves** for classification performance
- **Feature importance bar charts**

All visualizations are high-resolution (retina display) and publication-ready.

---

## 🔐 License

This project is licensed under the **MIT License** - feel free to use, modify, and distribute.

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software...
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to:
- Report bugs
- Suggest improvements
- Fork and submit pull requests

---

## 📧 Contact

**Nahom Mesfin**
- 🔗 **GitHub**: [nahommesfin-ds](https://github.com/nahommesfin-ds)
- 📧 **Email**: [Your email]
- 💼 **LinkedIn**: [Your LinkedIn profile]

---

## 📅 Project Timeline

- **Course**: PUBH 1142: Introduction to Health Data Science
- **Completion Date**: May 5, 2026
- **Status**: ✅ Complete & Ready for Publication

---

## 🙏 Acknowledgments

- **Data**: Kaggle Sleep Health and Lifestyle Dataset
- **Institution**: George Washington University, Milken Institute School of Public Health
- **Mentor/Instructor**: [Professor Name]
- **References**: 13 peer-reviewed academic sources

---

**Last Updated**: May 5, 2026 | **Version**: 1.0.0

---

## 📌 Next Steps

To push this project to GitHub:

```bash
# 1. Create README.md, requirements.txt, .gitignore (already done)
# 2. Initialize git repository
git init

# 3. Add all files
git add .

# 4. Create initial commit
git commit -m "Initial commit: FinalProject analysis notebook"

# 5. Add remote repository
git remote add origin https://github.com/nahommesfin-ds/FinalProject.git

# 6. Push to GitHub
git branch -M main
git push -u origin main
```

**Note**: Make sure you've created the `FinalProject` repository on GitHub first at https://github.com/new

---

**Ready to share your work! 🚀**
