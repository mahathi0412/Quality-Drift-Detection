# Data Quality & Drift Detection in Sales Data Using PySpark

**Data is never constant.**  
As I worked more with different datasets, I noticed something important — data evolves.  
New fields appear, old ones disappear, types change, and the way values behave shifts over time.

That's when I learned about **data drifting** — a concept that explains how these small changes, if left unnoticed, can quietly break data pipelines and business decisions.

There are different types of drifts that can happen:
- **Schema drift**: The structure of the data changes (new/missing columns, type mismatches).
- **Value drift**: The pattern of data values changes (average revenue goes up, variability increases).
- **Null drift**: Missing data starts to appear more often where it wasn't expected before.

This project simulates and detects these kinds of drifts — helping ensure that data remains reliable, trustworthy, and usable for analysis.

## What I Built

I created a **simple but effective data drift detection system** that does the following:
- Generates two batches of sales data: one clean (Batch 1) and one with drift (Batch 2).
- Automatically checks for:
  - New columns, missing columns, and data type mismatches.
  - Shifts in important value distributions like revenue.
  - Unexpected increases in missing data.
- Saves the findings into clean reports (both CSV and text formats) for easy review.

The whole process feels like giving the data a "health check" — to make sure it's still in good shape over time!

## Tools and Technologies Used

| Tool | Why I Used It |
|:---|:---|
| **PySpark** | To handle large datasets quickly and process data in a distributed way (just like real-world big data projects). |
| **Pandas** | To easily read and write CSV files, and work with smaller summary tables. |
| **Matplotlib** | To visualize changes in value distributions and spot drift more easily. |
| **Jupyter Notebook** | To build and explain everything step-by-step, with live testing and visuals. |

## Why These Choices?

- **PySpark** helps simulate working at scale, even if we're starting small.
- **Pandas** makes file handling and quick analysis painless.
- **Matplotlib** makes it easier to spot shifts that aren't obvious just by reading numbers.
- **Jupyter Notebook** lets me not only build but also *tell the story* of how the data drifts over time.
