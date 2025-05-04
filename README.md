# 📊 ESG Risk Analysis: Insights from S&P 500 Companies

**Author: Debraj Mahato**

---

## 🚀 Project Overview

This repository explores **Environmental, Social, and Governance (ESG) risk analysis** using a dataset of **S&P 500 companies**. ESG has become a vital lens through which companies are assessed, complementing traditional financial metrics with sustainability and ethical governance insights. The goal of this project is to **analyze, visualize, and model ESG risk factors**, helping stakeholders make data-driven decisions.

---

## 🌍 Why ESG Matters

With growing emphasis on sustainability and corporate responsibility, ESG analysis is crucial for:

- **Investors**: Identifying long-term risks and sustainable opportunities.
- **Companies**: Enhancing reputation and operational resilience.
- **Policymakers & Researchers**: Understanding industry-wide ESG trends.

By examining ESG metrics, stakeholders gain a **comprehensive understanding** of a company's sustainability profile and potential vulnerabilities.

---

## 🔑 Key ESG Metrics

| **Metric**                  | **Description**                                                                                 |
|-----------------------------|-------------------------------------------------------------------------------------------------|
| 🌎 Environmental Risk Score | Evaluates ecological impact and commitment to sustainability.                                   |
| 🏛️ Governance Risk Score    | Assesses governance structure, ethics, and corporate transparency.                              |
| 🤝 Social Risk Score        | Measures societal impact, including employee welfare and diversity.                             |
| ⚠️ Controversy Level        | Categorical measure (e.g., Low/Medium/High) of public or legal controversies.                   |
| 🔢 Controversy Score        | Numeric value quantifying the intensity of controversies (linked to reputational risks).        |

---

## 🗂️ Dataset Overview

The dataset focuses on companies listed in the **S&P 500 index** and includes the following key columns:

- `Symbol`
- `Sector`
- `Industry`
- `Full Time Employees`
- `Total ESG Risk Score`
- `Environmental / Governance / Social Risk Scores`
- `Controversy Level` & `Controversy Score`

This dataset can support ESG risk profiling, trend analysis, investment screening, and academic research.

---

## ⚙️ Data Cleaning Process

1. **Drop rows with missing ESG scores:**
   - `Total ESG Risk Score`
   - `Environmental Risk Score`
   - `Governance Risk Score`
   - `Social Risk Score`

2. **Fill numeric missing values:**
   - `Full Time Employees`: Filled with median.

3. **Fill categorical missing values:**
   - `Controversy Level`: Filled with `'Unknown'`.
   - `ESG Risk Level`: Filled with `'Unknown'`.

4. **Handle remaining missing values:**
   - Option to **drop rows** with missing `Controversy Score` or **impute** them using statistical/machine learning methods.

---

## 🔬 Analysis & Modeling

The repository includes:

- **Descriptive analysis** of ESG risk scores.
- **Visualization** of ESG distribution and outliers.
- **Predictive modeling** using **Random Forest Regressor** to forecast ESG-related metrics.

---

## 🚀 How to Run

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/esg-risk-analysis.git
