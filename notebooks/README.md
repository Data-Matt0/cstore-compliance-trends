# 🧪 Data Cleaning & Analysis – OSHA Inspections Notebook

This Jupyter notebook (`OSHA_data_project.ipynb`) contains the core data preparation and exploratory analysis for the **OSHA Convenience Store Compliance Trends** project. It prepares raw inspection-level CSV data for use in visualizations and dashboards.

---

## 🧼 What the Notebook Does

The notebook processes the raw OSHA inspection file (`osha_inspection.csv`) and produces a clean, analysis-ready subset focused on convenience stores.

### ✅ Key Data Wrangling Steps:
- **Selective column loading** for performance optimization
- **Renaming columns** for clarity and consistency
- **Type conversion** of `naics_code` and `inspection_date`
- **Filtering for NAICS 445110**, the U.S. industry code for Convenience Stores
- **Extracting year** from inspection dates for trend analysis
- **GroupBy summaries** to calculate:
  - Violations by store and state
  - Inspection frequency by year

---

## 📊 Output Preview

The notebook produces:

- `cstore_df` — filtered DataFrame of inspections at convenience stores  
- `violations_summary` — store-level violation counts  
- `annual_violations` — total inspections per year (used in trendline chart)

---

## 🛠️ Tools & Libraries

- **Python 3**  
- `pandas` – for data manipulation  
- `matplotlib` – for quick data visualizations  
- `google.colab.files` – for file upload/download within Colab

---

