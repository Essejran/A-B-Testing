# 🧪 A/B Testing – Conversion Rate Experiment

This project demonstrates a complete A/B test analysis using simulated binary outcome data. It is part of a strategic data science portfolio tailored for roles in e-commerce optimization and experimentation leadership.

## 🎯 Objective

Evaluate whether a new website or product variant leads to a statistically significant improvement in customer conversion rates compared to a control version.

## 📦 What's Included

- Simulated user-level binary conversion data (`converted = 1` or `0`)
- Proportional z-test to compare conversion rates between control and variant groups
- Visual comparison of conversion outcomes
- Clear business interpretation of results

## ✅ Methodology

- Classical **two-proportion z-test** using `scipy.stats`  
- Confidence intervals and p-values interpreted for business impact
- Statistical assumptions clearly stated and respected

## 📊 Tools Used

- Python 3.x
- `pandas` for data wrangling  
- `numpy` for calculations  
- `scipy.stats` for statistical testing  
- `seaborn` and `matplotlib` for visualizations

## 🧪 Z-Test Summary

A z-test checks whether the observed difference between conversion rates is likely due to random chance. The key elements are:

| Element        | Description |
|----------------|-------------|
| **Null Hypothesis (H₀)** | No difference in conversion rates |
| **Alternative Hypothesis (H₁)** | Variant conversion rate ≠ control conversion rate |
| **p-value** | Probability of observing the difference (or more extreme) if H₀ were true |
| **α (Significance Threshold)** | 0.05 commonly used in business settings |
| **Decision Rule** | Reject H₀ if p-value < 0.05 |

## 📈 Visualization

The analysis includes a barplot with 95% confidence intervals showing average conversion rate by group (control vs. variant). This helps both technical and non-technical stakeholders quickly interpret the impact.

## 📌 Assumptions

- Binary outcomes are independent and identically distributed
- Sample size is large enough for the normal approximation to hold
- No major external changes (e.g., ad campaigns, holidays) confound the results

## 💡 Business Interpretation

If the p-value is **< 0.05**, we consider the result **statistically significant** and may recommend launching the variant broadly.

If the result is **not significant**, we either maintain the control experience or design follow-up experiments to explore hypotheses more deeply.

---

This repo can be extended with:
- Bayesian A/B testing
- Power analysis and sample size planning
- Real aggregated conversion metrics (e.g., from web traffic logs or event data)
