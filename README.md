# Educational Data Analysis: SQL Project

This repository contains SQL scripts and analysis for an educational platform. The main goal of the project is to analyze user behavior, particularly focusing on engagement and monetization metrics. By understanding these aspects, we aim to optimize the user funnel and improve the platform's features.

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

## Files in this Repository

- `final_project_sql.ipynb`: Jupyter notebook containing SQL queries, results, and comprehensive analysis.