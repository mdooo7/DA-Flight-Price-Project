# ✈️ Flight Price — Data Cleaning & KPI Analysis

![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB)
![Colab](https://img.shields.io/badge/Google%20Colab-Environment-F9AB00?logo=googlecolab&logoColor=white)

A data cleaning and analysis project on a real-world flight booking dataset — built in Google
Colab to clean messy date/time fields and answer 7 business KPIs about pricing, routes,
stops, airlines, and departure timing.

## 📑 Table of Contents
- [Tech Stack & Tools](#️-tech-stack--tools)
- [Core Workflow](#-core-workflow)
- [Key Insights](#-key-insights)
- [Repository Structure](#-repository-structure)
- [How to Run](#-how-to-run-the-notebook)

## 🛠️ Tech Stack & Tools
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn

## 🔍 Core Workflow

<details open>
<summary><strong>1. Data Cleaning</strong> — 10,683 → 10,681 rows</summary>
<br>

Handled missing values and one malformed duration entry (a stray `'5m'` value with no
matching hours), reducing the raw dataset to a fully analysis-ready one.
</details>

<details>
<summary><strong>2. Feature Engineering</strong></summary>
<br>

Parsed journey date into `DAY`/`MONTH`/`YEAR`, split departure and arrival timestamps into
hours/minutes, and converted flight duration into total minutes.
</details>

<details>
<summary><strong>3. KPI Analysis</strong> — 7 business questions</summary>
<br>

Pricing by airline, route, and stop count; flight volume by airline and airport; monthly
price trends; and average departure timing by airline.
</details>

## 📈 Key Insights

| Metric | Finding |
|---|---|
| 💺 Priciest fare class | `Jet Airways Business` — ~₹58,359 avg (distinct fare class, not a data error) |
| 🔁 Stops vs. price | ~₹5,025 (non-stop) → ~₹17,686 (4 stops) — a ~3.5x increase |
| 🛫 Priciest route | Bangalore → New Delhi (~₹11,918) |
| 💸 Cheapest route | Chennai → Kolkata (~₹4,790) |
| ✈️ Dominant carrier | Jet Airways — **~36%** of all flights |
| 🏙️ Busiest airport | Delhi — **~42%** of all departures |

## 📁 Repository Structure

```text
DA-Flight-Price-Project/
├── README.md
├── DA_Flight_Price.ipynb
└── data/
    └── flight_price.xlsx
```

## 🚀 How to Run the Notebook
1. Clone this repository (the notebook pulls `data/flight_price.xlsx` from it automatically):
   ```bash
   git clone https://github.com/mdooo7/DA-Flight-Price-Project
   ```
2. Open `DA_Flight_Price.ipynb` in Google Colab (or upload it to Colab directly).
3. Run all cells sequentially: **Runtime → Run all**.
