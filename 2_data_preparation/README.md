# 2_data_preparation

This folder contains cleaned datasets
and an initial country-level merge
for further analysis.

## Files

- `survey_clean.csv`:
  - cleaned survey responses
  - headers normalized, text cleaned, PII removed.  
- `costs_clean.csv` :
  - cleaned generator and renewable system pricing data
  - headers normalized, numeric columns standardized in AED.  
- `merged_projects_plus_costs.csv`:
  - survey data combined with country-level median cost information.  
- `survey_clean_schema.json`:
  - schema summary of the cleaned survey dataset.  
- `costs_clean_schema.json`:
  - schema summary of the cleaned costs dataset.  
- `merged_schema.json`:
  - schema summary of the merged dataset.  

## Notes

- All currency fields are represented in **AED**.  
- Category and range values are preserved in their original form.  
- The merge is performed at the **country level**
  using median values from the cost dataset.  
- These datasets will be used for exploration and modeling in subsequent steps.
