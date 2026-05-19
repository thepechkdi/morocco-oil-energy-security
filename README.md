# 🇲🇦 Morocco: Global Oil Shocks & Energy Security

<div align="center">

[![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/yahyahafid/morocco-global-oil-shocks-energy-security)
[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![CI](https://img.shields.io/github/actions/workflow/status/yahyahafid/morocco-oil-energy-security/ci.yml?style=for-the-badge&label=CI)](https://github.com/yahyahafid/morocco-oil-energy-security/actions)

**An econometric and policy-driven analysis of how global oil price shocks shape Morocco's energy security, fiscal stability, and transition readiness.**

</div>

---

## Abstract

Morocco stands at a critical crossroads: a net oil importer with historically high energy subsidy burdens, facing recurrent global oil price cycles that reverberate across its trade balance, public finances, and macroeconomic stability. This project delivers a rigorous, data-driven examination of how external oil shocks — from the 2008 commodity super-cycle to the post-COVID demand surge and the 2022 Ukraine war-driven spike — have propagated through Morocco's economy. Using econometric modelling, time-series decomposition, and policy scenario analysis, the study quantifies Morocco's import dependency, maps subsidy cost trajectories, and assesses vulnerabilities in the trade balance. The analysis concludes with forward-looking policy recommendations centred on renewable energy acceleration, strategic reserve management, and structural reforms necessary for Morocco to reduce its petrostate exposure and meet its ambitious green hydrogen and solar transition targets by 2030.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Project Structure](#project-structure)
3. [Key Findings](#key-findings)
4. [Methodology](#methodology)
5. [Data Sources](#data-sources)
6. [Requirements & Installation](#requirements--installation)
7. [How to Run](#how-to-run)
8. [Outputs & Figures](#outputs--figures)
9. [License](#license)
10. [Author](#author)

---

## Project Overview

| Attribute        | Detail                                                    |
|------------------|-----------------------------------------------------------|
| **Domain**       | Energy Economics / Policy Analysis                        |
| **Geography**    | Kingdom of Morocco (MENA region context)                  |
| **Time Period**  | 2000 – 2024                                               |
| **Methods**      | Time-series analysis, OLS regression, scenario modelling  |
| **Tools**        | Python, Pandas, Statsmodels, Plotly, Scikit-learn         |
| **Notebook**     | [View on Kaggle](https://www.kaggle.com/code/yahyahafid/morocco-global-oil-shocks-energy-security) |
| **Dataset**      | [View on Kaggle Datasets](https://www.kaggle.com/datasets/yahyahafid/global-oil-shocks-and-energy-security) |

---

## Project Structure

```
morocco-oil-energy-security/
│
├── 📂 data/
│   ├── raw/                        # Original, unmodified source data
│   │   ├── brent_prices.csv
│   │   ├── morocco_imports.csv
│   │   ├── subsidy_costs.csv
│   │   └── trade_balance.csv
│   └── processed/                  # Cleaned and feature-engineered data
│       └── morocco_energy_panel.csv
│
├── 📂 notebooks/
│   └── morocco_oil_energy_security.ipynb   # Main analysis notebook
│
├── 📂 outputs/
│   ├── model_results.csv           # Regression outputs / summary tables
│   └── scenario_analysis.csv       # Policy scenario projections
│
├── 📂 figures/
│   ├── brent_price_timeline.png
│   ├── import_dependency_trend.png
│   ├── subsidy_cost_decomposition.png
│   ├── trade_balance_impact.png
│   └── energy_transition_roadmap.png
│
├── 📂 .github/
│   └── workflows/
│       └── ci.yml                  # GitHub Actions CI pipeline
│
├── .gitignore
├── requirements.txt
├── LICENSE
└── README.md
```

---

## Key Findings

> ⚠️ **Placeholder** — Fill in your actual findings after completing the analysis.

- 📌 **Finding 1 — Import Dependency:** Morocco's oil import bill represented approximately `X%` of its total goods imports over the 2010–2023 period, with peak exposure during `[year]`.

- 📌 **Finding 2 — Subsidy Burden:** A $10/barrel increase in Brent crude translates to an estimated `$X billion` increase in annual subsidy expenditure under the pre-2014 subsidy regime, equivalent to `X%` of GDP.

- 📌 **Finding 3 — Trade Balance Sensitivity:** Each 10% rise in oil prices is associated with a deterioration of Morocco's current account balance by approximately `X%` of GDP within two quarters.

- 📌 **Finding 4 — Subsidy Reform Impact:** The 2014 subsidy deindexation reform reduced fiscal exposure to oil shocks by an estimated `X%`, though second-order inflation effects on low-income households remain a structural concern.

- 📌 **Finding 5 — Transition Readiness:** Under a baseline renewable buildout scenario (20 GW solar + wind by 2030), Morocco's oil import dependency could fall to `X%`, saving an estimated `$X billion` annually at current prices.

- 📌 **Finding 6 — Policy Recommendation:** `[Summarize your top policy recommendation here]`

---

## Methodology

The analysis is structured into five analytical modules:

| Module | Description |
|--------|-------------|
| **1. Price Shock Identification** | Brent crude time-series decomposition; shock dating using Hamilton (2003) net oil price increase measure |
| **2. Import Dependency Mapping** | Energy import share of GDP and total imports; structural break detection (Zivot-Andrews) |
| **3. Subsidy Cost Modelling** | OLS regression of subsidy costs on Brent prices; counterfactual with post-2014 reform |
| **4. Trade Balance Analysis** | VAR/impulse-response analysis of oil price shocks on current account dynamics |
| **5. Scenario Projection** | Three energy transition scenarios (baseline / accelerated / delayed) with cost-benefit projections |

---

## Data Sources

| Dataset | Source | Access |
|---------|--------|--------|
| Brent Crude Oil Prices (daily) | U.S. EIA / World Bank Commodity Markets | [Kaggle Dataset](https://www.kaggle.com/datasets/yahyahafid/global-oil-shocks-and-energy-security) |
| Morocco Energy Imports & Trade Balance | World Bank World Development Indicators | Public |
| Subsidy Expenditure Data | IMF Article IV Reports / Morocco Ministry of Finance | Public |
| Renewable Energy Capacity | IRENA / MASEN | Public |
| Macroeconomic Indicators (GDP, CPI) | IMF World Economic Outlook | Public |

> All curated and preprocessed data is available via the [Kaggle Dataset](https://www.kaggle.com/datasets/yahyahafid/global-oil-shocks-and-energy-security).

---

## Requirements & Installation

### Prerequisites

- Python **3.9+**
- `pip` or `conda`
- Jupyter Notebook or JupyterLab

### Install Dependencies

Clone the repository and install all required packages:

```bash
git clone https://github.com/yahyahafid/morocco-oil-energy-security.git
cd morocco-oil-energy-security
pip install -r requirements.txt
```

### Core Libraries

| Library | Purpose |
|---------|---------|
| `pandas` | Data wrangling and time-series handling |
| `numpy` | Numerical computation |
| `matplotlib` | Static visualisation |
| `seaborn` | Statistical plots |
| `plotly` | Interactive dashboards |
| `scikit-learn` | Regression utilities and preprocessing |
| `statsmodels` | Econometric modelling (OLS, VAR, ARIMA) |
| `jupyter` | Notebook runtime |

---

## How to Run

### Option A — Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/yahyahafid/morocco-oil-energy-security.git
cd morocco-oil-energy-security

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook notebooks/morocco_oil_energy_security.ipynb
```

### Option B — Run on Kaggle (No Setup Required)

Click the badge below to open the notebook directly in Kaggle's cloud environment — zero installation needed:

[![Open in Kaggle](https://img.shields.io/badge/Open%20in-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/yahyahafid/morocco-global-oil-shocks-energy-security)

### Option C — Run on Google Colab

```
https://colab.research.google.com/github/yahyahafid/morocco-oil-energy-security/blob/main/notebooks/morocco_oil_energy_security.ipynb
```

---

## Outputs & Figures

All generated figures are saved to `/figures/` and model outputs to `/outputs/` after a full notebook run.

Key visualisations produced:

- **Brent Crude Timeline (2000–2024)** — annotated shock periods
- **Morocco Oil Import Dependency Trend** — share of GDP and imports
- **Subsidy Cost Decomposition** — pre/post reform comparison
- **Trade Balance Impulse Response** — VAR shock propagation
- **Energy Transition Scenario Comparison** — cost-benefit projections to 2030

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

```
MIT License — Copyright (c) 2024 Yahya Hafid
```

Free to use, modify, and distribute with attribution.

---

## Author

<div align="center">

**Yahya Hafid**  
*Data Scientist & AI/ML Engineer*  
Tangier, Morocco 🇲🇦

[![Kaggle](https://img.shields.io/badge/Kaggle-yahyahafid-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/yahyahafid)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Yahya%20Hafid-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yahya-h-b21805196/)

*If you found this project useful, consider leaving a ⭐ on the repo and an upvote on the Kaggle notebook!*

</div>

---

<div align="center">
<sub>Built with 🧠 Python · 📊 Data · ☀️ Renewable Energy Ambitions</sub>
</div>
