# Two‑Sample t‑Test: Impact of Ad Campaign on Customer Spending

## 📌 Business Context
The marketing team launched **two different ad campaigns**:
- **Ad A**
- **Ad B**

Management wants to know whether **Ad B drove higher customer spending** compared with Ad A.

## 🎯 Objective
Determine if the **average customer spending** differs significantly between the two ad groups.

## 📊 Dataset
Simulated data for 100 customers (50 per ad type):

| Column       | Description                               |
|--------------|-------------------------------------------|
| `Customer_ID`| Unique customer identifier                |
| `Ad_Type`    | Ad A or Ad B                              |
| `Spending`   | Amount spent by the customer (₹)          |

*Spending values were simulated with `numpy.random.normal()` to reflect realistic business variation.*

## 🧪 Statistical Methodology
1. **Assumption Checks**
   - **Normality:** Visual inspection (histogram + Q‑Q plot) indicated both groups approximately normal.
   - **Equal Variances:** Levene’s Test → p = 0.82 > 0.05 ⇒ assume equal variances.

2. **Two‑Sample t‑Test**
   - **Null Hypothesis (H₀):** Mean spending is equal for Ad A and Ad B.
   - **Alternative Hypothesis (H₁):** Mean spending differs between the two ads.

```
t = −3.89   p = 0.000185
```

## ✅ Results & Interpretation
- **p < 0.05** ⇒ Reject H₀  
- **Direction:** Negative t‑statistic ⇒  
  **`mean(Ad A)` < `mean(Ad B)`**

**Conclusion:**  
**Ad B significantly increases customer spending** compared with Ad A.

## 💼 Business Recommendation
Increase budget allocation for **Ad B** or optimize Ad A to match Ad B’s performance.

## 📂 Files in This Folder
- `two_sample_ttest_ad_spending.ipynb` – Code, visuals, and analysis  
- `README.md` – Business summary and interpretation

---

**Test:** Independent two‑sample t‑test  
**Goal:** Quantify marketing campaign impact on revenue
