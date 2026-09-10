# Flight Price — Data Cleaning & KPI Analysis

An end-to-end data cleaning and analysis project on a real-world flight booking dataset —
built in Google Colab to clean messy date/time fields and answer 7 business KPIs about
pricing, routes, stops, airlines, and departure timing.

## 🛠️ Tech Stack & Tools
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn

## 🔍 Core Workflow
1. **Data Cleaning:** Handled missing values and one malformed duration entry, reducing
   10,683 raw listings to 10,681 clean rows.
2. **Feature Engineering:** Parsed journey date into `DAY`/`MONTH`/`YEAR`, split departure
   and arrival timestamps into hours/minutes, and converted flight duration into total minutes.
3. **KPI Analysis:** Answered 7 targeted business questions — pricing by airline, route,
   and stop count; flight volume by airline and airport; monthly price trends; and average
   departure timing by airline.

## 📈 Key Insights
- `Jet Airways Business` averages ~₹58,359 per ticket — a distinct fare class, not a data error.
- Price rises steadily with each stop: ~₹5,025 (non-stop) → ~₹17,686 (4 stops), a ~3.5x increase.
- Bangalore → New Delhi is the priciest route (~₹11,918); Chennai → Kolkata the cheapest (~₹4,790).
- Jet Airways accounts for ~36% of all flights in the dataset — the dominant carrier.
- Delhi is the busiest source airport, handling ~42% of all departures.

## 🚀 How to Run the Notebook
1. Clone this repository (the notebook pulls `data/flight_price.xlsx` from it automatically):
   git clone https://github.com/mdooo7/DA-Flight-Price-Project
2. Open `DA_Flight_Price.ipynb` in Google Colab (or upload it to Colab directly).
3. Run all cells sequentially: **Runtime → Run all**.
