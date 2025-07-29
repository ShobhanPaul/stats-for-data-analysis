# ANOVA on Employee Productivity Across Work Shifts

## 📊 Business Context

A company wanted to evaluate if **employee productivity** (measured by average tasks completed) varied significantly across different **work shifts**:

- **Morning Shift**
- **Afternoon Shift**
- **Night Shift**

Management suspected that productivity may be influenced by energy levels, sleep cycles, or workload patterns.

---

## 🎯 Objective

To determine whether the **average number of tasks completed per employee** is **significantly different** across the three work shifts using:

- **One-way ANOVA**
- **Tukey's HSD** (for post-hoc analysis)

---

## 📁 Dataset Structure

The dataset contains 30 employees per shift, each with:

- `Employee ID`: Unique identifier
- `Morning Tasks`: Number of tasks in morning shift
- `Afternoon Tasks`: Number of tasks in afternoon shift
- `Night Tasks`: Number of tasks in night shift

---

## 🧪 Statistical Methodology

1. **ANOVA (f_oneway)**:
   - **Null Hypothesis (H₀)**: Mean productivity is equal across shifts.
   - **Alternative Hypothesis (H₁)**: At least one shift has different average productivity.

2. **Tukey's HSD**:
   - If ANOVA result is significant (p < 0.05), identify which pairs of shifts differ.

---

## ✅ Results Summary

- **ANOVA p-value**: < 0.000001 → Reject H₀
- **Conclusion**: At least one shift's average productivity differs significantly.

### Tukey's HSD Comparison:

| Comparison              | Mean Difference | Statistically Significant? |
|-------------------------|-----------------|----------------------------|
| Morning vs Afternoon    | Yes             | ✅                          |
| Morning vs Night        | Yes             | ✅                          |
| Afternoon vs Night      | Yes             | ✅                          |

---

## 📌 Business Recommendation

Employees are **most productive in the Morning Shift**, followed by Afternoon, then Night.

**Recommendation**: Reallocate high-priority tasks to **Morning Shifts** and explore interventions to improve **Night Shift** performance.

---

## 🧠 Skills Demonstrated

- Simulation of real-world business data
- One-way ANOVA
- Post-hoc analysis with Tukey’s HSD
- Data reshaping (`melt`)
- Practical interpretation of statistical results

---

## 📂 Files Included

- `employee_productivity_anova.ipynb`: Full analysis
- `README.md`: Business summary and explanation

---