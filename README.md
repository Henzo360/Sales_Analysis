# Sales Analysis and Visualisation

## Project overview

This project combines monthly retail transaction CSV files and analyses revenue, city-level performance, order timing, product demand, and products purchased together.

## Tools

- Python
- pandas and NumPy
- Matplotlib
- Jupyter Notebook

## Repository contents

- `sales analysys.ipynb` — data preparation and analysis workflow.
- `requirements.txt` — Python dependencies.
- Monthly `Sales_*.csv` source files — included at the repository root; the notebook also supports `data/Sales_Data/`.
- `output/` — generated cleaned data and summary tables.

## Workflow

1. Load monthly CSV files and combine them into one dataframe.
2. Validate required columns, remove repeated header rows, parse dates and numeric fields, and report invalid rows.
3. Calculate transaction revenue as quantity ordered multiplied by unit price.
4. Compare revenue by month and city/state.
5. Count unique orders by hour, summarise product demand and revenue, and identify product pairs co-occurring in the same order.
6. Export cleaned data and summary tables under `output/`.

## Interpretation notes

- The hourly analysis counts unique orders, not revenue. A higher order count does not necessarily imply higher revenue.
- Product co-occurrence describes products appearing in the same order; it does not establish causation.
- City/state extraction assumes the source address uses a comma-separated street, city, and state/postal-code format.
- The notebook reports invalid or missing required values and excludes those rows from the core analysis.

## How to run

1. Install dependencies with `python -m pip install -r requirements.txt`.
2. Keep the included `Sales_*.csv` monthly files in the repository root, or place them in `data/Sales_Data/`. Expected fields include `Order ID`, `Product`, `Quantity Ordered`, `Price Each`, `Order Date`, and `Purchase Address`.
3. Open `sales analysys.ipynb` in Jupyter and run cells from top to bottom.

The notebook creates `output/` and saves the cleaned dataset and summary tables there.

## Limitations

The monthly CSV files included here are the input data for this analysis. Results may differ if you replace them with another version of the dataset. This is descriptive analysis and does not establish causes for observed differences.

## Author

Henry Odionye
