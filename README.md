# 🚀 ELT Pipeline with dbt, Snowflake & Airflow (Cosmos)

This project demonstrates a modern ELT pipeline using:

* 🛠️ **dbt** for transformation and data modeling
* ❄️ **Snowflake** as the cloud data warehouse
* 🌬️ **Apache Airflow** (with [Cosmos by Astronomer](https://github.com/astronomer/astronomer-cosmos)) for orchestration

---

## 📊 Project Highlights

* **Data Modeling:** Implemented fact tables and data marts using dbt
* **Security:** Applied Snowflake Role-Based Access Control (RBAC)
* **Orchestration:** Used Airflow + Cosmos to manage modular dbt workflows

---

## 🧱 Stack

* **dbt-core**
* **Snowflake**
* **Apache Airflow**
* **Cosmos (Astronomer)**

---

## 📁 Suggested Folder Structure

Graphql

```python
elt-data_pipeline/
├── dags/
│   └── dbt_dag.py                # Airflow DAG using Cosmos
├── dbt/
│   └── data_pipeline/            # dbt project directory
│       ├── models/
│       ├── dbt_project.yml
│       └── ...
├── profiles/
│   └── profiles.yml              # dbt profile (optional - managed via Airflow)
├── requirements.txt
├── Dockerfile                    # Optional: containerize Airflow/dbt
├── README.md
└── .gitignore

```
