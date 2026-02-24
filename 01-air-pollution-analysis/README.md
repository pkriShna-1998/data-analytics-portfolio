# Global Air Pollution Data Analysis

## Project Overview

This project analyzes global air pollution data for the world's 1,000 most populated cities using the OpenWeatherMap Air Pollution API. The analysis includes automated data collection, integration with geographic and population data, statistical analysis, and interactive visualizations.

## Objectives

1. Collect real-time air pollution data from major cities worldwide
2. Analyze correlations between different pollutants
3. Identify trends and patterns in air quality
4. Visualize pollution distribution geographically
5. Rank cities by pollution levels

## Technologies Used

- **Python 3.8+**
  - Pandas & NumPy: Data manipulation and analysis
  - Matplotlib & Seaborn: Statistical visualizations
  - Plotly: Interactive dashboards and maps
  - Requests: API integration
  - SciPy: Statistical analysis

- **Data Sources**
  - OpenWeatherMap Air Pollution API
  - City population datasets
  - Geographic coordinate data

## Project Structure

```
01-air-pollution-analysis/
├── README.md
├── data/
│   ├── raw/                    # Raw data from API
│   └── processed/              # Cleaned and processed data
├── notebooks/
│   ├── 01-data-collection.ipynb
│   ├── 02-data-cleaning.ipynb
│   └── 03-analysis-visualization.ipynb
├── scripts/
│   ├── fetch_pollution_data.py
│   ├── data_processing.py
│   └── analysis.py
├── requirements.txt
└── outputs/
    ├── visualizations/         # Generated charts and maps
    └── reports/               # Analysis reports
```

## Key Findings

### Pollutants Analyzed
- **SO₂** (Sulfur Dioxide) - Industrial emissions
- **NO₂** (Nitrogen Dioxide) - Vehicle emissions
- **PM10** (Particulate Matter 10μm) - Dust and large particles
- **PM2.5** (Fine Particulate Matter) - Health-critical pollutant
- **O₃** (Ozone) - Secondary pollutant
- **CO** (Carbon Monoxide) - Combustion byproduct

### Analysis Methods
- **Descriptive Statistics**: Mean, median, standard deviation by city/region
- **Correlation Analysis**: Relationships between different pollutants
- **Regression Analysis**: Factors influencing pollution levels
- **Clustering**: Identifying cities with similar pollution profiles
- **Time Series**: Trend analysis if temporal data available

## Visualizations

1. **Geographic Maps**: World map with pollution levels by city
2. **Heatmaps**: Correlation matrix of pollutants
3. **Bar Charts**: Top/bottom polluted cities ranking
4. **Scatter Plots**: Relationships between pollutants
5. **Interactive Dashboards**: Plotly-based exploration tools
6. **Distribution Plots**: Pollution level distributions by region

## Getting Started

### Prerequisites
```bash
python 3.8 or higher
pip or conda
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/pkriShna-1998/data-analytics-portfolio.git
cd data-analytics-portfolio/01-air-pollution-analysis
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Running the Analysis

1. **Collect Data** (requires OpenWeatherMap API key):
```bash
python scripts/fetch_pollution_data.py --api-key YOUR_API_KEY
```

2. **Process Data**:
```bash
python scripts/data_processing.py
```

3. **Generate Analysis**:
```bash
python scripts/analysis.py
```

4. **View Jupyter Notebooks**:
```bash
jupyter notebook notebooks/
```

## Key Results

- **Most Polluted Cities**: [Based on average AQI]
- **Least Polluted Cities**: [Based on average AQI]
- **Strongest Pollutant Correlations**: [PM2.5 & PM10, NO₂ & SO₂]
- **Regional Patterns**: [Asia-Pacific shows highest PM2.5, Europe shows balanced pollution]

## Dependencies

See `requirements.txt` for complete list. Main packages:
- pandas>=1.3.0
- numpy>=1.21.0
- matplotlib>=3.4.0
- seaborn>=0.11.0
- plotly>=5.0.0
- requests>=2.26.0
- scipy>=1.7.0

## API Setup

To run this project, you'll need:

1. **OpenWeatherMap API Key**:
   - Sign up at https://openweathermap.org/api
   - Free tier: 60 calls/minute
   - Get Air Pollution API access

2. **Store credentials**:
   - Create `.env` file (don't commit to Git)
   - Add: `OPENWEATHER_API_KEY=your_api_key_here`

## Future Enhancements

- [ ] Machine learning models for pollution prediction
- [ ] Real-time data updates and monitoring
- [ ] Web application dashboard (Flask/Django)
- [ ] Integration with additional data sources
- [ ] Health impact assessment
- [ ] Seasonal trend analysis
- [ ] Air quality forecasting

## Contact

For questions or collaboration:
- Email: kanchan.ocpgmail.com
- LinkedIn: [linkedin.com/in/kanchan-ratan](https://www.linkedin.com/in/kanchan-ratan-a82193273)
- GitHub: [@kanchanratan1980](https://github.com/kanchanratan1980)

## License

This project is open source and available under the MIT License.
