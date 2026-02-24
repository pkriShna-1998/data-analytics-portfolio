# Airbnb Revenue vs. Home Price - ROI Payback Analysis

## Project Overview

This project quantifies short-term rental investment potential by analyzing Airbnb listing data and comparing rental revenue against home ownership costs. Using large-scale ETL with Dask, the analysis identifies neighborhoods with the best return-on-investment for Airbnb property investment.

## Objectives

1. Extract and clean Airbnb listing data (Denver)
2. Integrate with Zillow 2024 neighborhood home prices
3. Calculate rental revenue under multiple occupancy scenarios
4. Compare rental income vs. home purchase costs
5. Rank neighborhoods by investment potential
6. Calculate payback periods for investment recovery

## Analysis Components

### Data Sources
- Airbnb listings: price, available days, reviews
- Zillow data: neighborhood home prices (2024)
- Market data: vacancy rates, seasonal trends

### Revenue Scenarios
- **100% Occupancy**: Maximum theoretical revenue
- **70% Occupancy**: Realistic moderate scenario
- **50% Occupancy**: Conservative scenario

### Key Metrics
- Annual rental revenue
- Operating costs (property mgmt, utilities, maintenance)
- Net rental income
- ROI percentage
- Payback period (years)
- Breakeven analysis

## Technologies

- **Python**: Data processing and analysis
- **Dask**: Large-scale distributed ETL
- **Pandas & NumPy**: Data manipulation
- **SQL**: Database queries
- **Plotly & Matplotlib**: Visualizations

## Project Structure

```
04-airbnb-roi-analysis/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01-data-extraction.ipynb
│   ├── 02-etl-pipeline.ipynb
│   └── 03-roi-analysis.ipynb
├── scripts/
│   ├── extract_airbnb.py
│   ├── etl_pipeline.py
│   ├── roi_calculation.py
│   └── analysis.py
├── requirements.txt
└── outputs/
    ├── roi_rankings/
    └── visualizations/
```

## Key Findings

- **Best Neighborhoods**: [Top 5 neighborhoods by ROI]
- **Highest Revenue Potential**: [Neighborhoods with best revenue]
- **Shortest Payback Period**: [X years for best performers]
- **Average Annual Revenue**: $[X] per property
- **ROI Range**: X% - Y% across neighborhoods

## Methodology

### Step 1: Extract Data
- Scrape/import Airbnb listings
- Get Zillow home prices by neighborhood
- Collect market data

### Step 2: Transform with Dask
- Clean and deduplicate listings
- Calculate average nightly rates
- Aggregate by neighborhood
- Merge datasets

### Step 3: Revenue Calculation
- Calculate annual revenue per occupancy level
- Factor in seasonal variations
- Estimate operating expenses
- Compute net income

### Step 4: ROI Analysis
- Compare rental income vs. home price
- Calculate payback periods
- Rank neighborhoods
- Generate visualizations

## Getting Started

```bash
# Installation
git clone https://github.com/pkriShna-1998/data-analytics-portfolio.git
cd data-analytics-portfolio/04-airbnb-roi-analysis
pip install -r requirements.txt

# Run analysis
python scripts/extract_airbnb.py
python scripts/etl_pipeline.py
python scripts/roi_calculation.py
python scripts/analysis.py
```

## Key Results

Detailed ROI rankings and payback period analysis by Denver neighborhood with investment recommendations.

## Contact
- Email: kanchan.ocpgmail.com
- LinkedIn: [linkedin.com/in/kanchan-ratan](https://www.linkedin.com/in/kanchan-ratan-a82193273)

## License
MIT License
