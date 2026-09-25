# NYC Taxi Machine Learning Analysis

An end-to-end machine learning project analysing New York City taxi trip data to generate actionable business insights while considering the responsible use of predictive models.

This project was completed as part of the **Google Advanced Data Analytics Professional Certificate** and demonstrates the full analytical workflow, from exploratory data analysis and feature engineering to model development, evaluation and stakeholder recommendations.

## Project Overview

The project uses NYC taxi trip data to investigate fare and tipping behaviour through statistical analysis and machine learning.

The analysis had two main modelling components:

1. **Fare analysis** – examined the factors influencing taxi fares and developed a regression model to estimate fare amounts.
2. **Tipping classification** – compared Random Forest and XGBoost models to identify trips associated with generous tipping behaviour.

A key part of the project was considering not only model performance, but also **how predictions should be used responsibly in a real business setting**.

## Business Problem

Automatidata was asked to use taxi trip data to support decision-making for the New York City Taxi & Limousine Commission.

The original classification task involved predicting whether a customer would be a generous tipper. However, a model of this kind could create unintended consequences if drivers used predictions to avoid passengers expected to leave smaller tips.

I therefore approached the problem from a responsible-AI perspective: predictions should support aggregate analysis, operational planning and controlled experimentation rather than decisions that could unfairly disadvantage individual passengers.

## Data

The modelling dataset contained approximately **15,000 taxi trips** after data preparation.

The workflow included:

- Data cleaning and validation
- Exploratory data analysis
- Feature engineering
- Train/test splitting
- Model training and hyperparameter tuning
- Model comparison and evaluation
- Interpretation of results
- Translation of findings into business recommendations

## Tools & Technologies

- **Python**
- **pandas**
- **NumPy**
- **scikit-learn**
- **XGBoost**
- **Matplotlib**
- **Jupyter Notebook**
- **GridSearchCV**

## Machine Learning Models

### Regression

Regression analysis was used to investigate the relationship between trip characteristics and taxi fares.

The linear regression model achieved an **R² of approximately 0.87**, indicating that the selected trip characteristics explained a substantial proportion of variation in fare amounts.

### Tipping Classification

Two tree-based machine learning models were compared:

- Random Forest
- XGBoost

The models were evaluated using metrics including:

- Precision
- Recall
- F1 score
- Accuracy

The tuned Random Forest achieved approximately:

| Metric | Test Performance |
|---|---:|
| F1 Score | 0.745 |
| Recall | 0.824 |
| Precision | 0.680 |

XGBoost produced broadly similar performance, suggesting that additional model complexity did not create a meaningful improvement for this dataset.

## Key Findings

- Trip characteristics contained useful information for explaining taxi fares and tipping behaviour.
- The regression model explained approximately **87% of the variation in fare amounts**.
- Random Forest achieved strong recall in identifying generous tipping cases.
- XGBoost did not materially outperform Random Forest.
- Model performance alone should not determine deployment: the way predictions affect customers and drivers also needs to be considered.

## Responsible AI Consideration

One of the most important conclusions from the project was that a technically successful model is not automatically a suitable business solution.

Using predicted tipping behaviour to influence which passengers drivers accept could create unfair treatment and reinforce behavioural biases.

A safer approach would be to use the analysis for:

- Understanding tipping patterns at an aggregate level
- Identifying operational trends
- Supporting business planning
- Designing controlled experiments
- Generating insights without restricting customer access to services

This reframing demonstrates the importance of combining **machine learning performance with business judgement and responsible AI principles**.

## Recommendations

1. **Use predictive insights as decision support rather than automated decision-making.**
2. **Prioritise interpretable business insights alongside model accuracy.**
3. **Test predictive applications through controlled pilots before wider deployment.**
4. **Monitor model performance and potential unintended customer impacts over time.**
5. **Collect additional relevant data before using the model for operational decisions.**

## Skills Demonstrated

This project demonstrates:

- End-to-end data analysis
- Exploratory data analysis
- Feature engineering
- Regression modelling
- Classification
- Random Forest
- XGBoost
- Hyperparameter tuning
- Model evaluation
- Responsible AI
- Translating technical analysis into business recommendations

## Repository Contents

- `Activity_Course_6_Automatidata_project_lab.ipynb` – complete analysis and modelling workflow
- `Automatidata_Executive_Summary.docx` – executive summary of findings
- `Automatidata_Findings_Recommendations.pptx` – stakeholder presentation
- `README.md` – project overview and documentation

## About

**Eric Li**  
MSc Mathematical Finance | Data Analytics | Machine Learning | Financial & Risk Analytics

This project forms part of my data science and analytics portfolio.
