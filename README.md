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

## Tech Stack
* **Language**: SQL (PostgreSQL)
* **Platform**: DataCamp DataLab
