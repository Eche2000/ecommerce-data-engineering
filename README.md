# E-Commerce Data Engineering Lab

This project demonstrates an end-to-end 12-step data-engineering workflow using a synthetic e-commerce transaction dataset. The notebook loads raw transactions, selects suitable Python data structures, profiles data quality, applies reusable cleaning rules, transforms fields, engineers new features, enriches transactions with Ontario municipality metadata, and produces a small revenue analysis. Cleaned data is serialized to both CSV and JSON. The project is designed to run from top to bottom after the repository is cloned.

## Quick Start

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Open `notebook/data_engineering_lab.ipynb` and run all cells from top to bottom.

## Data Sources

* **Primary transactions:** Synthetic 503-row e-commerce dataset created for this lab. It includes intentional data-quality issues for cleaning practice.

* **Secondary metadata:** Curated subset of the Government of Ontario **Municipalities** open dataset, used to enrich shipping-city records and support the data dictionary. Source: https://data.ontario.ca/dataset/municipalities

## Repository Structure

```text
data/
  transactions.csv
  ontario_municipalities_subset.csv

notebook/
  data_engineering_lab.ipynb

.gitignore
README.md
requirements.txt
```

## Other Projects

* [My-NumPy-Operations](https://github.com/Eche2000/My-NumPy-Operations)
* [Anomaly_Detection](https://github.com/Eche2000/Anomaly_Detection_Lab1.git)
* [Data_Engineering_EDA Public](https://github.com/Eche2000/Data_Engineering_EDA.git)