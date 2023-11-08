# Educational Platform Data Analysis project: 

 - Python 
 - SQL

This repository contains scripts and analysis for an educational platform. The main goal of the project is to analyze user behavior, particularly focusing on engagement and monetization metrics. By understanding these aspects, we aim to optimize the user funnel and improve the platform's features.

# Python part

# A/B Testing Analysis for New Payment Mechanics

## Description

This project aims to determine whether a new payment mechanism should be implemented for all users based on the results of A/B testing. We've conducted a thorough analysis of user behavior and response towards the new mechanism, focusing on various critical metrics and user data.

## Main Steps

1. **Data Preparation:**
   - Used data from various sources including `groups.csv` for user group segmentation, and additional data like `groups_add.csv`, `active_studs.csv`, and `checks.csv` for comprehensive analysis.

2. **Analysis Tasks:**
   - Identified key metrics for evaluating the experiment's success.
   - Conducted a comparative analysis to find statistically significant differences between control and experimental groups.

3. **Anomaly Detection:**
   - Addressed anomalies in the data, such as undistributed students and users with extremely high payments, ensuring they don't skew the results.

4. **Function Implementation:**
   - Developed functions `key_metrics` for calculating essential metrics and `plot_metrics` for visual representation of the results.

## Results

- The Conversion Rate (CR) remained stable, indicating that the new payment mechanics didn't deter potential customers.
- Average Revenue Per User (ARPU) shows some growth but we coulnd proof that this increase is statistically significant. 
- There was a significant increase in Average Revenue Per Paying User (ARPPU), suggesting a positive impact of the new payment mechanics.


## Technologies

- **Python:** The primary programming language used for data manipulation, calculation, and analysis.
- **Pandas:** A fast, powerful, flexible, and easy-to-use open-source data analysis and manipulation tool.
- **Matplotlib/Seaborn:** Used for creating static, interactive, and animated visualizations in Python.


## Conclusions

The new payment mechanism showed a positive trend in key financial metrics without negatively impacting the user conversion rate. It's crucial, however, to ensure that the increase in revenue outweighs any additional costs related to the implementation of this new system. If the potential profit exceeds these costs, and the assumptions about the anomalies are correct, the recommendation is to proceed with the deployment of the new system into production.


# SQL Part

## Description

This project involves an in-depth analysis of user behavior and monetization for an educational platform. The platform operates under a trial model, offering students the ability to solve a certain number of problems for free each day, with the option to purchase full access for additional resources. The main focus was on identifying diligent students and assessing the impact of a new payment screen through various key performance indicators.

## Main Steps

1. **Identifying Diligent Students**: 
   - Analyzed user engagement based on the activity in solving small tasks called 'peas'.
   - Criteria: Students who solved at least 20 peas correctly in the current month.
   - Utilized data from the `default.peas` table, containing student IDs, timestamps, correctness, and subject information.

2. **Funnel Optimization Experiment**:
   - Writing the complex SQL query to calculate key metrics between control and experimental groups, including ARPU, ARPAU, and various conversion rates (CRs).
   - Analyzed user data from multiple tables: `default.peas`, `default.studs`, and `default.final_project_check`.

## Results

- **Diligent Students**: 
  - Identified a total of 136 students meeting the criteria of 'very diligent' based on their performance in solving peas.

- **Funnel Optimization**:
  - The experimental group (pilot) showed significantly better performance across all key metrics compared to the control group.
  - Improvements in ARPU (Average Revenue Per User) and ARPAU (Average Revenue Per Active User) indicate increased monetization among the experimental group.
  - Notable increases in conversion rates (both general and active users) suggest that the changes likely had a positive impact on user purchasing behavior.
 .

## Technologies

- **SQL**: Leveraged advanced SQL queries for data extraction and manipulation, ensuring optimization for handling large data volumes.
- **Database Management**: Engaged with multiple database tables, managing complex joins, and aggregations to derive meaningful insights.
- **Data Analysis**: Employed various data analysis techniques to interpret key metrics, identifying trends, and making data-driven recommendations.

## Conclusions

The experiment underscored the effectiveness of the new payment screen, demonstrating its impact through enhanced monetization and improved user engagement metrics. The positive outcomes affirm the decision to innovate and emphasize the importance of continual testing and optimization in the educational platform's features for sustained growth and user satisfaction.

