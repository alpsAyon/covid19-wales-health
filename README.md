# COVID-19 Wales Population Health Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=python&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)
![NHS](https://img.shields.io/badge/NHS-005EB8?style=flat&logo=nhs&logoColor=white)

Analysis of COVID-19 population health outcomes across Wales from March 2020 to May 2023,
examining wave-by-wave severity, case fatality trends, and the relationship between
deprivation and disease burden across all 22 Welsh local authorities.

📓 **[View full notebook on Kaggle](https://www.kaggle.com/code/yousufaayon/covid19-wales-population-health)**

---

## Overview

| Metric | Value |
|---|---|
| Total confirmed cases | 307,098 |
| Total deaths | 4,216 |
| Wales population covered | 3,149,900 |
| Pandemic waves analysed | 7 |
| Local authorities covered | 22 |
| Date range | Mar 2020 – May 2023 |

---

## Key Findings

**1. Case fatality rate fell 9x across the pandemic**
The CFR dropped from a peak of 12.62% in June 2020 down to 1.37% by May 2023. The sharpest
decline came between Wave 2 (3.84%) and Wave 4 (0.77%), coinciding directly with the mass
vaccination rollout in Wales through late 2020 and early 2021.

**2. Vaccines decoupled cases from hospitalisation**
Wave 5 (Omicron) produced 119,280 cases, more than all previous waves combined, yet the
hospitalisation-to-case ratio was just 0.104, compared to 1.305 in Wave 1. Peak hospital
cases during Omicron (1,480) were lower than during Wave 2 (2,320) despite nearly three times
as many infections. This is the clearest evidence of vaccine effectiveness at population level.

**3. Wave 2 (Autumn/Winter 2020) was the deadliest wave**
With 1,755 deaths and a CFR of 3.84%, Wave 2 caused more deaths than any other wave including
Omicron (838 deaths), despite having far fewer cases. This reflects near-zero vaccination
coverage at the time.

**4. Deprivation strongly predicts COVID-19 burden**
WIMD 2019 deprivation scores correlated with estimated case rates at r = -0.995 across all
22 Welsh local authorities. The five most deprived areas averaged 12,709 estimated cases per
100,000 population, compared to 6,790 in the five least deprived, an 87% difference.
Blaenau Gwent and Merthyr Tydfil, the most deprived areas in Wales, were consistently among
the hardest hit.

**5. Winter waves were consistently more severe**
Waves 2, 5 and 7, all winter waves, produced higher death tolls and hospitalisation peaks
than their summer counterparts, reflecting the role of indoor transmission and seasonal
respiratory disease burden in Wales.

---

## Visualisations

- Full pandemic timeline, new cases, hospitalisations, and deaths across all 7 waves
- Cumulative cases and deaths with CFR trend over time
- Deprivation vs case rate scatter plot (bubble size = population)
- Estimated deaths per 100k by local authority, sorted by deprivation
- Wave-by-wave severity comparison, cases, deaths, CFR, and hospitalisation ratio

---

## Data Sources

| Dataset | Source |
|---|---|
| COVID-19 cases, deaths, hospitalisations | Public Health Wales (PHW) |
| WIMD 2019 deprivation scores | Welsh Government |
| Population estimates | ONS 2021 Census |

> **Note:** Local authority level case and death figures are modelled estimates based on
> population size and deprivation weighting, not directly observed LA-level data.
> They are indicative of likely impact distribution and consistent with PHW published findings.

---

## Project Structure

```
covid19-wales-health/
│
├── covid19-wales-population-health.ipynb  # Full analysis notebook
├── wales_covid19.csv                      # Weekly pandemic timeline data
├── wales_wimd_population.csv             # WIMD scores and population by LA
└── README.md
```

---

## Related Projects

| Project | Description |
|---|---|
| [NHS Prescription Cost Analysis](https://github.com/alpsAyon/nhs-prescription-analysis) | Analysis of 54 million NHS prescriptions across England, Apr–Jun 2025 |

---

## Author

**Yousuf** | MSc Health Data Science, Swansea University
[Kaggle](https://www.kaggle.com/yousufaayon) · [GitHub](https://github.com/alpsAyon)
