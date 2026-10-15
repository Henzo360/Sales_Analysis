# Sales Analysis and Visualization

## Project overview
This project explores 2019 retail sales data using Python and pandas. The notebook combines monthly sales files into one dataset, prepares the data for analysis, creates sales-related variables, and examines sales performance across time, cities, products, and orders.

The analysis is intended to demonstrate an end-to-end exploratory data analysis (EDA) workflow: loading multiple files, cleaning records, transforming fields, answering business questions, and communicating patterns through visualisations.

## Business questions
- How did sales vary from month to month?
- Which cities generated the highest sales value?
- Which products had the highest order quantities?
- At what hours were orders most common?
- Which products appeared together in the same order?

## Tools and libraries
- **Python** — analysis workflow
- **pandas** — loading, combining, cleaning, and aggregating tabular data
- **NumPy** — numerical operations
- **Matplotlib and Seaborn** — charts and visual exploration
- **Power BI** — a dashboard is referenced as part of the project; dashboard images are not currently included in this repository

## Data preparation
The notebook reads multiple monthly CSV files and combines them into a single dataset. During preparation, it handles blank or invalid rows and repeated header rows that can occur when files are concatenated. Date and numeric fields are converted to appropriate types so they can be grouped and analysed consistently.

A sales-value field is calculated using unit price multiplied by quantity ordered. This allows the notebook to analyse sales value separately from the number of units sold.

## Analysis performed
### Monthly sales
Sales values are grouped by month to compare performance throughout 2019.

### City-level sales
The notebook groups sales by city to examine geographic differences in sales value.

### Product demand
Product order quantities are aggregated to identify products with high demand.

### Order timing
Order timestamps are used to examine order volume by hour of day.

### Products purchased together
Order identifiers are used to explore products that occur in the same order, providing a view of common product combinations.

## Findings recorded in the notebook
The notebook reports that December had the highest monthly sales and San Francisco, California, had the highest city-level sales. It identifies AAA Batteries (4-pack) as the product with the highest quantity ordered and highlights order activity around 10:00 and 19:00. The notebook also explores product pairs, including phones and related accessories.

These findings reflect the analysis recorded in the notebook and should be interpreted in the context of the source dataset and the notebook's cleaning and aggregation logic.

## Repository contents
- `sales analysys.ipynb` — Jupyter notebook containing data preparation, analysis, and visualisations.
- `.gitignore` — Git ignore configuration.

## Running the project
1. Clone or download the repository.
2. Install the main Python dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Place the monthly source CSV files in the location expected by the notebook, or update the file path in the data-loading cell.
4. Launch Jupyter Notebook and run the notebook cells in order.

The source monthly CSV files are not currently included in this repository, so they must be supplied locally before the complete analysis can be rerun.

## Author
Henry Odionye
