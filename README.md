<div align="center">

# Ntokozo Ntombela
### Graduate Data Engineer · Microsoft Certified: Fabric Data Engineer Associate (DP-700) · ICT Honours, DUT

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ntokozo-ntombela-ba662235a)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://data-engineering-portfolio-xi.vercel.app/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ntombelan098@gmail.com)

</div>

---

## About me

I'm an ICT graduate from the Durban University of Technology (72% average, 15 distinctions) finishing my Honours in 2026. I build data pipelines in Python, SQL and PySpark, mainly on Microsoft Fabric, Azure and Databricks.

My projects focus on South African financial services: sanctions screening, POPIA-compliant data quality checks and job-market data. Each repo explains what's real, what's simulated, and what I'd improve next.

My Honours research is **"Evaluating Cost-Sensitive Machine Learning for Vehicle Insurance Fraud Detection"**.

**Looking for:** 2027 graduate, internship or junior data engineering roles in South Africa (Durban, Johannesburg or Cape Town; on-site, hybrid or remote).

---

## Featured projects

### [SA Financial Crime & Fraud Intelligence Platform](https://github.com/ntokozo078/sa-fincrime-fabric-platform)
An end-to-end **Microsoft Fabric** project modelling a FICA/AML compliance workflow on synthetic South African data.

- Bronze → Silver → Gold **Medallion lakehouse**, orchestrated with Data Factory pipelines (Bronze triggers Silver)
- **PySpark sanctions screening** of 1,000 synthetic company registrations using Levenshtein fuzzy matching
- Explainable **rule-based risk scoring** (sanctions match, company age, director count, province)
- Simulated transaction stream through **Eventstream into a KQL database**, with KQL queries for FICA threshold and velocity checks
- Power BI semantic model over the Gold tables
- Stack: `Microsoft Fabric` `PySpark` `Delta Lake` `KQL` `Eventstream` `Power BI` `Python`

### [SA Bank Data Quality & POPIA Pipeline](https://github.com/ntokozo078/SA-bank-data-quality-pipeline)
A Python data quality pipeline for synthetic SA banking transactions, also tested on the public PaySim dataset.

- SA ID validation with date, citizenship and **Luhn checksum** checks, plus cellphone, email and amount rules
- Failed records go to **quarantine with a reason** for each failed check
- **POPIA-style PII masking** with salted SHA-256, applied to quarantined and accepted records
- **8-rule fraud score**, evaluated against PaySim's fraud labels (95% recall, low precision; the README explains why)
- **3-state circuit breaker** that rejects a batch with too many bad records
- Writes accepted records to **Delta Lake**, with a Streamlit dashboard and Great Expectations checks
- Stack: `Python` `pandas` `scikit-learn` `Delta Lake` `Great Expectations` `Streamlit` `APScheduler`

### [Entry-Level Job Market Pipeline](https://github.com/ntokozo078/entry-job-market-pipeline)
An ETL pipeline that collects **real** entry-level tech job listings, with a live website and REST API.

- Extracts from **2 APIs (Adzuna, Remotive) and 1 scraper (Careers24)**: South Africa plus 6 other countries, about 220 jobs per run
- Freshness and seniority filters, then an **upsert into PostgreSQL** on source and job ID (SCD Type 1)
- Retires listings a source stops returning, with retention rules and a row cap
- Flask website, Chart.js dashboard and REST API, deployed on Render
- **Pytest suite run by GitHub Actions** on every push
- Stack: `Python` `PostgreSQL` `SQLAlchemy` `Flask` `BeautifulSoup` `pytest` `GitHub Actions`

---

## Tech stack

**Languages**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![KQL](https://img.shields.io/badge/KQL-00BCF2?style=for-the-badge&logo=microsoftazure&logoColor=white)

**Data engineering and cloud**

![Microsoft Fabric](https://img.shields.io/badge/Microsoft_Fabric-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-FDEE21?style=for-the-badge&logo=apachespark&logoColor=black)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=for-the-badge&logo=databricks&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)

**Databases**

![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Microsoft SQL Server](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)

**Analytics and ML**

![pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

**Web and tooling**

![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)

Also used in my degree: Java, C# and ASP.NET.

---

## Certifications

| Certification | Issuer | Year |
|---|---|---|
| Microsoft Certified: Fabric Data Engineer Associate (DP-700) | Microsoft | 2026 |
| Microsoft Certified: Azure Data Fundamentals (DP-900) | Microsoft | 2025 |
| Data Engineer Associate | DataCamp | 2026 |
| dbt Fundamentals | dbt Labs | 2026 |
| Databricks for Data Engineering | Databricks | 2025 |
| Databricks Fundamentals | Databricks | 2025 |
| Spark Fundamentals I | IBM | 2025 |
| SQL Intermediate | Sololearn | 2026 |
| Data Analytics Job Simulation | Quantium via Forage | 2026 |

---

<div align="center">

*Building data pipelines, and being clear about what they can and can't do yet.*

</div>
