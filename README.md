# Brain Stroke Data Analysis Project

## Introduction
This project focuses on an exploratory analysis of a brain stroke dataset, sourced from Kaggle. With more than 2000 entries spanning across 11 columns, this comprehensive dataset sheds light on an array of factors presumed to influence the occurrence of strokes. The key concern is the 'strokes' column, which serves as our target variable. In the context of logistic regression (the model used within this project), the target variable is binary - 1 representing a positive result for a stroke and 0, a negative result. 

The objective is to identify the intricate relationships between the occurrence of strokes and a series of predictor variables - gender, age, hypertension, heart disease, and smoking status. 

## Questions Under Investigation:
1. Does gender play a significant role in stroke occurrence and if so, which gender demonstrates a higher stroke frequency?
2. And more insightful questions dealing with the various predictor variables.

## Data Wrangling

The original dataset incorporates columns such as gender, age, heart_disease, ever_married, work_type, Residence_type, avg_glucose_level, and bmi smoking_status. 

## Data Loading
```python
stroke_df =pd.read_csv( '/content/brain_stroke.csv ')
```

## Analysis

**Confusion Matrix**

A confusion matrix was generated to discern how well the model fares in making predictions. It indicated a relatively high false positive rate (30%) and a true negative rate (70%). If the treatment's side effects were severe, this could develop into an issue. 

However, the side effects of stroke medication, as identified from several sources, include mild symptoms like diarrhoea, indigestion, nausea, and stomach pain. 

The high false positive rate might raise issues if other ailments' symptoms imitated strokes. We note that a low precision could be problematic, especially in cases where diseases mimicking strokes are common. 

The true positive rate for our model stands at around 82%.

Please note this analysis was carried out without medical expertise, and results should not be used for clinical decision making.

**Project Completion Date**: May 16, 2023.

*Please refer to interactive Python Jupyter notebooks for the complete analysis.* 
