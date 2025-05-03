# E-News- Project
At E-news Express, We need to analyze the user interaction data from an A/B testing experiment conducted on the two landing page variants. The experiment aims to determine the effectiveness of the new design in increasing user engagement and conversions.
Specifically, the objectives are:
*Do the users spend more time on the new landing page than on the existing landing page?
*Is the conversion rate (the proportion of users who visit the landing page and get converted) for the new page greater than the conversion rate for the old page?
*Does the converted status depend on the preferred language?
*Is the time spent on the new page the same for the different language users.

# Data Dictionary 
The data contains information regarding the interaction of users in both groups with the two versions of the landing page.
user_id - Unique user ID of the person visiting the website
group - Whether the user belongs to the first group (control) or the second group (treatment)
landing_page - Whether the landing page is new or old
time_spent_on_the_page - Time (in minutes) spent by the user on the landing page
Converted - Whether the user gets converted to a subscriber of the news portal or not
language_preferred - Language chosen by the user to view the landing page

# Solution Approach
**Data Preparation:** Load and clean the data, ensuring variables are in the correct format and addressing any missing or outlier values.
**User Engagement Analysis:** Perform a one-tailed t-test to compare the average time spent on the new and old landing pages.
**Conversion Rate Comparison:** Conduct a proportion z-test to determine if the new landing page has a higher conversion rate than the old one.
**Language Impact on Conversion:** Use a chi-square test to analyze if conversion status is dependent on the preferred language.
**Time Analysis by Language:** Conduct a one-way ANOVA to check if time spent on the new page differs across language groups, and summarize actionable insights.



**Conclusion** : The analysis conducted on the A/B test data for the two landing pages has provided valuable insights into user behavior and the effectiveness of the new landing page.

Here's a summary of the key findings:

**Time Spent on the Landing Pages:**
Users spent significantly more time on the new landing page compared to the old one. The statistical test (T-test) confirmed that this difference is statistically significant (p-value < 0.05), implying that the new landing page is more engaging and keeps users' attention for longer periods.

**Conversion Rates:**
The new landing page also demonstrated a higher conversion rate, as indicated by the results of the two-sample z-test for proportions (p-value = 0.008), which showed that the new landing page is more effective in converting visitors into subscribers.

**Conversion and Preferred Language:**
The analysis revealed no significant relationship between the preferred language of users and their conversion status. The Chi-square test returned a p-value of 0.213, suggesting that conversion rates are independent of the language preference of users.

**Time Spent and Language Preference:**
An analysis of the time spent on the new page by users with different language preferences (English, French, and Spanish) indicated no significant difference in engagement levels across these groups. The ANOVA test and subsequent tests for normality and variance homogeneity failed to reject the null hypothesis, indicating that the time spent on the page is consistent across language groups.

