# **ESG Risk Analysis: Insights from S&P 500 Companies**

This repository provides an in-depth analysis of Environmental, Social, and Governance (ESG) risk for companies listed in the S&P 500. The project utilizes machine learning to predict future ESG risk scores, helping investors and stakeholders assess sustainability and governance factors. Through sector-wise analysis and predictive modeling, this repository offers a comprehensive approach to ESG risk evaluation.

## **Table of Contents**
- [Introduction](#introduction)
- [Dataset Overview](#dataset-overview)
- [Analysis](#analysis)
  - [Sector-wise ESG Risk Analysis](#sector-wise-esg-risk-analysis)
  - [Top Performers by ESG Risk Level](#top-performers-by-esg-risk-level)
  - [Predictive Analysis](#predictive-analysis)
- [Model Construction](#model-construction)
  - [Features and Approach](#features-and-approach)
  - [Outlier Detection and Model Refinement](#outlier-detection-and-model-refinement)
- [Evaluation](#evaluation)
  - [Accuracy](#accuracy)
  - [Testing Number of Estimators](#testing-number-of-estimators)
- [Conclusion](#conclusion)
- [Usage](#usage)
- [Sources](#sources)

## **Introduction**

In an era where sustainability is paramount, ESG risk analysis offers a vital tool for evaluating companies’ environmental, social, and governance practices. This project focuses on analyzing the ESG risk profiles of S&P 500 companies, offering insights for investors and decision-makers. The dataset includes key ESG parameters, and the project employs machine learning models to predict future ESG risk scores.

## **Dataset Overview**

The dataset features ESG risk scores for S&P 500 companies, with the following key metrics:
- **Environmental Risk Score**: Reflects the company’s ecological impact and practices.
- **Social Risk Score**: Measures the company’s societal contributions and community impact.
- **Governance Risk Score**: Assesses corporate governance practices and ethics.
- **Controversy Level & Score**: Tracks public controversies and their intensity.
- **Total ESG Risk Score**: A comprehensive score combining all ESG factors.

## **Analysis**

### **Sector-wise ESG Risk Analysis**
The analysis highlights ESG risk levels across different sectors:
- **High ESG Risk**: The **Energy** and **Utilities** sectors face significant environmental and social risks.
- **Low ESG Risk**: **Real Estate** and **Technology** sectors have the lowest ESG risk exposure.

### **Top Performers by ESG Risk Level**
Some companies, like **Pentair Plc** and **Costar Group Inc**, have balanced ESG profiles, with scores close to the sector mean. These companies are considered good examples of effective ESG risk management.

## **Predictive Analysis**

### **Model Objective and Overview**
The predictive model is designed to estimate a company’s future ESG risk score based on historical data. Key features include:
- **Sector**
- **Industry**
- **Employee count**
- **Environmental, Social, and Governance Risk Scores**

### **Model Construction**
A **Random Forest Classifier** is employed for prediction, with the model’s performance initially impacted by outliers and data leakage. After removing problematic features (like "ESG Risk Percentile"), the model is retrained, resulting in more balanced predictions.

### **Outlier Detection and Model Refinement**
Outliers were identified and removed to enhance model accuracy. The final model demonstrated a reasonable accuracy of **87.2%**, with the **Environment Risk Score** being the most influential predictor.

## **Evaluation**

### **Accuracy**
The model achieved an accuracy of **87.2%** using the **Random Forest Classifier**. This level of accuracy suggests good predictive potential but also indicates room for further refinement.

### **Testing Number of Estimators**
Adjusting the "n_estimators" parameter showed an improvement in accuracy, though the law of diminishing returns applies after a certain point. Optimizing this parameter strikes a balance between accuracy and efficiency.

## **Conclusion**

ESG risk analysis is crucial for understanding a company's sustainability and governance practices. This project empowers investors to make informed decisions by analyzing ESG risk scores and predicting future trends. By integrating ESG factors into decision-making, businesses can foster sustainable growth and responsible practices.

## **Usage**

To use this analysis and model, clone this repository and follow the instructions in the installation section. The machine learning model can be customized for different datasets to predict ESG risk scores for other companies or sectors.

## **Sources**

1. "The Business Case for ESG" by Harvard Business Review. [Link](https://hbr.org/2019/05/the-business-case-for-esg)
2. "Environmental, Social and Governance (ESG) Criteria" by Investopedia. [Link](https://www.investopedia.com/terms/e/environmental-social-and-governance-esg-criteria.asp)
3. "Why ESG Matters: The Sustainable Investor's Guide" by BlackRock. [Link](https://www.blackrock.com/us/individual/education/understanding-esg-investing)
4. "ESG Ratings: An Overview" by MSCI. [Link](https://www.msci.com/our-solutions/esg-investing/esg-ratings)
5. "ESG and Corporate Financial Performance: Mapping the Landscape" by Journal of Applied Corporate Finance. Authors: Mozaffar Khan, George Serafeim, and Aaron Yoon. [Link](https://onlinelibrary.wiley.com/doi/full/10.1111/jacf.12221)
6. "ESG Risk and Financial Performance: The Long View" by Morgan Stanley. [Link](https://www.morganstanley.com/ideas/esg-sustainable-investing-performance)
7. "A Primer on Environmental, Social, and Governance (ESG) Metrics" by The World Bank. [Link](https://www.worldbank.org/en/topic/sustainabledevelopment/brief/esg-metrics-primer)
8. "Corporate Governance and Equity Prices" by Paul Gompers and Joy Ishii. [Link](https://www.nber.org/papers/w8449)
