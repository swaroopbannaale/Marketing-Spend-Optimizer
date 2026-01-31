# Marketing-Spend-Optimizer
 project optimizes marketing budgets for maximum yield from ad spend data (15k+ records on campaigns, engagement, banners, placements). Key outcomes include 20% projected ROI uplift via reallocation, XGBoost predictions, and strategies like prioritizing high-engagement segments
The project preprocesses marketing data, uncovers insights (e.g., Camp 2: 1.05 ROI; high engagement best), runs hypothesis tests (ANOVA rejects null on ROI diffs), and builds revenue predictors for budget reallocation (+20% projected ROI).
​
Key Components
Preprocessing: Cleans 15,408 rows (drop dups/NaNs, fill placement="unknown"), engineers 12+ features (CTR, ROI, ROAS, banner area, engagement numeric).
​
EDA: Univariate stats (e.g., revenue mean $17.94), groupbys (campaigns/placements/banners), heatmaps, bars saved as PNGs.
​
Stats: ANOVA (F=132.61, p=0), t-tests (revenue diffs), correlations (revenue~postclicksales 0.89), Chi-square (banner impact).
​
ML & Optimization
Models: Linear Reg (R²=0.90), RF (0.99), GB, XGBoost best; feature importance: postclickconversions 62%.
​
Strategies: Reallocate budget (Camp 1: -69% to Camp 2 +431%); 12-month roadmap (A/B tests Month 1-2).
​
Setup
Colab-ready: files.upload("onlineadvertisingperformancedata.csv"); libs: pandas/numpy/matplotlib/seaborn/sklearn/scipy/xgboost/statsmodels. Run top-to-bottom for dashboards/models/recs
