# A/B Testing on Marketing Campaign Data in Python

## Introduction

This project performs an A/B test on a dataset to assess the impact of two different advertising strategies on user conversion rates. The primary goal is to determine if there is a significant difference in the conversion rates between the experimental group (exposed to advertisements) and the control group (exposed to a Public Service Announcement, or PSA).

## Background (Context and Problem)

Marketing campaigns are a key factor in driving sales, and understanding which type of advertisement is more effective is crucial. In this case, we have data from a marketing campaign where users were exposed to either an ad or a PSA. We want to test whether the exposure to an ad leads to a higher conversion rate (purchasing the product) compared to the PSA exposure.

This is a typical A/B testing problem where two groups are compared, and statistical analysis is used to assess the difference in outcomes between the groups. The objective is to determine whether the ad significantly influences user behavior compared to the PSA.

## Tools Used

**Python** and the following
- **pandas**: For data wrangling and manipulation.
- **numpy**: For numerical computations.
- **seaborn** and **matplotlib**: For data visualization and plotting.
- **scipy**: For performing the chi-squared statistical test.

## The Analysis

1. **Data Loading**: The dataset is loaded into Python using pandas and cleaned by removing unwanted columns and ensuring there are no duplicates or missing values.
2. **Exploratory Data Analysis (EDA)**: Initial exploration is conducted to check the basic statistics of the dataset, as well as to identify any anomalies such as duplicates and missing values.
3. **Conversion Rate Calculation**: The conversion rates for both groups (ad and psa) are calculated by dividing the number of conversions by the total number of users in each group.
4. **Statistical Test**: A chi-squared test for independence is performed to test the null hypothesis (no difference in conversion rates between the two groups). The p-value is used to determine if the difference in conversion rates is statistically significant.
5. **Visualizations**: The distribution of conversion rates for both groups is visualized using density plots to understand the spread and shape of the conversion rates.

## Results

- **Conversion Rates**:
  - The conversion rate for users exposed to ads is 2.55%, while for those exposed to PSAs, it is 1.78%.
  - This suggests that users exposed to ads have a higher conversion rate compared to those who saw a PSA.

- **Hypothesis Testing**:
  - The chi-squared test yielded a p-value much smaller than 0.05, indicating that the difference in conversion rates between the two groups is statistically significant. Therefore, we reject the null hypothesis and conclude that the ad exposure has a meaningful impact on the conversion rate.

## Conclusion

The A/B test results indicate that the advertisement exposure significantly improves the conversion rate compared to the PSA. This analysis helps guide marketing strategies by demonstrating the effectiveness of ads over PSAs in driving sales.
