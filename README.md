\# Halston \& Reid: Sales and Marketing Analysis

Lifesight Data Science Intern case study · Terese Mathew, M.Sc. Data Science, CHRIST (Deemed to be University)



Exploratory analysis of 130 weeks (Dec 2023 – Jun 2026) of sales and marketing data for Halston \& Reid, a US luxury apparel brand selling online and through its own stores. The goal: understand the business, find what drives revenue, separate observed relationships from causal claims, and recommend what to do and test next.



\## Files

| File | What it is |

|---|---|

| `eda.ipynb` | Exploratory analysis in Python: data checks, growth, seasonality, online vs store, promotions, marketing spend, marketing vs sales, recommendations |

| `dashboard.pbix` | Power BI dashboard (5 pages: Overview, Seasonality, Promotions, Marketing, Recommendations) |

| `dashboard pdf.pdf` | PDF export of the dashboard for quick viewing without Power BI |

| `Halston\_Reid\_Case\_Study.xlsx` | Original case study data |



\## How to run

\*\*Notebook\*\*

1\. `pip install pandas numpy matplotlib openpyxl jupyter`

2\. Keep `eda.ipynb` and `Halston\_Reid\_Case\_Study.xlsx` in the same folder.

3\. Run `jupyter notebook`, open `eda.ipynb`, and run all cells.



\*\*Dashboard\*\*

1\. Open `dashboard.pbix` in Power BI Desktop (free).

2\. If asked for the data, go to Transform data → Data source settings → Change source, and select `Halston\_Reid\_Case\_Study.xlsx`.

3\. No Power BI? Open `dashboard pdf.pdf`.



\## Approach

1\. \*\*Data audit:\*\* checked completeness, reconciliation and every numeric claim in the brief.

2\. \*\*Preparation:\*\* retail calendar (week of 31 Dec 2023 = 2024 week 1); like-for-like comparisons use weeks 1–25 because 2026 is a half year; months compared on average weekly revenue.

3\. \*\*Exploratory analysis:\*\* growth split into orders vs AOV; seasonality; online vs store; promotions compared within the same month; spend by channel over time.

4\. \*\*Marketing vs sales:\*\* correlations before and after removing seasonality and trend, plus the 2024 Google Shopping pause read against the same weeks of 2025. No causal claims.



\## Key findings

1\. \*\*Growth is shifting to basket value:\*\* H1 revenue +24% (2025) and +28% (2026); 45% of 2026 growth came from higher AOV vs 31% in 2025.

2\. \*\*Strong seasonality with a stagnant low season:\*\* June peaks at \~3.3x October; most months grew 10–50% in 2025, October only \~3.5%.

3\. \*\*Promotions look better than they are:\*\* +28% overall, but only \~+11% vs non-promo weeks in the same month, with lower AOV in \~2/3 of months.

4\. \*\*Lean, more efficient marketing:\*\* media is 3–5% of revenue; revenue grew \~20% in 2025 while spend fell \~13%.

5\. \*\*Most spend–revenue correlations are seasonality:\*\* only Meta and Google Shopping still track online revenue after adjustment.



\## Recommendations

1\. Review promotions in already-strong weeks to protect AOV and full-price positioning.

2\. Grow the autumn trough: test a capsule launch or direct mail drop in October, with a holdout group.

3\. Track AOV and full-price mix as core KPIs.

4\. Measure before moving budget: a direct mail holdout, a Google Shopping geo test and a Meta lift study, then a marketing mix model calibrated on the results.



\## Limitations

Observational data (no causal claims); 12 correlated channels over 130 weeks; no impressions, clicks, traffic, price or inventory data; offline channels act over several weeks but are booked in one.

