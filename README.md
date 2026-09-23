# Email Experiment Analysis

## Overview

This project analyzes a multi-arm email experiment designed to understand how email content, user characteristics, and delivery frequency affect engagement and downstream conversion.

The experiment includes approximately 480,000 treatment users across 12 behavioral segments, 10 randomized email templates, and two delivery schedules: daily and twice weekly. The analysis evaluates email engagement, account linking and funding behavior, treatment effects, campaign timing, and the conversion funnel.

## Business Questions

The analysis focuses on five questions:

1. Which email templates generate the highest open rates, and which user characteristics are associated with stronger engagement?
2. How do account linking and funding rates vary across treatment groups?
3. Does receiving campaign emails increase funding rates relative to no-email control groups?
4. How does engagement change across successive email sends?
5. Where does the largest drop-off occur in the email-to-funding conversion funnel?

## Methods

- Email engagement and friction analysis
- Behavioral user segmentation
- Treatment vs. control comparison
- One-sided two-proportion z-tests
- Time-series analysis by scheduled send day
- Conversion funnel analysis

## Key Findings

- **Funding FAQ** achieved the highest open rate at **25.99%**, substantially outperforming the other email templates.
- Users active within the previous 20 days showed the strongest engagement difference, with a **19.41% open rate compared with 16.47%** among inactive users.
- Email treatment did not consistently increase funding across all segments. Only **2 of 24 treatment-frequency groups** showed statistically significant positive funding lift at the 5% level.
- Day 0 was not the highest-engagement send. Daily groups peaked on **Day 1 (19.58%)**, while twice-weekly groups peaked on **Day 4 (19.80%)**.
- The largest observed funnel drop-off occurred between **email opening and account linking**. Among eligible users, 49.58% opened at least one email, but only **3.92% of openers** subsequently linked an account.

## Recommendations

- Use the strong performance of the **Funding FAQ** template as a starting point for future messaging experiments.
- Incorporate recent user activity into targeting and personalization strategies.
- Investigate the **open-to-link** stage as the primary conversion bottleneck and test improvements to messaging, calls-to-action, and the account-linking journey.
- Continue experimenting with campaign timing and frequency rather than assuming additional sends generate additional value.

## Tools & Techniques

**Python:** pandas, NumPy, statsmodels, Matplotlib, Seaborn  
**Analysis:** A/B Testing, Two-Proportion Z-Test, User Segmentation, Time-Series Analysis, Funnel Analysis

## Repository

- [`Email_Experiment_Analysis.ipynb`](Email_Experiment_Analysis.ipynb) — Complete analysis, visualizations, statistical tests, and recommendations.

## Data

The original project data is not included in this repository. The notebook documents the dataset structure and analytical methodology used in the project.

## Note

The available data does not cover the full planned experiment observation window. Therefore, conversion rates and treatment-control results should be interpreted as interim rather than final experiment outcomes.
