# Zillow Housing Market Forecasting & Investment Analysis

## Project Overview

This project forecasts Denver neighborhood housing prices through 2035 using multiple predictive modeling approaches. It combines real estate data from Zillow with advanced machine learning and time-series forecasting to identify investment opportunities.

## Objectives

1. Analyze historical Denver housing price trends
2. Build predictive models using multiple approaches
3. Forecast neighborhood prices to 2035
4. Identify high-ROI investment neighborhoods
5. Visualize market insights and opportunities

## Methodologies

### Models Implemented
- **Linear Regression**: Baseline price predictions
- **Deep Learning (Keras)**: Neural network models for complex patterns
- **Prophet**: Time-series specific forecasting
- **Feature Engineering**: Quarterly/yearly aggregations, one-hot encoding, cyclical features

### Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Mean Absolute Percentage Error (MAPE)

## Technologies

- Python (scikit-learn, TensorFlow/Keras, Prophet)
- Data: Zillow real estate data
- Visualization: Matplotlib, Seaborn, Plotly
- Web Framework: Flask for interactive dashboard

## Key Features

- Multi-model forecasting approach
- Neighborhood-level analysis
- Interactive Flask web application
- ROI analysis and investment ranking
- Heatmaps and growth charts
- Comparative neighborhood analysis

## Project Structure

```
03-zillow-housing-forecast/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01-exploration.ipynb
│   ├── 02-preprocessing.ipynb
│   ├── 03-modeling.ipynb
│   └── 04-forecasting.ipynb
├── scripts/
│   ├── data_processing.py
│   ├── model_training.py
│   ├── forecasting.py
│   └── analysis.py
├── app/
│   ├── flask_app.py
│   └── templates/
├── requirements.txt
└── outputs/
    ├── models/
    ├── visualizations/
    └── forecasts/
```

## Key Results

- Best performing model: [Deep Learning/Prophet]
- Most bullish neighborhood: [Neighborhood Name]
- Highest CAGR forecast: [X%]
- Predicted prices range: $[X] - $[Y] by 2035

## Getting Started

```bash
# Installation
git clone https://github.com/pkriShna-1998/data-analytics-portfolio.git
cd data-analytics-portfolio/03-zillow-housing-forecast
pip install -r requirements.txt

# Run analysis
python scripts/data_processing.py
python scripts/model_training.py
python scripts/forecasting.py

# Launch web app
python app/flask_app.py
```

## Contact
- Email: kanchan.ocpgmail.com
- LinkedIn: [linkedin.com/in/kanchan-ratan](https://www.linkedin.com/in/kanchan-ratan-a82193273)

## License
MIT License
