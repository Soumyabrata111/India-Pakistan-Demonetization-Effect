# India-Pakistan-Demonetization-Effect
This repository contains code to analyze the impact of the Indian demonetization event on the economic indicators of Pakistan.

# Demonetization and Economic Indicators in Pakistan
This project analyzes the impact of the Indian demonetization event on the economic indicators of Pakistan. We test the null hypothesis that there is no significant difference in the economic indicators of Pakistan before and after the demonetization event, and the alternative hypothesis that the event had a significant impact on the economic indicators of Pakistan, either positive or negative.

# Data
The data used in this project is stored in two CSV files: CG_DEBT_GDP_Pak.csv and PPPPC_Pak.csv. The former contains information on Central Government Debt as a percentage of Pakistan's GDP (PPP), while the latter contains data on Gross Domestic Product per capita, PPP (current international $) for Pakistan. Both datasets come from the International Monetary Fund's database. Data considered in the study is from 2014 to 2019. Data beyond 2019 has not been considered to let not the effects of COVID-19 & flood influence the result.

# Code
The code for this project is written in Python using the pandas, scipy, matplotlib, and seaborn libraries. We first read in the two datasets and rename the Pakistan column to match the variable names. We then merge the two datasets on the Year column to create a new DataFrame. We split this DataFrame into two: one for data before 2016 (the year of the demonetization event) and one for data after.

We perform several statistical tests on the data to analyze the impact of the demonetization event. First, we test for normality and equal variance between the two sets of data. We then perform a two-sample t-test and a Wilcoxon rank-sum test for each economic indicator.

Finally, we create line plots for each economic indicator with a marker at the year of the demonetization event.

# Results
Based on the hypothesis testing and data analysis performed, the following results were obtained:

The two-sample t-test results suggest that there is no significant difference in the economic indicators of Pakistan before and after the Indian demonetization event. The p-values for both CG_DEBT_GDP_Pak and PPPPC_Pak are greater than the significance level of 0.05. Therefore, we fail to reject the null hypothesis.

The Shapiro-Wilk test results suggest that the data for both CG_DEBT_GDP_Pak and PPPPC_Pak are normally distributed before and after the demonetization event. The p-values for both tests are greater than the significance level of 0.05.

The Levene's test results suggest that the assumption of equal variances is met for both CG_DEBT_GDP_Pak and PPPPC_Pak. The p-values for both tests are greater than the significance level of 0.05.

The Wilcoxon rank-sum test results suggest that there is no significant difference in the central government debt as a percentage of Pakistan's GDP (PPP) before and after the demonetization event. The p-value for the test is greater than the significance level of 0.05.

The line plot for CG_DEBT_GDP_Pak shows a slight decrease in the central government debt as a percentage of Pakistan's GDP (PPP) after the demonetization event, but the difference is not significant.

Overall, the analysis suggests that the Indian demonetization event did not have a significant impact on the economic indicators of Pakistan. However, it is important to note that this is based on the data available and the specific methods used in the analysis. Further research may be necessary to confirm these findings.

# Blog
The blog, entitled 'Uncovering the Effect of India's Demonetization on Pakistan's Economy through Statistical Analysis' related to this repository is avaialble at https://indian-demonetization-effect-pak.blogspot.com/2023/03/uncovering-effect-of-indias.html
