Copyright reserved @misraturp
# Pandas-Fundamentals-Secrets


## Pandas Fundamentals – Pro Secrets (Learning Notes)

### Overview

This repository contains concise notes and Python code snippets derived from the YouTube series *“Pandas Fundamentals Pro Secrets”* by Misra Turp. The objective is to strengthen core pandas skills essential for practical data analysis and preprocessing tasks.

### Topics Covered

* Core pandas objects: `DataFrame` and `Series`
* Index handling: `set_index()`, `reset_index()`, `sort_values()`
* Data transformation: `assign()`, `apply()`, vectorised operations
* Conditional data filtering: boolean masking, `isin()`, `isna()`, logical `AND`/`OR` operations

### Example Code

```python
import pandas as pd

# Sample DataFrame creation
villages = pd.DataFrame(columns=["village_name", "village_population", "taluka"],
                        data=[["gonavadi", 300, "ambegaon"],
                              ["savargaon", 250, "junnar"],
                              ["katraj", 1035, "pimpri chinchwad"]])

# Indexing and sorting
villages.set_index('village_population', inplace=True)
villages.reset_index(inplace=True)

# Feature engineering
villages['village_population_5yrs'] = villages['village_population'] * 2.5

# Conditional filtering
villages[villages['sarpanch'] == 'Male']
```

### Relevance

The material directly supports skill development for roles such as:

* Data Analyst
* Data Scientist
* Machine Learning Engineer

Proficiency in pandas is fundamental for efficient handling of structured datasets in professional data-driven environments.

### Technologies Utilised

* Python 3.x
* pandas library

