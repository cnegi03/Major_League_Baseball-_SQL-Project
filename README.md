# Major_League_Baseball_SQL_Project
Advanced SQL quering techniques to track how player statistics have changed over time and across different teams in the league

# ⚾ Major League Baseball (MLB) Advanced SQL Analytics Project

This project demonstrates how SQL can be used to perform real-world analytical problem solving on large relational datasets using Major League Baseball (MLB) historical data.

The analysis focuses on player development, team spending behavior, and career progression using advanced SQL techniques commonly required in Data Analyst and Business Analyst roles.

---

## 🚀 Why This Project Matters

Sports analytics closely mirrors real business analytics problems:

- Large datasets spanning multiple decades  
- Complex table relationships  
- Trend analysis over time  
- Ranking and segmentation problems  
- Financial and workforce analysis  

This project applies SQL exactly the way it is used in professional analytics teams.

---

## 📌 Business Questions Answered

### 🏫 School & Talent Pipeline Analysis
- How many schools have produced MLB players by decade?
- Which schools consistently produce the most professional players?
- What are the top 3 talent-producing schools in each decade?

---

### 💰 Team Salary & Financial Analysis
- How much do teams spend annually on player salaries?
- Which teams fall into the top 20% of average spending?
- How has cumulative payroll grown over time?
- In which year did each team exceed **$1 billion** in total spending?

---

### 👤 Player Career Analytics
- What age do players typically debut and retire?
- Which players had the longest MLB careers?
- Which team did players start and end their careers with?
- How many players remained with the same team for over 10 years?

---

### 🔍 Player Comparison & Trend Analysis
- Which players share the same birthday?
- What percentage of players bat right-handed, left-handed, or both?
- How have average height and weight at debut changed by decade?
- What are the decade-over-decade physical trends in MLB players?

---

## 📁 Project Structure

Major_League_Baseball-_SQL-Project/
│
├── README.md
│
└── sql/
└── final_project_solutions.sql


---

## 🧰 Tools & Technologies

- SQL (MySQL)
- Relational Databases
- GitHub

---

## 📊 Dataset Overview

The database contains historical MLB data including:

- **players** — demographics, debut and final game dates
- **schools** — player educational background
- **school_details** — full school metadata
- **salaries** — yearly salary data by team and player

Database used:

```sql
maven_advanced_sql

SQL Skills Demonstrated

This project demonstrates strong command over:

Common Table Expressions (CTEs)

Advanced window functions:

ROW_NUMBER()

NTILE()

LAG()

Rolling SUM()

Multi-table JOINs

Financial aggregations

Ranking & segmentation logic

Date & time calculations

Conditional aggregation (pivoting)

Business-driven SQL analysis

🔍 Sample Query
SELECT
    teamID,
    yearID,
    ROUND(
        SUM(total_spend) OVER (
            PARTITION BY teamID
            ORDER BY yearID
        ) / 1000000, 1
    ) AS cumulative_spend_millions
FROM salaries;

How to Run the Project

Import MLB datasets into MySQL.

Create the database:
sql

CREATE DATABASE maven_advanced_sql;
USE maven_advanced_sql;

Execute the SQL script:
final_project_solutions.sql
Run each section independently to view insights.

## 📈 Key Outcomes

Identified long-term salary inflation trends across MLB teams

Highlighted elite schools producing professional players

Quantified player longevity and career stability

Revealed physical evolution of athletes across decades

Demonstrated SQL-driven analytical decision making

🎯 Skills Demonstrated for Employers

✔ Advanced SQL querying
✔ Analytical thinking
✔ Business problem translation
✔ Trend & cohort analysis
✔ Data storytelling using SQL
✔ Large dataset handling

👤 Author

Charu Negi
MBA – Business Analytics

GitHub: https://github.com/cnegi03

⭐ If you find this project useful, please consider starring the repository.




