# Employee Attrition Prediction & Retention Decision-Support Tool

###  Business Problem

Employee turnover costs organizations **6–9 months of an employee's salary** in recruiting, onboarding, and lost productivity. HR teams often react to attrition *after* resignations happen—but by then, the cost is already sunk.

This project builds a **decision-support tool** that identifies high-risk employees *before* they leave, enabling HR to prioritize retention interventions where they will have the greatest financial impact.

---

### 🎯 Objective

Build a machine learning model and interactive dashboard that:

1. Predicts which employees are at high risk of attrition
2. Identifies the key drivers of turnover
3. Segments at-risk employees by department, role, and satisfaction level
4. Quantifies the potential cost of inaction

---

###  Tools

| Category | Tools |
|----------|-------|
| Language | Python |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Power BI |
| Machine Learning | Scikit-learn (Random Forest, Logistic Regression) |
| Model Explainability | SHAP (feature importance) |

---

### Key Findings

**1. Overtime is the strongest single predictor of attrition**
Employees working overtime show a **31% attrition rate**—more than double the company average. This segment represents a critical risk group that can be addressed through workload redistribution.

**2. The model identifies high-risk employees with 85% recall**
The Random Forest model catches 85% of employees who actually leave, giving HR a proactive window to intervene. This is more valuable than raw accuracy because missing a high-risk employee is costlier than a false alarm.

**3. Sales and Laboratory Technician roles show disproportionately high exit rates**
These roles account for a significant share of total attrition. Targeted career-path interventions in these functions would have outsized impact.

**4. Younger, lower-income employees are more likely to leave**
Early-tenure employees with lower compensation show the highest flight risk. This aligns with research on psychological contract breach and unmet growth expectations.

**5. Low job satisfaction is a leading indicator, not a lagging one**
Satisfaction scores drop *before* resignation. This makes satisfaction surveys an early-warning system, not just a retrospective metric.

---

### Dashboard Overview

The Power BI dashboard includes:

- **Risk Segmentation Page:** High-risk employee count, risk by department, risk by job role
- **Driver Analysis Page:** Feature importance (SHAP values), overtime vs. attrition, satisfaction vs. attrition
- **Financial Impact Page:** Estimated cost of turnover by department, cost of inaction for high-risk segments
- **Interactive Filters:** Department, job role, gender, tenure band

![Risk Segmentation](powerbi/screenshots/risk_segmentation.png)
![Driver Analysis](powerbi/screenshots/driver_analysis.png)
![Financial Impact](powerbi/screenshots/financial_impact.png)

---

### 💡 Business Recommendations

| Finding | Recommendation | Expected Impact |
|---------|---------------|-----------------|
| Overtime drives 31% attrition | Audit overtime-heavy roles and redistribute workload | Reduce attrition in highest-risk segment by 15–20% |
| Sales & Lab Tech roles have high exit rates | Create clear career progression paths for these functions | Improve retention in critical roles |
| Younger, lower-income employees leave most | Review entry-level compensation and growth opportunities | Reduce early-tenure attrition |
| Low satisfaction precedes exit | Act on survey data within 30 days, not quarters | Convert early warnings into interventions |
| Model identifies 85% of leavers | Integrate model into HRIS for monthly risk scoring | Shift from reactive to proactive retention |

---

### Quantified Business Impact

If the model helps HR retain just **10 high-risk employees** per year (conservative estimate):

- Average replacement cost: ₹3–5 L per employee
- **Total savings: ₹30–50 L annually**

This connects the technical work directly to the P&L.

---

###  Repository Structure


**Notebook:** [Employee_Attrition_Prediction_HR_Analytics.ipynb](Employee_Attrition_Prediction_HR_Analytics.ipynb)
