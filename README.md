# a-b_testing

## Project Overview
Analysis of marketing campaign effectiveness using statistical methods in Python. We compare two user groups: the test group that saw the actual advertisement (ad) and the control group that saw a public service announcement (psa).

## Goal
To determine whether there is a statistically significant difference in conversion rates between the two groups.

## Tech Stack
* Environment: Jupyter Notebook
* Libraries: Pandas, NumPy, SciPy (stats), Matplotlib, statsmodels(Z-test).

## Workflow
**1.** Implemented Stratified Sampling to create balanced groups, ensuring a fair and unbiased comparison between the test (ad) and control (psa) populations.

**2.** Formulated hypotheses and calculated conversion rates for both groups:
Ad Group Conversion: 26.4%
PSA Group Conversion: 20.2%

**3.** Performed a Z-test to determine if the difference in conversions was statistically significant. The resulting p-value (0.039) was less than the standard alpha threshold of 0.05, allowing us to reject the null hypothesis and confirm that the difference is statistically significant.

**4.** Calculated aggregate functions for ad views across both groups:
Means: ~24–25 views
Medians: ~12–13 views
The gap between the mean and median indicates a high data spread and the presence of outliers that skew the average.

**5.** Visualization & Outlier Analysis
Used Boxplots to identify outliers in both groups. The distribution of views was nearly identical confirming that the groups had equal exposure. This validates the fairness of the A/B test and the conclusion that the higher conversion in the "ad" group was due to the advertisement itself.

## Conclusions
* With a p-value of 0.039 (lower than the 0.05 threshold), we successfully rejected the null hypothesis. The increase in conversion for the test group is statistically significant, confirming that the advertisement effectively drives user action.
* The analysis confirmed that both groups were exposed to the content with equal intensity (median of 12–13 impressions). This ensures that the results were not biased by uneven ad delivery.
* The discovery of significant outliers (users with 100+ impressions) suggests an opportunity for cost savings. Implementing a "frequency cap" could prevent over-exposure and save marketing budget without sacrificing conversions.

## Files Description
1. Original file `marketing_AB.csv`.
2. Jupyter Notebook Python code are in file `a_b_marketing.ipynb`.
