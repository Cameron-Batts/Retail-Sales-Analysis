# Retail Sales Aggregation and Store-Type Comparison
**Cameron Batts**

## Problem
Turn department-level sales into comparable store-week summaries using validated joins and pandas aggregation.

## Approach
Read 421,570 department-week records and 45 store records, exclude holiday observations, validate the many-to-one store join, and sum sales by Store, Date and Type. Compare average store-week sales across store types.

## Results
Recomputed nonholiday averages were $1,369,654.70 for Type A, $816,921.64 for Type B and $472,741.57 for Type C. The overall average was $1,041,256.38 across observed nonholiday store-weeks. These are descriptive differences, not causal effects of store type.

## Limitations
Holiday weeks are excluded, so these figures do not describe full-year sales. Store size, location, department coverage and other confounders are not controlled. Negative sales records are retained. No forecasting, causal estimation or sales uplift was demonstrated.

## Data
Data/sales.csv and Data/stores.csv are included. Dates are day/month/year. The original repository did not document an upstream source or redistribution license; provenance remains unverified.

## Verification
Included-data code cells executed successfully during this update.

## Run
```bash
python -m pip install -r requirements.txt
jupyter lab
```
Open [the notebook](Notebook/retail_sales_analysis.ipynb) and run cells in order. Dependencies are unpinned.

## Files
- [Analysis report](Reports/retail_sales_analysis.html)
- [Original PDF](Report/retail_sales_analysis.pdf): historical export; may predate corrections.
- [Live portfolio report](https://cameron-batts.github.io/retail_sales_analysis.html)
