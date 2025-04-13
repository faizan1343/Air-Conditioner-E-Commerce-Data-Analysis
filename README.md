# Air Conditioner E-Commerce Data Analysis

This repository contains an analysis of air conditioner data scraped from an e-commerce platform (e.g., Amazon). The project focuses on data cleaning, calculating discounts, identifying duplicate listings, and basic visualizations, with plans for further analytical enhancements.

## Project Overview

The dataset (`Air Conditioners.csv`) includes 720 air conditioner listings with 9 features:
- **name**: Product name (e.g., "LG 1.5 Ton 5 Star AI DUAL Inverter Split AC")
- **main_category**: Category (appliances)
- **sub_category**: Sub-category (Air Conditioners)
- **image**: Image URL
- **link**: Product URL
- **ratings**: Customer rating (1–5)
- **no_of_ratings**: Number of reviews
- **discount_price**: Discounted price (₹)
- **actual_price**: Original price (₹)

### Current Features
- **Data Cleaning**:
  - Handle missing values in `ratings`, `no_of_ratings`, `discount_price`, and `actual_price` using mean imputation.
  - Clean price columns by removing non-numeric characters (₹, commas).
- **Analysis**:
  - Calculate `Discounted_Price` (actual - discount) and `Discount_Percentage`.
  - Identify products listed multiple times using `groupby`.
  - Compute average ratings (3.81), prices, and discounts.
- **Visualization**:
  - Styled table of duplicate products with a green gradient.
  - (Note: Scatter plot code is incomplete and requires fixing.)
- **Output**:
  - Cleaned dataset saved as CSV.
  - Summary statistics (e.g., average discount percentage: -4.13%).

### Planned Enhancements
- Fix scatter plot visualization.
- Validate and correct negative discount percentages.
- Add advanced analyses (e.g., price vs. rating correlation, clustering by features).
- Incorporate predictive modeling (e.g., price prediction).
- Create interactive dashboards with Plotly or Dash.

## Getting Started

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

Install dependencies:
```bash
pip install -r requirements.txt
