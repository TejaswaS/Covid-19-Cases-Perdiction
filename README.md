🦠 Global COVID-19 Data Analysis & Visualizer
A Python-based data analysis and geospatial visualization project designed to aggregate, clean, and map global COVID-19 confirmed cases across countries using interactive map visualizers.

📌 Features
Global Data Aggregation: Automatically merges and computes worldwide confirmed cases from raw, daily time-series data.

Intelligent Data Cleaning: Handles complex country naming conventions, regional subdivisions, and special character stripping (e.g., handling states, territories, and parenthetical notes).

Geographic Mapping: Maps custom country names to standard ISO Alpha-3 country codes via continent lookup datasets.

Interactive Choropleth Maps: Visualizes the global distribution and severity of infection ranges across five categorized tiers using Plotly Express.

🛠️ Tech Stack & Libraries
Data Manipulation: pandas, numpy

Geospatial & Visualization: plotly, matplotlib

Time Series / ML Ready: prophet, scikit-learn (prepared for forecasting)

📂 Project Structure & Workflow
Ingestion: Loads daily global confirmed cases and deaths dataset files.

Cleaning & Grouping: * Extracts total case counts for each unique territory/region.

Normalizes string formats by trimming territory extensions, periods, and notes.

Aggregates region-level cases up to unified country-level totals.

Data Discretization & Binning: Bins case numbers into intuitive visual categories:

U50K | 50Kto200K | 200Kto800K | 800Kto1.5M | 1.5M+

ISO Mapping & Plotting: Converts country titles to standard 3-letter ISO codes and generates an interactive Mercator choropleth map.

🚀 Getting Started
Prerequisites
Ensure you have Python installed along with the required libraries:

pip install pandas numpy matplotlib plotly prophet scikit-learn
Running the Project
Clone the repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Place the required dataset files (CONVENIENT_global_confirmed_cases.csv, CONVENIENT_global_deaths.csv, and continents2.csv) in the root directory.

Run the script:

python Code.py
