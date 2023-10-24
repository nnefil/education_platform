# Educational Data Analysis: 

 - Python 
 - SQL

This repository contains scripts and analysis for an educational platform. The main goal of the project is to analyze user behavior, particularly focusing on engagement and monetization metrics. By understanding these aspects, we aim to optimize the user funnel and improve the platform's features.

# Python part

## Project Overview

This analysis focuses on the results of an A/B test for a new payment mechanism, aiming to identify whether the proposed changes should be adopted across the platform. Through rigorous data analysis and statistical testing, the project offers insights into user behavior and the efficacy of the new system compared to the old one.

## Datasets

The analysis uses several datasets that include information about user groups, activity, and payments:

- `groups.csv`: Data on user group allocation, indicating whether users belong to the control (A) or experimental (B) group.
- `groups_add.csv`: Additional data on group allocation obtained post-experiment.
- `active_studs.csv`: Information on users who were active during the testing period.
- `checks.csv`: Records of transactions made during the experiment.

These datasets form the backbone of our A/B testing analysis, providing a comprehensive view of user engagement and interaction with the payment system during the test phase.

## Key Findings

The project delves deep into comparison metrics between the two groups, highlighting key performance indicators and user response to the new mechanism. While specific outcomes are detailed within the project, significant findings include:

- **Engagement Metrics**: Differences in how often and how long users interacted with the platform, pointing to shifts in engagement patterns.
- **Revenue Indicators**: Changes in revenue generation, with a focus on payment frequency, average transaction value, and overall income.
- **User Experience**: Insights derived from user behavior, potentially reflecting their experience and satisfaction with the new system.

These findings, among others in the project, are instrumental in making an informed decision about the wider implementation of the new payment mechanism.

## Technologies

- **Python**:
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, SciPy
- **Environment**: Jupyter Notebook

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
