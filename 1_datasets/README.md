# Dataset

This research uses two primary datasets to explore energy consumption, generator
usage, and renewable energy adoption on construction sites in the Middle East and
Africa. These datasets support modeling and analysis of operational behaviors
and sustainability trends in the construction sector, a topic with limited prior
research.

## 1. Construction Site Energy Usage — Real Survey Dataset

This dataset contains 29 expert responses collected via a structured Google Form
shared exclusively with construction professionals. Despite its small size, this
dataset is highly valuable due to its precision, context specificity, and the
expertise of its respondents.

### Source

Collected via Google Forms distributed only to engineers and professionals
working on active construction sites.

### Method of Collection

The Google Form was designed for technical usability and analytical clarity.
All questions were formatted as multiple choice or numeric responses to ensure
ease of answering and compatibility with downstream data analysis. The form was
shared manually with vetted professionals in the Middle East and Africa.

### Structure

Each row in the dataset represents one construction site energy profile based on
professional experience.

#### Key Columns

- **`Project Type`**: Residential, Commercial, Infrastructure, etc.
- **`Country`**: Country where the project is located
- **`Average Size of the Construction Site (m²)`**: Self-reported size of the site
- **`Estimated Project Duration`**: Total expected time to completion
- **`Primary Source of Energy`**: Diesel, Grid, Solar, or Hybrid
- **`Average Daily Energy Consumption`**: Site energy use in kWh/day
- **`Peak Power Demand (kW)`**: Highest measured or estimated demand
- **`Diesel Consumption per Week`**: Fuel usage in liters
- **`Generator Sizes Used`**: Generator capacity or combinations used
- **`Monthly Generator Maintenance Cost`**: Maintenance cost in local currency
- **`Common Generator Issues`**: Predefined selection: Overheating, Noise, Leaks,etc.
- **`Considered Solar/Wind`**: Interest in renewable alternatives
- **`CO₂ Emissions Tracking`**: Whether emissions are measured
- **`Sustainability Requirements`**: Are environmental standards enforced?
- **`Role`**: Job role of the respondent (e.g., Site Engineer, Manager)

#### Additional Notes

- This is an original dataset created for this research.
- Responses reflect realistic, field-based experiences from the construction sector.
- The structure allows direct comparison across sites and simplifies statistical
  modeling.

### Flaws and Limitations

- Small sample size (n=29)
- Self-reported estimates may contain minor inaccuracies
- No third-party validation due to survey-based collection

### Dataset Recreation

This dataset is not publicly available. It was collected using a custom Google
Form. To replicate, redesign a survey targeting construction professionals using
the same structure and wording used in this project.

## 2. Synthetic Construction Site Dataset — GPT-Generated Expansion

This dataset was synthetically generated using ChatGPT to create 5,000
additional entries modeled after the original survey structure. It provides a
scalable version of the real data for deeper analysis, machine learning
experimentation, and visualization.

### Dataset Source

Generated using ChatGPT with structured prompts informed by the real dataset’s
columns and value patterns.

### Generation Prompt

> Using the structure of the original 29-entry dataset on construction site
energy usage (including fields like project type, country, energy consumption,
diesel usage, and generator specs), generate 5,000 synthetic entries. The data
should reflect realistic, domain-informed patterns that are internally
consistent and representative of construction site operations in the Middle East
and Africa. Include a range of site sizes, power sources, and maintenance behaviors.

### Method of Generation

The synthetic data simulates real-world distributions across all features using
controlled variability and predefined ranges. Multi-select responses were
modeled using weighted random logic to mirror human patterns.

### Synthetic dataset Structure

Each row represents a simulated construction site record.

#### Synthetic dataset Key Columns

- **`Project_Type`**: Simulated project category
- **`Country`**: Country where the site is located
- **`Average Daily Energy Consumption`**: Simulated kWh/day
- **`Peak Power Demand (kW)`**: Estimated peak requirement
- **`Generator_Sizes_Used`**: Randomized values like 30kVA, 100kVA, etc.
- **`Diesel Consumption per Week`**: Simulated based on site demand
- **`Renewable_Concerns`**
- **`Common_Gen_Issues`**
- **`Power_Source_Factors`**: Multi-select categories
- **`Monthly_Gen_Maintenance_Cost`**: Maintenance cost estimates
- **`Consider_Hybrid_System`**, **`Track_CO2_Emissions`**
- **`Join_Pilot_Study`**: Yes/No flags

#### Synthetic dataset Additional Notes

- Does not contain any real-world identities or confidential information.
- Suitable for training models or validating dashboard prototypes.
- Closely resembles the original dataset's layout and logic.

### Synthetic dataset Flaws and Limitations

- Fully synthetic data — not field-verified
- Model-based randomization may miss outlier behaviors
- Assumes logic applies across regions and project types uniformly

### Synthetic Dataset Recreation

To recreate this dataset, use ChatGPT or another LLM with a prompt like the one
above. Maintain the same columns and value distributions as in your real survey.

## Public Hosting of Prepared Dataset

For this milestone, we are hosting all datasets directly in this GitHub
repository. Dataset sizes are small enough for version-controlled collaboration.

our data is organized as follows:

1. **Raw Dataset**: Original form responses from the Google Form
   - Location: [`raw_datasets`](raw_dataset/raw_data.csv)

2. **Synthetic dataset**: generated synthetic dataset with formatting
   fixes
   - Location: [`synthetic_data`](raw_dataset/synthetic_data.csv)
