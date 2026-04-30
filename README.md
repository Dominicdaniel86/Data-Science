# Data Science Project

## How to Set Up This Project

**✅ Requirements**
Before starting, make sure you have installed:

- Python 3
- Anaconda (or Miniconda)

### Step 1 - Clone/Download the Project

```bash
git clone https://github.com/Dominicdaniel86/Data-Science.git
cd Data-Science
```

### Step 2 - Create the Conda Environment

Run this command in the project root folder (where `environment.yml` is located):

```bash
conda env create -f environment.yml
```

This will install all required dependencies automatically.

### Step 3 - Activate the Environment

```bash
conda activate data-science
```

(*The environment name needs to match the name defined inside `environment.yml`.*)

### Step 4 - Run the Project

```bash
python main.py
```

### (Optional) Step 5 - Deactivate the Environment

When you're done working:

```bash
conda deactivate
```

### How to Update the Dependencies

Whenever you update your Anaconda environment using `pip` commands like this:

```bash
conda install numpy
```

make sure to also add the dependency to the `environment.yml` file. This ensures a consistent environment for all other project members.

### How to Load Updated Dependencies

If someone updates the `environment.yml` file, run this command:

```bash
conda env update -f environment.yml --prune
```

This updates your environment safely.

Using the OxCGRT documentation to fill in the description row:

## How to read the Dataset
This table shows the different columns of our combined dataset. It includes a short description for the columns that are not self-explanatory, together with 3 example values below.

| Indicator | Group | State | Subgroup | Phase | Time Period | Time Period Label | Time Period Start Date | Time Period End Date | Value | Low CI | High CI | Confidence Interval | Quartile Range | C1M_combined_numeric | C2M_combined_numeric | C3M_combined_numeric | C4M_combined_numeric | C5M_combined_numeric | C6M_combined_numeric | C7M_combined_numeric | C8EV_combined_numeric | E1_combined_numeric | E2_combined_numeric | H1_combined_numeric | H2_combined_numeric | H3_combined_numeric | H6M_combined_numeric | H7_combined_numeric | H8M_combined_numeric | V1 (summary) | V2 (summary) | V3 (summary) | V4 (summary) | ConfirmedCases | ConfirmedDeaths | PopulationVaccinated | StringencyIndex_Average | GovernmentResponseIndex_Average | ContainmentHealthIndex_Average | EconomicSupportIndex | MajorityVaccinated |
|-----------|-------|-------|----------|-------|-------------|------------------|----------------------|---------------------|-------|--------|---------|---------------------|----------------|----------------------|----------------------|----------------------|----------------------|----------------------|----------------------|----------------------|----------------------|---------------------|---------------------|---------------------|---------------------|---------------------|----------------------|---------------------|---------------------|--------------|--------------|--------------|--------------|----------------|-----------------|----------------------|-------------------------|--------------------------------|-------------------------------|----------------------|--------------------|
| Mental health symptom | Demographic grouping | Country or territory | Specific demographic subgroup | Survey wave number | Numeric index of the time period | Human-readable date range | Start date (YYYYMMDD) | End date (YYYYMMDD) | % of subgroup reporting the indicator | Lower bound of 95% confidence interval | Upper bound of 95% confidence interval | CI range as a string | — | School closing policy (majority population, 0–3 ordinal) | Workplace closing policy (majority, 0–3) | Cancel public events policy (majority, 0–2) | Restrictions on gathering size (majority, 0–4) | Close public transport policy (majority, 0–2) | Stay at home requirements (majority, 0–3) | Restrictions on internal movement (majority, 0–2) | International travel controls (vaccinated/everyone, 0–4) | Income support policy (0–2) | Debt/contract relief for households (0–2) | Public information campaign (0–2) | Testing policy (0–3) | Contact tracing policy (0–2) | Facial coverings policy (majority, 0–4) | Vaccination policy (0–5) | Protection of elderly people (majority, 0–3) | Existence of a prioritised vaccine rollout plan (0–2) | Vaccine eligibility/availability across population groups (0–3) | Overall approach to vaccine funding (0–5) | Mandatory vaccination requirement in place for any group (0–1) | Cumulative confirmed COVID-19 cases | Cumulative confirmed COVID-19 deaths | % of population fully vaccinated (or binary proxy where data unavailable) | Average stringency of C1–C8 + H1 closure measures (0–100) | Average across all government response indicators (0–100) | Average across containment and health indicators (0–100) | Average of E1 and E2 economic support indicators (0–100) | If the majority of population is vaccinated (NV = no, V = yes) |
| Symptoms of Depressive Disorder | By Age | United States | 30 - 39 years | 1 | 1 | Apr 23 - May 5, 2020 | 20200423 | 20200505 | 25.7 | 24.1 | 27.3 | 24.1 - 27.3 | | 2.5 | 2.5 | 1.5 | 3.5 | 0.5 | 1.5 | 1.5 | 3.0 | 1.5 | 1.0 | 2.0 | 1.0 | 1.0 | 3.5 | 0.0 | 2.5 | 0.0 | 0.0 | 0.0 | 0.0 | 1051643.0 | 64448.0 | 0.0 | 72.69 | 64.58 | 64.88 | 62.5 | NV |
| Symptoms of Depressive Disorder | By Age | United States | 40 - 49 years | 1 | 1 | Apr 23 - May 5, 2020 | 20200423 | 20200505 | 24.8 | 23.3 | 26.2 | 23.3 - 26.2 | | 2.5 | 2.5 | 1.5 | 3.5 | 0.5 | 1.5 | 1.5 | 3.0 | 1.5 | 1.0 | 2.0 | 1.0 | 1.0 | 3.5 | 0.0 | 2.5 | 0.0 | 0.0 | 0.0 | 0.0 | 1051643.0 | 64448.0 | 0.0 | 72.69 | 64.58 | 64.88 | 62.5 | NV |
| Symptoms of Depressive Disorder | By Age | United States | 50 - 59 years | 1 | 1 | Apr 23 - May 5, 2020 | 20200423 | 20200505 | 23.2 | 21.5 | 25.0 | 21.5 - 25.0 | | 2.5 | 2.5 | 1.5 | 3.5 | 0.5 | 1.5 | 1.5 | 3.0 | 1.5 | 1.0 | 2.0 | 1.0 | 1.0 | 3.5 | 0.0 | 2.5 | 0.0 | 0.0 | 0.0 | 0.0 | 1051643.0 | 64448.0 | 0.0 | 72.69 | 64.58 | 64.88 | 62.5 | NV |
