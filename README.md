# 🧾 Retail OLTP Data Pipeline

An end-to-end data pipeline project that simulates a retail OLTP system using synthetic data. It features a FastAPI-powered data generator, hourly ingestion with Databricks, data modeling with dbt on Azure Synapse, and final visualization in Tableau.

---

## 🧱 Project Stack

| Layer            | Tool/Service            |
|------------------|--------------------------|
| Data Generation  | Python, Faker, FastAPI   |
| Ingestion        | Azure Databricks         |
| Data Warehouse   | Azure Synapse Analytics  |
| Transformation   | dbt (Core or Cloud)      |
| Visualization    | Tableau                  |

---

## 🚀 Project Plan & Milestones

### ✅ Phase 1: Project Setup
- [x] Define normalized OLTP schema for a retail platform
- [x] Document schema for use in API + dbt
- [ ] Initialize GitHub repo and set up folder structure

### 🔄 Phase 2: Build Data Generator API
- [ ] Scaffold FastAPI project
- [ ] Use Faker to generate customers, products, orders, etc.
- [ ] Expose `/transactions` endpoint with hourly batch of fake data
- [ ] Deploy API to cloud (Render, Heroku, Azure)

### 💾 Phase 3: Ingest Data into Synapse
- [ ] Create Databricks notebook to call API and load to Synapse
- [ ] Schedule notebook to run every hour
- [ ] Confirm records land in `raw` schema

### 🛠️ Phase 4: Model Data with dbt
- [ ] Set up dbt project connected to Synapse
- [ ] Create staging models (`stg_`)
- [ ] Create fact/dim models (e.g. `fct_sales`, `dim_customer`)
- [ ] Add tests + documentation

### 📊 Phase 5: Visualize in Tableau
- [ ] Connect Tableau to Synapse
- [ ] Build sales dashboards: revenue, top customers, categories
- [ ] Add filters and publish dashboard

---

## 📁 Folder Structure (Planned)

```
retail-oltp-data-pipeline/
├── api/                  # FastAPI + Faker project
├── databricks/           # Notebooks for ingestion
├── dbt/                  # dbt transformation project
├── tableau/              # Tableau workbook & exports
├── docs/                 # ERDs, diagrams, and setup notes
├── README.md
```

---

## 🧠 Goals

- Simulate a real-world retail OLTP system
- Practice full-stack analytics engineering
- Showcase cloud + API + BI integration in a single project
- Build something portfolio-worthy and scalable

---

## 📬 Contact

Project maintained by **Damilare Abolaji**  
If you have questions or suggestions, feel free to open an issue or reach out.
