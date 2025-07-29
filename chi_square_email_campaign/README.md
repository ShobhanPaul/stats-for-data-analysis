\# Chi-Square Test – Email Campaign vs Purchase Rate



\## 📌 Problem Statement

An e-commerce company ran an A/B test with two versions of an email campaign (A and B) to see if one version leads to more purchases.



\## ❓ Business Question

Does the \*\*type of email\*\* sent (Version A or B) affect whether a customer makes a \*\*purchase\*\*?



\## 📊 Data Summary



| Email Version | Purchased | Not Purchased |

|---------------|-----------|----------------|

| A             | 40        | 160            |

| B             | 70        | 130            |



Total: 400 customers, equally split across both versions.



\## 🧪 Statistical Approach



\### Hypotheses:

\- \*\*Null Hypothesis (H₀)\*\*: Email version and purchase behavior are \*\*independent\*\* (no association).

\- \*\*Alternative Hypothesis (H₁)\*\*: Email version and purchase behavior are \*\*dependent\*\* (email influences purchase rate).



\### Test Used:

Chi-Square Test of Independence using `scipy.stats.chi2\_contingency`.



\### Result:

\- \*\*Chi-Square Statistic\*\*: 10.55  

\- \*\*p-value\*\*: 0.00116  

\- \*\*Degrees of Freedom\*\*: 1  

\- \*\*Expected Frequencies\*\*: \[\[55, 145],

\[55, 145]]


\### ✅ Conclusion:

Since p-value < 0.05, we \*\*reject the null hypothesis\*\*.  

There is a statistically significant association between email version and purchase rate.  

\*\*Recommendation:\*\* Email Version B led to higher purchases and should be used in future campaigns.



\## 💻 Tools Used

\- Python

\- Pandas

\- SciPy

\- Jupyter Notebook



---







