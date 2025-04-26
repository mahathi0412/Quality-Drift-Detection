# Data Quality & Drift Detection in Sales Data Using PySpark

**Data is never constant.**  
While working with different datasets, I realized that changes often happen — new fields get added, old ones disappear, data types evolve, and distributions shift.  
That's when I came across the concept of **data drifting**.

Data drift, if not detected early, can silently cause serious downstream issues:
- **Schema drift**: New columns, missing columns, datatype changes.
- **Value drift**: Changes in the distribution (mean, standard deviation) of important fields.
- **Null drift**: Increase in missing data.

This project simulates and detects such drifts — helping ensure that data remains trustworthy and reliable for analysis and business decisions.

## 🛠What I Built

I designed a **lightweight data drift detection system** that:
- Loads two batches of sales data (Batch 1 as baseline, Batch 2 with intentional drift).
- Detects:
  - Schema changes (new/missing columns, type mismatches)
  - Value distribution shifts (mean and standard deviation shifts)
  - Null value increases
- Saves findings into detailed reports (CSV and TXT formats).

## Technologies Used

| Technology | Purpose |
|:---|:---|
| **PySpark** | Handle large datasets and perform distributed data processing efficiently. |
| **Pandas** | Simplify file I/O operations (reading CSVs, saving reports). |
| **Matplotlib** | Visualize value distribution shifts between batches. |
| **Jupyter Notebook** | Easy environment for iterative development, visualization, and testing. |

## Why These Tools?

- **PySpark**: Fast, scalable, and widely used for production pipelines.
- **Pandas**: Perfect for quick manipulation and saving of smaller metadata tables.
- **Matplotlib**: Lightweight for basic drift visualizations.
- **Jupyter Notebook**: Ideal for testing logic and explaining it step-by-step.
