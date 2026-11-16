# Data Science Roadmap: Daily Plan & Progress

**Pace:** about 2 h/day, Monday–Saturday. Sunday is for rest or catching up.
**Start:** Tue 17 Nov 2026 · **Core roadmap ends:** about early April 2027 · **Extension ends:** about early May 2027
**How it works:** each day, open the chat and say `Day N done` (or `stuck on Day N`). I check your folder, review the work and give you the next day in detail.

**Main dataset for Levels 0–2:** [Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). It has 9 linked tables: orders, customers, payments, reviews and more. That makes it good for SQL joins, KPIs and cohorts, and later for NLP on its review text.

**If exams or the PFE take your time:** mark those days `PAUSED` and shift the dates. Never skip a level's exit check.

---

## Where you are now
- [x] Math foundations: vectors, matrices, PCA, distributions/t-test, confidence intervals, correlation
- [ ] Math notebooks need fixes (see Days 1–2)
- [ ] Level 0 not started (EDA notebook, SQL practice)

---

## Week 1: Close the math foundations (17–21 Nov)

| Day | Date | Task | Deliverable | Done |
|---|---|---|---|---|
| 1 | Tue 17 Nov | Sync the folder with GitHub. Fix 01_Vectors (feature scaling and cosine similarity) and 02_Matrices (meaningful multiplication, real rotation matrix) | 2 fixed notebooks, pushed | [x] |
| 2 | Wed 18 Nov | Fix 03 (eigh, true variance %), 04 (paired test, one-sided, Cohen's d), 05 (title). Finish Correlation as 06 (goal, takeaways, correlation ≠ causation) | 4 notebooks, pushed | [ ] |
| 3 | Thu 19 Nov | **07 Gradient descent, part 1:** linear regression, MSE loss, deriving the gradient by hand, implementing GD in NumPy | 07_Gradient_Descent.ipynb | [ ] |
| 4 | Fri 20 Nov | **07, part 2:** effect of the learning rate (too small / good / divergent), loss curve, comparing with the normal equation and sklearn | Notebook complete, pushed | [ ] |
| 5 | Sat 21 Nov | **08 Probability and Bayes:** conditional probability, Bayes on a fraud-alert example, checking it by simulation | 08_Probability_Bayes.ipynb, pushed | [ ] |

## Week 2: Level 0, setup and audit (23–28 Nov)

| Day | Date | Task | Deliverable | Done |
|---|---|---|---|---|
| 6 | Mon 23 Nov | Repo structure (`Level0/`, `data/` gitignored, `sql/`). Download Olist. Pandas audit: load all 9 tables, shapes, dtypes, keys | Level0/01_olist_audit.ipynb | [ ] |
| 7 | Tue 24 Nov | Mini EDA: missing values (why they're missing, not just how many), date parsing, duplicates, joining orders, items and customers | Cleaning section | [ ] |
| 8 | Wed 25 Nov | Mini EDA: summary statistics, 3 charts that each answer a question, written conclusions | Level0/02_mini_eda.ipynb, pushed | [ ] |
| 9 | Thu 26 Nov | SQL: load Olist into SQLite. Patterns 1–10: SELECT, WHERE, ORDER BY, GROUP BY, HAVING, CASE | sql/olist_patterns.sql | [ ] |
| 10 | Fri 27 Nov | SQL patterns 11–20: INNER/LEFT joins, multi-table joins, subqueries, CTEs | +10 queries | [ ] |
| 11 | Sat 28 Nov | SQL patterns 21–30: window functions (ROW_NUMBER, RANK, LAG, running totals, moving averages). **Level 0 exit check** | 30 queries, pushed | [ ] |

---

## Weeks 3–24: overview (each week gets a day-by-day plan before it starts)

| Week | Dates | Level | Focus | Deliverable |
|---|---|---|---|---|
| 3 | 30 Nov–5 Dec | 1 · Analysis | Cleaning and EDA: outliers, data dictionary | Olist sales analysis notebook |
| 4 | 7–12 Dec | 1 | Visualization and storytelling: charts → insights → recommendations | Sales analysis, final version |
| 5 | 14–19 Dec | 1 | SQL metrics: cohorts, retention, funnels | KPI analysis project. **Level 1 exit** |
| 6 | 21–26 Dec | 2 · Statistics | Sampling, bias, effect size, statistical power | Stats notebook |
| 7 | 28 Dec–2 Jan | 2 | A/B testing, guardrail metrics, segments, Simpson's paradox | A/B test analysis project |
| 8 | 4–9 Jan | 2 | Writing an analytics memo | 1-page decision memo. **Level 2 exit** |
| 9 | 11–16 Jan | 3 · ML | Workflow: baseline, train/val/test split, preprocessing, leakage | ML workflow notebook |
| 10 | 18–23 Jan | 3 | Classification: logistic regression, trees, confusion matrix, ROC/PR-AUC | Churn model, built properly |
| 11 | 25–30 Jan | 3 | Regression, feature engineering, regularization, ensembles | Price-prediction model |
| 12 | 1–6 Feb | 3 | Error analysis project | Churn/price project with error slices |
| 13 | 8–13 Feb | 3 | Cross-validation, tuning, class imbalance | Improved model and comparison |
| 14 | 15–20 Feb | 3 | Interpretability: feature importance, SHAP, communicating risk | **Level 3 exit** |
| 15 | 22–27 Feb | 4 · Modern | NLP: TF-IDF, embeddings, classification, topic discovery | Review-text notebook |
| 16 | 1–6 Mar | 4 | Text intelligence project (Olist reviews → complaint triage) | Applied NLP project |
| 17 | 8–13 Mar | 4 | Recommendation or demand forecasting | Specialization project |
| 18 | 15–20 Mar | 4 | Product case study: success metrics, decision framework | Case study. **Level 4 exit** |
| 19 | 22–27 Mar | 5 · Portfolio | Packaging: READMEs, case studies, visuals | 3 flagship repos |
| 20 | 29 Mar–3 Apr | 5 | Freelance readiness: scoping, proposals, interview practice | Proposal template. **Level 5 exit** |
| 21–24 | 5 Apr–1 May | 6 · Stretch | Specialization capstone and a lightweight dashboard or API | Capstone |

---

## Log
<!-- One line per day: date — what you did — what was hard -->
- Day 1: synced with GitHub, fixed 01_Vectors (scaling + hand-written cosine) and 02_Matrices (meaningful products, real rotation matrix). Hard: seeing that a compatible shape does not mean a meaningful product, and that steps swamp sleep without scaling.
