# Roland Dela Rosa — Data & Analytics Portfolio

**Live portfolio:** https://rolanddelarosaph.github.io  
**GitHub:** https://github.com/rolanddelarosaph

This repository contains my personal portfolio: a place to bring together projects, practical experience, and the different ways I work with data. The projects cover the full path from collecting and preparing data to modelling it, analysing it, and presenting the results.

My work sits across **data engineering, analytics engineering, and data analytics**. I enjoy building the foundations that make data useful — pipelines, transformations, data models, and reporting workflows — while keeping sight of the questions the data is meant to answer.

The portfolio is intended to give a clear picture of that range rather than position me around only one job title.

---

## Featured projects

The projects are presented in the following order, from the most recent end-to-end platform project to the earlier warehouse and research work.

### 1. Australian Hospital Performance Analytics

An end-to-end hospital analytics project using Australian Institute of Health and Welfare (AIHW) MyHospitals data. I built a scheduled Bronze–Silver–Gold workflow in Microsoft Fabric, using API ingestion and PySpark to clean, transform, and model hospital performance data. Fabric Data Factory schedules and orchestrates the pipeline stages, while the semantic model and Power BI dashboards let users explore emergency department activity and elective surgery performance across Australian hospitals.

**Tools:** Microsoft Fabric · Fabric Data Factory · PySpark · Power BI · DAX · REST API

**Repository:** https://github.com/rolanddelarosaph/australian-hospital-performance-analytics

### 2. Philippine Food Price Analytics Pipeline

A cloud ELT project combining Philippine food-price data, PSA Consumer Price Index data, and exchange-rate information. Python handles ingestion and preparation, Snowflake provides the cloud data warehouse, and dbt organises the transformations into analytical models. Apache Airflow is used for orchestration, with Docker supporting the development environment. Python notebooks explore food-price movements, inflation, exchange-rate relationships, and time-series forecasting, while the Tableau dashboard presents market trends and regional comparisons.

**Tools:** Python · Snowflake · dbt · Apache Airflow · Astronomer Cloud · Docker · Tableau · pandas · Prophet

**Repository:** https://github.com/rolanddelarosaph/ph-food-price-pipeline  
**Tableau dashboard:** https://public.tableau.com/app/profile/roland.dela.rosa/viz/PHFoodPriceDashboard/DASHBOARD

### 3. PSA Labor Force Survey — Educational Intergenerational Mobility

My undergraduate thesis examines intergenerational mobility in the Philippines across educational, occupational, and income outcomes. This public repository focuses on the educational component. It contains the pipeline used to prepare quarterly Philippine Statistics Authority Labor Force Survey files, account for changes in survey schemas and education coding, clean and recode records, and construct parent–child household relationships for educational mobility analysis. The prepared data is used for Bayesian multilevel modelling with PyMC and Bambi to examine educational mobility and regional differences across the Philippines.

The occupational and income components are part of the broader thesis, but their analysis workflows are not included in this repository showcase as completed, reproducible components. They required additional data cleaning, organisation, and computational resources, so I have kept the public project scope focused on the educational work that is organised for presentation.

**Tools:** Python · pandas · PyMC · Bambi · ArviZ · ETL · Bayesian Multilevel Modelling

**Repository:** https://github.com/rolanddelarosaph/psa-lfs-educational-mobility-pipeline

### 4. European Fashion Retail Data Warehouse

A SQL and Python data warehouse project built around a European fashion e-commerce dataset. The workflow organises source data into Bronze, Silver, and Gold layers, applies cleaning and deduplication, and builds a dimensional model for analytical queries. The Gold layer uses a star schema, while reusable SQL queries use joins, CTEs, ranking, and window functions to answer business questions about sales, products, customers, and inventory.

**Tools:** MySQL 8.0 · Python · SQL · Stored Procedures · Star Schema · CTEs · Window Functions

**Repository:** https://github.com/rolanddelarosaph/datawarehouse-european-ecommerce

---

## Skills and tools

| Area | Technologies and methods |
|---|---|
| Programming and querying | Python, R, SQL |
| Data platforms and storage | Microsoft Fabric, Snowflake, MySQL |
| Cloud knowledge | AWS (working knowledge) |
| Data engineering | ETL / ELT, API ingestion, data pipelines, data quality checks, medallion architecture |
| Transformation and orchestration | PySpark, dbt, Microsoft Fabric Data Factory, Apache Airflow, Astronomer Cloud |
| Data modelling | Dimensional modelling, star schema, fact and dimension tables |
| Analytics and visualisation | Power BI, DAX, Tableau, pandas, NumPy, matplotlib |
| Statistical analysis | Regression, time-series forecasting, Bayesian modelling, PyMC, Bambi, ArviZ |
| Development workflow | Git, GitHub, Jupyter Notebook, Docker |

The tools listed above reflect the technologies used across the projects in this portfolio. The depth of experience varies by tool and project; the linked repositories provide the implementation details.

---

## Experience

My professional background includes client and platform support at Cognizant, customer service and business-analysis work at Amazon, and independent statistical consulting. These roles have helped me develop a practical approach to investigating problems, working with operational data, communicating findings, and building reporting solutions.

For the full work history and role details, see the **Experience** section of the live portfolio.

---

## About

I hold a **Bachelor of Science in Statistics** from Rizal Technological University. My academic training gave me a foundation in statistical reasoning, research methods, and quantitative analysis, which I apply alongside my project work in data engineering and analytics.

I graduated **Magna Cum Laude** and was a **DOST-SEI scholar**.

I am interested in opportunities across data engineering, analytics engineering, and data analytics — particularly roles where data preparation, modelling, analysis, and reporting are connected parts of the same workflow.

---

## Repository structure

```text
rolanddelarosaph.github.io/
├── index.html
├── README.md
├── .gitignore
└── images/
    ├── profile.png
    ├── aihw_architecture.png
    ├── elective_surgery_dashboard.png
    ├── emergency_department_dashboard.png
    ├── architecture food pipeline.png
    ├── ph_food_price_dashboard.png
    ├── architecture lfs.png
    ├── bayes.png
    └── architecture datawarehouse.png
```

The project detail panels and image galleries are part of `index.html`. Project source code and full technical documentation remain in their respective GitHub repositories.

---

## Run locally

This is a static website built with HTML, CSS, and vanilla JavaScript. It does not require a package manager, build step, or framework.

1. Clone the repository:

   ```bash
   git clone https://github.com/rolanddelarosaph/rolanddelarosaph.github.io.git
   ```

2. Open the project folder:

   ```bash
   cd rolanddelarosaph.github.io
   ```

3. Open `index.html` in a browser, or use a local development server:

   ```bash
   python3 -m http.server 8000
   ```

4. Visit `http://localhost:8000`.

Keep the `images/` folder beside `index.html`; the page uses relative image paths.

---

## Deployment

The portfolio is hosted with **GitHub Pages** from the repository's `main` branch. Changes pushed to `main` are published by GitHub Pages.

---

## Contact

- **Email:** roland.delarosa.ph@gmail.com
- **LinkedIn:** https://www.linkedin.com/in/roland-dela-rosa-5595713b9/
- **GitHub:** https://github.com/rolanddelarosaph
- **Tableau Public:** https://public.tableau.com/app/profile/roland.dela.rosa

---

*This portfolio is a work in progress. I update it as I build, improve, and document projects.*
