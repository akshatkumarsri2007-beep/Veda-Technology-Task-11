# Task 11 – Advanced Filtering & Business Question Answering

Business insight sheet built from raw order data using Excel conditional formulas (SUMIFS, COUNTIFS, AVERAGEIFS).

**Intern:** Akshat Srivastava · **Company:** Veda Technology · **Role:** Data Analytics Intern
**Program:** Data Analytics Internship — Level 1, Day 11

---

##  Overview

This task answers five targeted business questions directly from a raw Superstore order dataset (120 records, 10 columns) using Excel's conditional and lookup formulas — instead of manually sorting or scanning the sheet. A supporting **Filter Raw Data** sheet was built alongside the raw table to isolate specific orders, regions, categories, and segments on demand.

##  Objective

Practice using conditional aggregation formulas (`SUMIFS`, `COUNTIFS`, `AVERAGEIFS`) and sorting/filtering techniques to pull specific, decision-ready answers out of a raw transactional dataset.

##  Tools Used

- Microsoft Excel

##  Dataset

Sample Superstore Dataset — 120 records, 10 columns.

##  Business Questions & Answers

| # | Business Question | Answer |
|---|---|---|
| 1 | Which Region has the highest sales? | West — Rs. 7,15,050 |
| 2 | Which Category is most profitable? | Office Supplies — Rs. 1,19,987.88 profit |
| 3 | Which orders resulted in a loss? | 12 orders (out of 120) |
| 4 | What is the total sales of the Corporate segment? | Rs. 10,14,600 |
| 5 | Which order(s) had the highest quantity? | 15 units — 11 orders tied (e.g. ORD-1009, ORD-1012, ORD-1032) |

##  Supporting Breakdown

### Region-wise Sales & Profit

| Region | Orders | Sales (Rs.) | Profit (Rs.) |
|---|---|---|---|
| West | 33 | 7,15,050 | 90,561.61 |
| South | 36 | 6,09,600 | 64,960.63 |
| East | 25 | 5,29,450 | 40,212.72 |
| North | 26 | 4,28,050 | 78,140.04 |

### Category-wise Sales, Profit & Margin

| Category | Orders | Sales (Rs.) | Profit (Rs.) | Margin % |
|---|---|---|---|---|
| Office Supplies | 49 | 10,68,200 | 1,19,987.88 | 11.2% |
| Furniture | 40 | 6,98,800 | 75,759.75 | 10.8% |
| Electronics | 31 | 5,15,150 | 78,127.37 | 15.2% |

##  Key Insights

- **West leads on sales, North is leaner.** West has the highest regional sales (Rs. 7,15,050), but North — with the lowest sales of the four regions — converts a higher share into profit (≈18% margin) than West (≈13% margin). Sales volume and profit efficiency don't move together.
- **Office Supplies wins on volume, not margin.** It's the most profitable category (Rs. 1,19,987.88) purely on order count (49 of 120), even though its margin (11.2%) isn't the best. Electronics has fewer orders (31) but the healthiest margin (15.2%); Furniture sits lowest on margin (10.8%).
- **Losses are rare but not negligible.** Only 12 of 120 orders (10%) were loss-making — the business model is sound, but a few of those losses run Rs. 1,500–2,400 each and are worth periodic review.
- **Corporate is the anchor segment.** At Rs. 10,14,600, Corporate accounts for nearly 45% of total sales (Rs. 22,82,150) — more than Home Office and Consumer combined come close to matching.
- **High order quantity is a pattern, not an anomaly.** Eleven orders hit the max quantity of 15 units, spread across multiple categories and regions rather than concentrated in one segment.

##  Takeaway

Answering business questions straight from raw data with conditional formulas — rather than eyeballing a sorted list — makes the answers reproducible and audit-friendly. It also surfaces subtleties a single sorted view would hide, like a lower-sales region still generating strong profit, or a category leading on profit through volume rather than margin. The real value of `SUMIFS`/`COUNTIFS` here isn't speed — it's that the same five formulas will still give the right answer after the dataset grows well past 120 rows.

---

*Part of the Veda Technology Data Analytics Internship — Level 1, Day 11.*
