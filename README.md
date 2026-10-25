# Fantasy Premier League & Football Performance Analytics

> English Premier League · Seasons 2025/26 and 2026/27
> Status: **Proposed — data validation required** · Machine Learning is **out of scope**
> Proposal date: 15 October 2026

![Python](https://img.shields.io/badge/Python-Pandas%20%7C%20NumPy-blue)
![SQL](https://img.shields.io/badge/SQL-queries-lightgrey)
![Power BI](https://img.shields.io/badge/Power%20BI-dashboards-yellow)
![Tableau](https://img.shields.io/badge/Tableau-dashboards-orange)
![Status](https://img.shields.io/badge/status-proposed-informational)

---

## Table of Contents

1. [Project Name](#1-project-name)
2. [Project Idea](#2-project-idea)
3. [Team Members](#3-team-members)
4. [Work Plan](#4-work-plan)
5. [Roles & Responsibilities](#5-roles--responsibilities)
6. [KPIs](#6-kpis)
7. [Instructor](#7-instructor)
8. [Project Files](#8-project-files)
9. [Data Sources](#9-data-sources)
10. [Risks & Limitations](#10-risks--limitations)
11. [Tools & Technologies](#11-tools--technologies)
12. [License](#12-license)

---

## 1. Project Name

**Fantasy Premier League & Football Performance Analytics**

Short name: `FPL_Data_Analysis`

---

## 2. Project Idea

Football data is abundant, but turning it into clear information that supports decisions takes organisation and analysis. FPL points alone also do not describe every aspect of a player's performance.

This project analyses English Premier League data for the **2025/26** and **2026/27** seasons to understand player and team performance. Fantasy Premier League (FPL) is the practical application: comparing player prices against their points and statistics, and proposing squads that fit a budget.

**Core principle:** every result rests on verifiable data, and every recommendation has a clear reason that can be explained and reviewed.

### Objectives

| # | Objective | Details |
|---|-----------|---------|
| 1 | **Football performance analysis** | Goals, assists, minutes played, xG, xA, and tackles / defensive contributions (only if reliable data is found) |
| 2 | **Season comparison** | 2025/26 vs 2026/27. The 2026/27 season is ongoing, so the limits of the comparison must be stated |
| 3 | **FPL analysis** | Total points, price, value for money, availability, position, gameweeks |
| 4 | **Squad recommendation dashboard** | Budget up to £100m, with multiple scenarios |

### Squad scenarios (proposed; criteria set after data inspection)

- **Balanced Squad**
- **Safer Squad** – relies on more stable indicators
- **High-Risk Squad** – chases higher returns and accepts more uncertainty
- **Value-Focused Squad** – focuses on value for money

Evaluation criteria: past points, price and value for money, minutes played and participation, available football performance indicators, and level of uncertainty.

> **Important:** recommendations do not guarantee future points. A squad with the highest historical points is not necessarily the best going forward, so the dashboard shows its criteria and limits openly.

### Scope

| In scope | Out of scope |
|----------|--------------|
| Collecting and validating data for both seasons | Machine Learning |
| Data dictionary, understanding, and cleaning | Automatic match-outcome prediction |
| Exploratory Data Analysis (EDA) | Guaranteeing a best future squad or a number of points |
| Player and team performance analysis; season comparison | Collecting every possible statistic regardless of usefulness |
| FPL points and price analysis | A full commercial application in the first phase |
| Matplotlib charts and SQL | Continuous automation before data collection is stable |
| Power BI and Tableau dashboards | |
| Feasibility study of suggested FPL squads | |
| Documenting results, limits, and data sources | |

---

## 3. Team Members

| # | Name | Role | Contact / GitHub |
|---|------|------|------------------|
| 1 | Mohamed Ahmed | _TBD_ | _TBD_ |
| 2 | Nabil Sadek | _TBD_ | _TBD_ |
| 3 | Mahmoud Sayed | _TBD_ | _TBD_ |
| 4 | Ali Ahmed | _TBD_ | _TBD_ |
| 5 | Abdelmasih Magdy | _TBD_ | _TBD_ |

---

## 4. Work Plan

### Roadmap (13 steps)

| Step | Phase | Part |
|------|-------|------|
| 1 | Business Questions | Part 1 – Python (about one week) |
| 2 | Data Sources | Part 1 |
| 3 | Data Collection & Validation | Part 1 |
| 4 | Data Understanding | Part 1 |
| 5 | Data Cleaning | Part 1 |
| 6 | Exploratory Data Analysis | Part 1 |
| 7 | Football Performance Analysis | Part 1 |
| 8 | FPL Analysis | Part 1 |
| 9 | Visualization | Part 1 |
| 10 | SQL Integration | Part 2 – expansion |
| 11 | Power BI / Tableau | Part 2 |
| 12 | Squad Recommendation Scenarios | Part 2 (depends on data completeness and agreed criteria) |
| 13 | Final Documentation | Part 2 |

### First-week Python plan

| Day | Output |
|-----|--------|
| Day 1 | Data inventory |
| Day 2 | Initial data report |
| Day 3 | Cleaned dataset |
| Day 4 | Exploratory findings |
| Day 5 | Business analysis |
| Day 6 | Visualizations |
| Day 7 | Python notebook + README |

**Priority:** a complete, well-understood Python analysis, not implementing every part of the project. If one season's data is incomplete, the scope of the first version is adjusted rather than presenting unreliable results.

### Data workflow

```
External data sources
        │
        ▼
   data/raw/                 (original copies only, never edited)
        │
        ▼
Data Understanding notebook → Data Cleaning notebook
        │
        ▼
   data/processed/
        │
        ▼
Football Analysis + FPL Analysis
        │
        ▼
 SQL Integration → Power BI / Tableau → Squad Recommendation Dashboard
```

<!-- TODO: add calendar dates / milestones once the course deadline is fixed. -->

---

## 5. Roles & Responsibilities

<!-- TODO: assign names. The deck defines the work areas but not who owns them. -->

| Role | Responsibilities | Owner |
|------|------------------|-------|
| **Project Lead / Coordinator** | Scope, timeline, supervisor communication, final report | _TBD_ |
| **Data Engineer** | Source validation, data collection, `data/raw`, database / SQL design and setup | _TBD_ |
| **Data Analyst (Python)** | Data understanding, cleaning, EDA, football and FPL analysis, notebooks | _TBD_ |
| **BI Developer** | Power BI and Tableau dashboards, squad comparison dashboard | _TBD_ |
| **Documentation & QA** | Data dictionary, README, reports, checking results and stated limits | _TBD_ |

---

## 6. KPIs

The deck does not define numeric KPIs. The ones below are **proposed from its deliverables and risks** and should be agreed with the team and instructor.

| KPI | Target (proposed) | How it is measured |
|-----|-------------------|--------------------|
| Data sources verified (opened and checked for completeness, quality, consistency) | 100% of sources used | Source checklist |
| Season coverage | Both seasons covered, or the scope reduction documented | Last gameweek and update date per source |
| Data dictionary coverage | Every column used in analysis is documented | Data dictionary vs. columns used |
| Player-ID match rate across sources | _TBD_ % (set after inspection) | Matched ÷ total players |
| First-week Python deliverables | 7 of 7 daily outputs delivered | Weekly plan checklist |
| Analytical questions answered with data | _TBD_ of the listed questions | Questions tracker |
| Dashboards delivered | At least 1 Power BI + 1 Tableau | Files in `dashboards/` |
| Squad scenarios delivered | 4 scenarios, each within £100m with its criteria shown | Dashboard review |
| Documented SQL queries | _TBD_ | Files in `sql/` |
| Reproducibility | A new team member can rerun notebooks from `data/raw` | Fresh-run test |

---

## 7. Instructor

<!-- TODO: fill in. The proposal deck does not name the instructor / supervisor. -->

- **Name:** _TBD_
- **Course / Program:** _TBD_
- **Institution:** _TBD_
- **Contact:** _TBD_

---

## 8. Project Files

Proposed structure (can be reduced at first; final file names depend on the data actually obtained):

```
FPL_Data_Analysis/
├── data/
│   ├── raw/                 # Original copies, no direct edits
│   └── processed/           # Cleaned and prepared data
├── notebooks/               # Analysis steps, code, interpretations
├── sql/                     # Table design and queries
├── visualizations/          # Charts (Matplotlib)
├── dashboards/
│   ├── power_bi/
│   └── tableau/
├── reports/                 # Documentation and results
├── .gitignore               # Keeps data/ out of the repo
├── LICENSE                  # MIT (code)
├── LICENSE-docs             # CC BY 4.0 (documentation and visuals)
└── README.md
```

**Data management rule:** document the collection date and the source of every dataset.

### Expected deliverables

- [ ] Documented dataset for both seasons
- [ ] Data dictionary
- [ ] Python notebooks
- [ ] Player and team performance analysis
- [ ] Season comparison
- [ ] FPL points and value-for-money analysis
- [ ] Documented SQL queries
- [ ] Power BI and Tableau dashboards
- [ ] FPL squad comparison dashboard
- [ ] README
- [ ] Final report with results, limitations, and recommendations

Final deliverables depend on data quality and available time. Anything that could not be done will be documented.

---

## 9. Data Sources

**No source is *Verified* yet.** Verified means opened and checked for completeness, quality, and consistency.

| ID | Source | Status | Notes |
|----|--------|--------|-------|
| A | [Historical FPL data (GitHub)](https://github.com/vaastav/Fantasy-Premier-League) | Provisionally identified | Weekly updates appear to have stopped after 2024/25, so 2025/26 and 2026/27 coverage is unconfirmed |
| B | [Current FPL API](https://fantasy.premierleague.com/api/bootstrap-static/) | Provisionally identified | Endpoint returned JSON; the fields this project needs are not yet checked |
| C | Additional football statistics (passing, defensive) | Requires further validation | No source named yet. Check availability, coverage, definitions, player matching, terms of use, and quality |

---

## 10. Risks & Limitations

| Risk | Handling |
|------|----------|
| Data completeness | Check the last gameweek and update date of every source |
| Inconsistent definitions | Data dictionary; document differences before comparing |
| Missing football statistics | Find a suitable extra source, or narrow the analytical question |
| Player identification | Stable IDs; verify matches before merging |
| Misleading comparisons | Compare equivalent periods; state the limits |
| Squad recommendations | Show reasons and uncertainty; no guaranteed results |

A statistical relationship is not automatic proof of causation. Any derived indicator will have its calculation explained.

---

## 11. Tools & Technologies

| Tool | Use |
|------|-----|
| Python + Pandas (Jupyter via Anaconda) | Collecting, cleaning, and analysing data |
| NumPy + Matplotlib | Descriptive statistics and charts |
| SQL | Organising data and running queries |
| Power BI | Interactive dashboards |
| Tableau | Interactive dashboards |

---

## 12. License

Copyright (c) 2026 Mohamed Ahmed, Nabil Sadek, Mahmoud Sayed, Ali Ahmed, Abdelmasih Magdy

This repository uses a different license for each kind of content:

| Content | Location | License |
|---------|----------|---------|
| **Code**: notebooks, scripts, SQL schema and queries | `notebooks/`, `sql/` | [MIT](LICENSE) |
| **Documentation**: reports, README, data dictionary | `reports/`, `README.md` | [CC BY 4.0](LICENSE-docs) |
| **Visuals**: charts and dashboard screenshots / PDF exports | `visualizations/`, `dashboards/` (exports) | [CC BY 4.0](LICENSE-docs) |
| **Dashboard workbooks** (`.pbix`, `.twbx`) | `dashboards/power_bi/`, `dashboards/tableau/` | Our design is CC BY 4.0, but workbooks may embed source data. Publish them only with data extracts removed. |
| **Data**: raw, processed, database files | `data/` | **No license of ours.** Data stays under the terms of its original source (see [Data Sources](#9-data-sources)). It is excluded from the repo through `.gitignore`; use the scripts to rebuild it. |

**Data attribution:** historical FPL data comes from [vaastav/Fantasy-Premier-League](https://github.com/vaastav/Fantasy-Premier-League), whose author asks for a link back. Each dataset's source URL, collection date, and terms are recorded in `data/README.md`.

**Disclaimer:** this project is an academic analysis. It is not affiliated with or endorsed by the Premier League or Fantasy Premier League, and nothing here guarantees future FPL points.

---

## Acknowledgements

- Historical FPL data: [vaastav/Fantasy-Premier-League](https://github.com/vaastav/Fantasy-Premier-League) (the author asks for a link back when the data is used)
- Official Fantasy Premier League API
