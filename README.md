# Roland Dela Rosa — Junior Data Engineer Portfolio

**Live site:** https://rolanddelarosaph.github.io

---

## Overview

Personal portfolio website for Roland Dela Rosa, a Junior Data Engineer and final-year BS Statistics student at Rizal Technological University (DOST Undergraduate Scholar, Magna Cum Laude). Built with vanilla HTML, CSS, and JavaScript — no frameworks, no build tools, deployed via GitHub Pages.

---

## Repository Structure

```
rolanddelarosaph.github.io/
├── index.html          # Main portfolio page
├── README.md           # This file
├── .gitignore
└── images/
    ├── architecture food pipeline.png
    ├── architecture datawarehouse.png
    ├── architecture lfs.png
    ├── ph_food_price_dashboard.png
    └── bayesian_model_result.png
```

---

## Projects

### Philippine Food Price Analytics Pipeline

End-to-end cloud ELT pipeline ingesting 300K+ rows from three real data sources (WFP market prices, PSA Consumer Price Index, and a live BSP exchange rate API) into Snowflake through a Medallion Architecture. dbt handles Bronze to Silver to Gold transformations with 20 automated data quality tests. A 4-task Apache Airflow DAG on Astronomer Cloud schedules the full pipeline on the 1st of every month. Output feeds a live Tableau dashboard and two analytical notebooks covering exchange rate lag analysis and Prophet time-series forecasting.

**Stack:** Python · Snowflake · dbt · Apache Airflow · Astronomer Cloud · Tableau · Prophet

**Repository:** https://github.com/rolanddelarosaph/ph-food-price-pipeline

---

### European Fashion Retail Data Warehouse

End-to-end SQL data warehouse for a fashion retailer across six European countries. A single Python command runs the full 4-stage Medallion pipeline — Bronze loaded via LOAD DATA LOCAL INFILE, Silver cleaned through stored procedures with type casting and ROW_NUMBER() deduplication, Gold built as a star schema with foreign key constraints and indexed fact table — all wrapped in a MySQL transaction that rolls back on any failure. Includes 14 business analytics queries using window functions, CTEs, RANK(), and LAG().

**Stack:** MySQL 8.0 · Python · Stored Procedures · Star Schema · Window Functions · CTEs

**Repository:** https://github.com/rolanddelarosaph/datawarehouse-european-ecommerce

---

### PSA LFS Educational Mobility — ETL Pipeline and Bayesian Multilevel Analysis

ETL pipeline processing 11.28 million rows of PSA Labor Force Survey microdata across 48 quarterly CSV files spanning 2010 to 2024. The pipeline handles three distinct PSA column schemas and two grade coding systems introduced by the K-12 reform mid-2016 using a schema config registry in settings.py. A 12-step cleaning pipeline produces 122,591 father-son pairs fed into a Bayesian Multilevel Linear Model estimating intergenerational educational mobility across all 17 Philippine regions. Built as an undergraduate thesis at Rizal Technological University.

**Stack:** Python · PyMC · Bambi · ArviZ · pandas · ETL Pipeline

**Repository:** https://github.com/rolanddelarosaph/psa-lfs-educational-mobility-pipeline

---

## Technical Stack

| Area | Tools |
|---|---|
| Languages | Python, SQL |
| Cloud Data Warehouse | Snowflake |
| Transformation | dbt |
| Orchestration | Apache Airflow, Astronomer Cloud |
| Database | MySQL 8.0 |
| Statistical Modelling | PyMC, Bambi, ArviZ |
| Visualisation | Tableau, matplotlib, seaborn |
| Architecture Patterns | Medallion Architecture, Star Schema, ETL, ELT |

---

## Contact

**Email:** roland.delarosa.ph@gmail.com

**LinkedIn:** https://www.linkedin.com/in/roland-dela-rosa-5595713b9/

**GitHub:** https://github.com/rolanddelarosaph
