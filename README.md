# E-Commerce A/B Testing: Checkout Optimization

## Project Overview
This project analyzes the results of an A/B test conducted on an e-commerce platform to evaluate the performance of a new "One-Click Checkout" feature (Treatment Group) compared to the standard multi-page checkout (Control Group). The primary objective is to mathematically determine if the new design yields a statistically significant increase in the conversion rate.

## Tools & Techniques
- **Language:** Python
- **Libraries:** Pandas, NumPy, SciPy, Matplotlib, Seaborn
- **Skills:** A/B Testing, Experimental Design, Data Cleaning, Exploratory Data Analysis (EDA), Statistical Hypothesis Testing (Chi-Square)

## Methodology
1. **Data Generation:** Simulated a 14-day traffic log (3,000 users) with intentional experimental noise (routing errors) to mimic real-world tracking issues.
2. **Data Cleaning:** Identified and removed 137 corrupted rows where users were exposed to mismatched landing pages, ensuring absolute data integrity before testing.
3. **Exploratory Data Analysis:** Calculated baseline conversion rates. The Control group converted at **10.4%**, while the Treatment group converted at **15.0%**.
4. **Statistical Testing:** Conducted a Chi-Square test ($\alpha = 0.05$) to evaluate the statistical significance of the observed difference.

## Key Findings & Business Recommendation
- **$p$-value:** `0.000262`
- **Statistical Verdict:** Significant
- **Conclusion:** The probability of the conversion increase being a result of random chance is negligible (far below the 0.05 threshold). 
- **Actionable Insight:** The business should immediately deploy the "One-Click Checkout" feature to all users to maximize revenue.