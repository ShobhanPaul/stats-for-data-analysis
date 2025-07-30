# Delivery Time Analysis Across Cities (Kruskal-Wallis + Dunn’s Test)

## 📌 Objective
Analyze whether delivery times differ significantly across three cities (City A, B, and C), using a non-parametric statistical approach suited for real-world, potentially non-normal data.

## 📊 Dataset Description
The dataset simulates delivery times for three cities:

- **City A**
- **City B**
- **City C**

Each city's delivery time (in minutes) is represented by a sample of 30 observations.

## 🧪 Statistical Tests Used

### 1. Kruskal-Wallis H-Test
- A non-parametric alternative to one-way ANOVA.
- Used when the assumption of normality may not hold.
- Null Hypothesis (H₀): All groups have the same median delivery time.
- Result: **p = 0.0063** → Reject H₀.

### 2. Post-hoc Analysis: Dunn’s Test with Bonferroni Correction
To determine which specific city pairs differ:

| Comparison | p-value | Conclusion |
|------------|---------|------------|
| City A vs City B | 0.134 | Not significant |
| City A vs City C | 0.770 | Not significant |
| City B vs City C | 0.005 | **Significant** ✅ |

### Medians:
- City A: 15.55 mins
- City B: 23.95 mins
- City C: 13.20 mins

## ✅ Conclusion
- **City C has significantly faster delivery times than City B.**
- **City A and City C**, and **City A and City B** are **not significantly different**.
- City C is the **best-performing region** in terms of delivery speed based on this analysis.

## 💼 Business Implication
City C's delivery operations are outperforming others. Efforts can be made to investigate what makes City C efficient and replicate its practices in other cities.

---

**Test Type**: Non-parametric  
**Test Name**: Kruskal-Wallis H + Dunn's Post-hoc  
**Goal**: Understand regional delivery time efficiency
