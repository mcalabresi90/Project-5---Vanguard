# Vanguard Customer Experience Analysis

## Project Overview

This project evaluates the effectiveness of a new UI design for Vanguard's customer experience. The primary goal is to assess whether the updated UI improves user engagement and completion rates compared to the traditional UI. The analysis is based on data collected during an A/B testing experiment that ran from March 15, 2017, to June 20, 2017.

## Key Performance Indicators (KPIs)

1. **Completion Rate (reaching step_4)**

   - Measures the percentage of users who complete the entire process.
   - Excluded visits that did not go through all steps (0-4) for accuracy.

2. **Average Time per Step**

   - Evaluates the efficiency of the UI by calculating the average time users take to complete each step.
   - Excluded repeated steps to ensure more accurate outcomes.

3. **Error Rate per Group**

   - Analyzes the frequency of errors encountered by users in the control and test groups.
   - Error rate is computed per visit_id when the user goes back to a previous step at least once.

## Hypothesis Testing

The analysis involves conducting statistical tests to evaluate the differences between the control and test groups for each KPI.

## Experiment Evaluation

### Design Effectiveness

The experiment was well-structured as an A/B test. The Test group consistently had more visits, which could indicate a traffic imbalance. There were no obvious biases identified in the assignment process.

### Duration Assessment

The experiment ran for about 3 months (03/15/2017 to 06/20/2017), which is generally enough time to collect meaningful data on user interactions.

### KPI 1: Completion Rate

- **Z-statistic:** 14.6441
- **P-value:** virtually 0 (7.35e-49)
- **Difference:** ~5.74 percentage points (Control: 48.67%, Test: 54.41%)
- **Conclusion:** The new UI significantly increases the completion rate.

### KPI 2: Average Time per Step

- **P-value:** All below 0.00001
- **Conclusion:** The new UI is significantly faster in completing steps.

#### Detailed Results:

- In 4 of the 5 steps, the test group was faster than the control group.
- Only in step 2 did the control group outperform the test group.
- The test group was on average 120 seconds faster during the entire process compared to the control group.
- Total time for the control group: 560 seconds.
- Total time for the test group: 440 seconds.

## Conclusions

The A/B test results show a significantly higher completion rate (product purchase) in the test group compared to the control group, indicating a successful and positive impact.

However, some metrics, like average time per step, may not fully capture the user experience. A deeper analysis requires insights into specific features and their impact. Overall, the new UI had a positive impact, but there’s room for improvement.

The error rate was strictly evaluated, counting any step repetition as an error. However, going back a step doesn't always indicate poor design, as users may revisit steps to review information before purchase.

### Final Thoughts

- Adding user qualitative feedback can provide valuable insights.
- Speed is not always better. Is the new process less informative? Will customers be disappointed with this purchase? (e.g., cancellation rate of the order, client satisfaction)
- Additional data collection and monitoring are recommended to assess long-term impact.

## How to Run the Analysis

1. Open the Jupyter notebook file.
2. Execute the cells in sequence to reproduce the analysis.
3. The results are summarized in the final sections of the notebook.
