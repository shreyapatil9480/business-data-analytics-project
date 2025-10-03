# Business Data Analytics Project

This repository contains a **synthetic dataset**, an **analysis notebook**, and all supporting files needed to explore and model business data.  It is intended to showcase data‐driven skills relevant to **business analysis**, **programme management** and **data analysis** roles.  The project starts with basic descriptive analysis and scales up to predictive modeling, so that the difficulty increases as you progress through the notebook.

## Contents

| File | Description |
| --- | --- |
| `synthetic_business_data.csv` | A generated dataset containing 500 weekly observations between 2019 and 2027.  Each row represents sales data for one product category in a given region and week.  Columns include the date, product category, region, units sold, revenue, cost, profit, marketing spend, customer satisfaction and month. |
| `analysis_notebook.ipynb` | A Jupyter notebook that walks through exploratory data analysis (EDA), creates visualizations, and builds predictive models.  The analysis starts with simple summary statistics, then moves to more complex charts and correlation analysis, and finally builds regression and classification models using scikit‑learn. |
| `requirements.txt` | A list of Python packages needed to run the notebook. |

## Dataset Description

The synthetic dataset mimics revenue and cost data for five product categories (`Electronics`, `Furniture`, `Clothing`, `Food`, `Office Supplies`) across four geographic regions (`North`, `South`, `East`, `West`).  Additional columns include:

- **Date** – the week of observation.
- **Units_Sold** – number of units sold during the week (drawn from a Poisson distribution).
- **Revenue** – total revenue generated (units sold × revenue per unit plus random noise).
- **Cost** – total cost incurred (units sold × cost per unit plus random noise).
- **Profit** – difference between revenue and cost.
- **Marketing_Spend** – synthetic marketing expenditure associated with the observation.
- **Customer_Satisfaction** – a random score between 50 and 100 representing customer satisfaction.
- **Month** – the month extracted from the date (useful for modelling seasonal effects).

Because it is synthetic, the dataset can be freely shared and modified.

## Getting Started

1. **Install dependencies.**  Ensure you have Python 3.8+ installed.  Install the required packages using the provided `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```

2. **Open the notebook.**  Launch Jupyter Notebook or JupyterLab and open `analysis_notebook.ipynb`:

   ```bash
   jupyter notebook
   ```

3. **Run the cells.**  Step through the notebook sequentially.  It will:
   - Load and display the dataset.
   - Compute descriptive statistics and show them in a table.
   - Create bar, line and heatmap charts to visualise revenue distribution, time series patterns and feature correlations.
   - Build a regression model to predict profit and evaluate its performance using RMSE and R².
   - Create a classification model to identify high‑profit vs low‑profit observations and report the accuracy.

## Project Structure & Difficulty

The notebook is structured so that the complexity increases as you progress:

1. **Exploratory Analysis** – loads the data and performs straightforward summaries and visualizations.
2. **Intermediate Visualisations** – examines trends over time and interactions between variables.
3. **Predictive Modelling** – introduces machine learning techniques to forecast profit and classify high-profit instances.  This section uses pipelines and preprocessing to handle categorical variables, offering a real‐world example of preparing data for models.

By working through these sections, you can demonstrate a range of analytical skills relevant to business analysis and data science roles.

## Future Extensions

This project can be extended in many ways:

- **Time‑series modelling** to predict future revenue or profit.
- **Optimization analysis** to recommend marketing spend levels that maximize profit.
- **Dashboard creation** using tools like Tableau, PowerBI or Plotly Dash for interactive reporting.

Contributions and suggestions are welcome.  Feel free to fork the repository and propose improvements via pull requests.

---

*This project was generated automatically to showcase data analysis capabilities on a synthetic business dataset.*

