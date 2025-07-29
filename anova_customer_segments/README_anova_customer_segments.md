
# 📊 ANOVA + Tukey HSD: Customer Segment Purchase Analysis

## 🔍 Business Problem
A retail company wants to know whether **Bronze**, **Silver**, and **Gold** customers spend differently on average. Understanding this can help tailor marketing, pricing, and loyalty programs.

## 🧪 Hypothesis Testing Approach

### ✅ Test Used: **One-Way ANOVA**
- **Null Hypothesis (H₀)**: All customer segments have the same mean purchase amount.
- **Alternative Hypothesis (H₁)**: At least one segment has a different mean purchase amount.

### ✅ Follow-up Test: **Tukey's Honest Significant Difference (HSD)**
- Used for pairwise comparisons **after** a significant ANOVA result.
- Helps identify **which** segments differ.

## 📈 Dataset
- **Segment**: Customer group (Bronze / Silver / Gold)
- **Purchase_Amount**: Total amount spent by the customer (₹)

> Data was simulated using `numpy.random.normal()` to mimic real-world variation.

## 📊 Key Results

### ANOVA Output:
- **F-statistic** ≈ 54.20  
- **p-value** ≈ 5.16e-16 ➝ **Reject Null Hypothesis**

### Tukey HSD Summary:

| Comparison        | Mean Difference | Significant? |
|------------------|------------------|----------------|
| Bronze vs Gold   | +32.07           | ✅ Yes          |
| Bronze vs Silver | +15.42           | ✅ Yes          |
| Silver vs Gold   | +16.64           | ✅ Yes          |

## 💡 Business Insights
- All segments spend **significantly differently**.
- **Gold customers** spend the most, followed by **Silver**, then **Bronze**.
- This supports **segment-based pricing or targeting** strategies.

## 📂 Files in This Folder
- `anova_customer_segments.ipynb`: Full code, visualizations, and test interpretation.
- `README.md`: This summary.
