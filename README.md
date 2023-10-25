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
- There was a significant increase in both Average Revenue Per User (ARPU) and Average Revenue Per Paying User (ARPPU), suggesting a positive impact of the new payment mechanics.
- Decision made not to consider data from 13 undistributed students and 10 users with anomalously high payments to avoid biased results.

## Technologies

- **Python:** The primary programming language used for data manipulation, calculation, and analysis.
- **Pandas:** A fast, powerful, flexible, and easy-to-use open-source data analysis and manipulation tool.
- **Matplotlib/Seaborn:** Used for creating static, interactive, and animated visualizations in Python.


## Conclusions

The new payment mechanism showed a positive trend in key financial metrics without negatively impacting the user conversion rate. It's crucial, however, to ensure that the increase in revenue outweighs any additional costs related to the implementation of this new system. If the potential profit exceeds these costs, and the assumptions about the anomalies are correct, the recommendation is to proceed with the deployment of the new system into production.


# SQL Part

## Project Overview

The project revolves around the analysis of 'peas,' which are small tasks within the platform's various lessons. Our analysis focuses on identifying diligent students based on their interactions and accomplishments concerning these tasks. We also conducted an experiment to test a new payment screen's effectiveness, analyzing different user metrics before and after its implementation.

## Datasets

The data used in this project comes from three main tables:

1. `default.peas`: Contains data about the 'peas' or tasks that students solve, including timestamps, whether they solved them correctly, and the subject.

2. `default.studs`: Information about the students, including an identifier and the experimental group they belong to.

3. `default.final_project_check`: Data concerning purchases made by students, including timestamps, the amount spent, and the subject.

## Key Findings

- Identification of highly diligent students based on task completion.
- Analysis of the effectiveness of a new payment screen through key metrics such as Average Revenue Per User (ARPU) and Conversion Rate (CR).
- The experimental group showed a significant improvement in all key metrics, suggesting the new payment feature's success.
