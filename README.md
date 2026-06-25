# Difference-in-Differences Project: AI Shopping Assistant

## Project Overview

This project uses Difference-in-Differences to estimate whether an AI shopping assistant increased 30-day customer retention.

The AI assistant launched in selected treatment cities. Other cities did not receive the feature and serve as the control group.

## Business Question

Did the AI shopping assistant increase 30-day retention?

## Method

I used Difference-in-Differences to compare retention changes before and after launch between treatment and control cities.

The main model estimates the interaction between:

* treatment city
* post-launch period

The key variable is `did`.

## Final Result

The final model includes:

* city fixed effects
* month fixed effects
* user-level control variables

The estimated DiD effect is **4.49 percentage points**.

The p-value is **0.0132**, which is below 0.05.

This means the result is statistically significant.

The 95% confidence interval is from **0.94 to 8.03 percentage points**.

## Business Recommendation

The AI shopping assistant appears to improve 30-day retention.

I recommend expanding the feature to more cities, while continuing to monitor guardrail metrics such as:

* 30-day spending
* app sessions
* customer support tickets
* discount usage
* model cost
* user complaints

## Tools Used

* Python
* Pandas
* Matplotlib
* Statsmodels
* Jupyter Notebook
* Difference-in-Differences
