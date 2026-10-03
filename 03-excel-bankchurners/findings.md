# Bank Customer Churn Analysis — Excel Findings

## Business Question
Which customer segments and behaviors predict churn, and what should the bank monitor to catch at-risk customers early?

## What I Did
- Analyzed 10,127 bank customers using pivot tables in Excel
- Broke down churn by income, education, card category, gender, and age
- Compared transaction amount change vs. transaction count change (Q4 vs. Q1) between churned and retained customers
- Checked each finding for statistical reliability (sample size) before drawing conclusions
- Built a dashboard with supporting charts (churn by age, education, income)

## Key Findings

### 1. Overall churn rate: 16.1%
1,627 of 10,127 customers churned.

### 2. Demographic factors are weak standalone predictors
Income, education, and card tier all show churn rates clustered between 14–18% — none stand out as a strong signal on their own. The one exception: **Doctorate holders churn notably higher at 21.1%**, worth flagging even though the broader education category isn't predictive.

### 3. A data-reliability catch
Platinum cardholders showed a 25% churn rate — but this is based on only 20 total customers, too small a sample to trust. Flagged as statistically unreliable rather than reported at face value.

### 4. Transaction frequency is the strongest signal in the dataset
| Transaction Count Change | Churn Rate |
|---|---|
| Increased | 6.3% |
| Decreased | 16.9% |
| No Change | 10.2% |

Customers whose transaction count declined quarter-over-quarter churned at nearly **3x the rate** of customers whose count increased.

### 5. Transaction amount change is a much weaker signal
| Transaction Amount Change | Churn Rate |
|---|---|
| Increased | 14.3% |
| Decreased | 16.3% |

Only a 2-point gap — spending amount alone barely separates churned from retained customers.

## Recommendation
The bank should monitor transaction **frequency** trends, not just spending value or demographics, to flag at-risk customers early. A customer can maintain stable total spending while quietly reducing how often they use the card — and that drop in usage frequency is a meaningfully stronger early-warning signal than anything demographic or spend-based.
