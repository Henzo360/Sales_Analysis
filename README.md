# Sales Analysis and Visualization

## Project overview
Exploratory analysis of a store's 2019 electronics sales data using Python. The project combines monthly CSV files, cleans the resulting dataset, investigates sales patterns, and translates the findings into recommendations for merchandising, inventory planning, and promotion timing.

## Business questions
- Which months and cities generated the highest sales?
- Which products sold most frequently, and which contributed high sales value?
- At what times of day were orders most common?
- Which products appeared together in the same order?
- How can these findings inform inventory and marketing decisions?

## Tools
- Python
- pandas and NumPy for data preparation and analysis
- Matplotlib and Seaborn for visualisation
- Power BI for a dashboard (add a dashboard screenshot to this repository to make it viewable here)

## Workflow
1. Combined monthly CSV files into one dataset.
2. Removed invalid/blank rows and repeated header rows introduced during file concatenation.
3. Converted date and numeric fields to suitable data types.
4. Created a sales-value field from quantity ordered multiplied by unit price.
5. Analysed sales by month, city, hour, and product.
6. Examined products that appeared in the same order and visualised selected findings.

## Findings reported in the notebook
- December had the highest monthly sales.
- San Francisco, California, was reported as the highest-sales city.
- AAA Batteries (4-pack) had the highest quantity ordered in the analysis.
- The notebook identified order activity peaks around 10:00 and 19:00.
- Product-pair analysis highlighted phones and related accessories appearing in the same orders.

These are descriptive findings from this dataset, not proof that promotions at those times will cause higher sales. Validate the results against the cleaned data before using them for business decisions.

## Recommendations
- Plan inventory and fulfilment capacity ahead of the December peak.
- Compare city-level performance with marketing spend, margins, and customer counts before reallocating budget.
- Test promotion timing using controlled experiments rather than relying on order volume alone.
- Review frequently co-purchased products when designing bundles or cross-sell placements.

## Repository contents
- `sales analysys.ipynb` — analysis notebook.

## How to run
1. Clone or download this repository.
2. Install the required Python libraries: `pip install pandas numpy matplotlib seaborn`.
3. Place the source monthly CSV files in the location expected by the notebook, or update the notebook's file path.
4. Run the notebook from top to bottom.

The source sales CSV files are not currently listed in this repository, so you must supply them locally before rerunning the analysis.

## Next improvements
- Add the dataset source and licensing/usage details.
- Add a data dictionary and a short data-quality summary.
- Add exported charts and a Power BI dashboard screenshot under an `images/` folder.
- Report exact revenue totals and product/city rankings from the cleaned dataset.
- Replace hard-coded file paths with a relative project path.

## Author
Henry Odionye
