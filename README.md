# SQL-Analyzing-Students-Mental-Health

## Project Overview
This project analyzes survey data from a Japanese international university using **PostgreSQL** to explore how the length of stay (`stay`) impacts the average mental health diagnostic scores of international students.

---

## Dataset & Metrics
The analysis focuses on international students (`inter_dom = 'Inter'`) and evaluates three key mental health diagnostic scores:
* **`PHQ-9` (dep)**: Measures depression severity (`average_phq`).
* **`SCS` (tosc)**: Measures social connectedness (`average_scs`).
* **`ASISS` (toas)**: Measures acculturative stress (`average_as`).

---

## Key SQL Techniques Used
* **Data Filtering**: Isolated international student data.
* **Data Aggregation**: Used `ROUND()`, `AVG()`, and `COUNT()` to compute metrics per length of stay.
* **Grouping & Sorting**: Applied `GROUP BY stay` and sorted results in descending order (`ORDER BY stay DESC`).

---

## Key Findings

Among international students with 1–4 years of stay (the groups with meaningful sample sizes), average depression scores (PHQ-9) rose from 7.48 to a peak of 9.09 at 3 years, and acculturative stress increased from 72.8 to 87.7, while social connectedness declined from 38.1 to 33.9. Groups with 5+ years of stay contain only 1–3 students and are not reliable for conclusions. This is a descriptive analysis; it shows association, not causation.

---

## Tech Stack
* **Language**: SQL (PostgreSQL)
* **Platform**: DataCamp DataLab
