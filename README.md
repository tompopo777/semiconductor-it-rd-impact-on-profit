# 💹 Industry Analysis: IT and R&D Spending's Impact on Profit

A financial econometrics study examining how IT intensity and R&D investment impact firm profitability (ROA) across the semiconductor industry from 2017 to 2021, using OLS regression and multicollinearity diagnostics.

---

## 📖 Overview

This project investigates the relationship between a firm's IT and R&D spending and its Return on Assets (ROA) in the semiconductor sector. Using panel data from 2017–2021, the analysis applies OLS regression with control variables, VIF diagnostics, and correlation analysis to surface key drivers of profitability.

---

## ❓ Research Question

**How do IT intensity and R&D intensity affect the profitability (ROA) of semiconductor firms?**

---

## 📊 Dataset

- **Industry:** Semiconductor (2017–2021)
- **Key Variables:**

| Variable | Description |
|---|---|
| `ROA` | Return on Assets (dependent variable) |
| `IT_Intensity` | IT spending as a ratio of revenue |
| `RD_Intensity` | R&D spending as a ratio of revenue |
| `Leverage` | Debt-to-asset ratio |
| `CapEx_Intensity` | Capital expenditure ratio |
| `Cash_to_Assets` | Liquidity measure |
| `Sales_Growth` | Year-over-year revenue growth |
| `Firm_Age` | Years since firm founding |

> ⚠️ Dataset is not included due to confidentiality. Source: Compustat / WRDS.

---

## 🔍 Techniques Used

| Method | Purpose |
|---|---|
| OLS Regression (statsmodels) | Model ROA against IT/R&D and control variables |
| VIF Analysis | Detect multicollinearity among predictors |
| Pearson Correlation Heatmap | Visualize variable relationships |
| Trend Analysis | Track IT/R&D intensity over 2017–2021 |
| Scatter Plot + Regression Line | Visualize IT Intensity vs. ROA relationship |

---

## 📁 Project Structure

```
semiconductor-it-rd-impact-on-profit/
│
├── semiconductor_analysis.ipynb   # Main analysis notebook
├── requirements.txt               # Python dependencies
└── README.md
```

---

## 🚀 Key Steps

1. **Data Loading** — Load semiconductor firm-level panel data (CSV)
2. **OLS Regression** — Fit model with IT/R&D intensity and control variables
3. **Multicollinearity Check** — VIF analysis to validate model stability
4. **Summary Statistics** — Mean, SD, Min, Max for all variables
5. **Correlation Heatmap** — Pearson correlation matrix visualization
6. **Trend Visualization** — Bar and line plots of IT/R&D intensity by year
7. **ROA vs IT Intensity** — Scatter plot with regression line

---

## 📈 Results
<p align="center">
  <img src="images/OLS Regression Results.png" width="800" alt="OLS Regression Results.png"/>
</p>

### Correlation Heatmap
<p align="center">
  <img src="images/Correlation Heatmap.png" width="800" alt="Correlation Heatmap.png"/>
</p>

### IT & R&D Intensity Trend (2017–2021)
<p align="center">
  <img src="images/IT & R&D Intensity Trend (2017–2021).png" width="800" alt="IT & R&D Intensity Trend (2017–2021).png"/>
</p>

### Average IT Intensity and ROA (2017–2021)
<p align="center">
  <img src="images/Average IT Intensity and ROA (2017–2021).png" width="800" alt="Average IT Intensity and ROA (2017–2021).png"/>
</p>

### IT Intensity vs. ROA
<p align="center">
  <img src="images/IT Intensity vs. ROA.png" width="800" alt="IT Intensity vs. ROA.png"/>
</p>

---

## 📝 Conclusion

The semiconductor industry demonstrated a consistent upward trend in both
IT and R&D intensity from 2017 to 2021, reflecting the sector's heavy
reliance on continuous technological innovation and digital infrastructure
investment to maintain competitive advantage.

Firms that allocated higher proportions of revenue toward IT showed a
positive association with Return on Assets (ROA), suggesting that
strategic technology investment translates into measurable profitability
gains. Similarly, R&D intensity remained a core driver of firm performance,
consistent with the industry's innovation-driven business model where
product cycles are short and differentiation is critical.

The analysis also highlights that financial health indicators such as
leverage and capital expenditure intensity play important moderating roles
— firms with excessive debt burdens tended to show lower profitability
regardless of IT or R&D investment levels, underscoring the importance
of balanced capital allocation in a capital-intensive industry.

Overall, these findings suggest that semiconductor firms benefit most
when IT and R&D investments are sustained strategically over time,
rather than deployed reactively — reinforcing the notion that long-term
innovation commitment, not short-term spending spikes, is what drives
profitability in this sector.

---

## 🛠️ Libraries

- `pandas`, `numpy` — Data manipulation
- `statsmodels` — OLS regression and VIF analysis
- `matplotlib`, `seaborn` — Data visualization

