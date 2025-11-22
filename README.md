# End-to-End ELT Pipeline using Airflow, dbt, and Snowflake

![Pipeline](screens%20of%20work/pipeline.png)

This project demonstrates a complete **End-to-End ELT pipeline** using:

- **Airflow** (Orchestration)
- **dbt** (Transformations & Modeling)
- **Snowflake** (Data Warehouse)
- **Docker** (Full Environment Setup)

The goal is to simulate a **real production-grade workflow** followed by Data Engineers.

---

## 🚀 Project Overview

The pipeline follows a clean ELT structure:

1. **Extract**: Raw data loaded into Snowflake (manually or via scripts).
2. **Load**: Data is ingested into Snowflake staging layers.
3. **Transform**: dbt applies business logic → staging → intermediate → marts.
4. **Orchestrate**: Airflow triggers `dbt run` and `dbt test`.

---

## ❄️ Snowflake Setup

Screenshots from Snowflake during the setup and loading phase:

![Snowflake](screens%20of%20work/snowflake.png)

---

## 📦 dbt Project

Your dbt project includes:

- `models/`
- `tests/`
- `snapshots/`
- `macros/`

Example screenshot of dbt running:

![dbt](screens%20of%20work/dbt.png)

### 📊 dbt Lineage Graph

![Lineage](screens%20of%20work/lineage_graph.png)

---

## 🧱 Folder Structure

