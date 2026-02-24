# Quality Management KPI & Statistical Process Control (SPC) System

## Project Overview

Comprehensive quality analytics system tracking manufacturing defects, supplier quality metrics, and process capability across 12 production facilities. This system enabled proactive quality management, reduced defects, and improved supplier performance significantly.

## Business Impact

- **25% reduction in defect rates** within 6 months
- **Identified 8 critical process issues** requiring immediate intervention
- **Supplier quality improvements**: Average DPPM reduced from 4,200 to 1,200  
- **45% faster quality issue escalation** through automated alerts
- **Process capability improved from Cpk 0.8 to 1.67** (Six Sigma capable)
- **12 production facilities monitored** with real-time KPI dashboards

## Technical Stack

- **Languages:** Python, SQL
- **Statistical Analysis:** SPC, control charts, Cpk/Ppk calculations
- **Data Pipeline:** Pandas, NumPy
- **Visualization:** Plotly interactive dashboards
- **BI Tools:** Power BI quality scorecard
- **Database:** SQL Server with quality metrics

## Quality Metrics Tracked

### Product Quality
- Defect rates by product line, shift, operator
- First Pass Yield (FPY) - percentage of items produced without defects
- Critical defect trending and root cause analysis
- Scrap and rework rates

### Supplier Quality
- AQL (Acceptable Quality Level) monitoring
- DPPM (Defects Per Million) tracking
- Supplier certification status
- Incoming inspection results

### Process Control
- Statistical Process Control (SPC) with control charts
- Control limit violations and out-of-control alerts
- Process capability analysis (Cpk/Ppk)
- Trend analysis and forecasting

## Project Structure

```
07-quality-kpi-system/
├── README.md
├── notebooks/
│   ├── 01_quality_data_exploration.ipynb
│   ├── 02_spc_analysis.ipynb
│   └── 03_supplier_quality_analysis.ipynb
├── src/
│   ├── data_collectors/
│   │   ├── defect_collector.py
│   │   ├── supplier_quality_collector.py
│   │   └── process_data_collector.py
│   ├── analyzers/
│   │   ├── spc_analyzer.py
│   │   ├── capability_analyzer.py
│   │   └── trend_analyzer.py
│   └── reporters/
│       ├── quality_dashboard.py
│       ├── spc_chartmaker.py
│       └── alert_generator.py
├── data/
│   ├── sample_defect_data.csv
│   ├── supplier_quality_data.csv
│   └── process_measurements.csv
└── requirements.txt
```

## Key Features

### Quality Monitoring
- Automated daily data collection from QMS
- Real-time defect tracking and alerting
- Facility-level and product-level dashboards
- Historical trend analysis

### Statistical Analysis
- Control chart generation (X-bar, R, P charts)
- Process capability calculations (Cpk, Ppk, Cpu, Cpl)
- Outlier detection and root cause flagging
- Hypothesis testing for quality improvements

### Alerting System
- Out-of-control point detection
- Run rules violations (e.g., 4/5 points beyond 1-sigma)
- Trend detection (8 consecutive up/down points)
- Email alerts to quality teams
- SLA breach notifications

## Installation

```bash
pip install -r requirements.txt
python -m src.data_collectors.defect_collector
python -m src.analyzers.spc_analyzer
```

## Data Sources

- Quality Management System (QMS) database
- Receiving inspection records
- Production defect reports
- Supplier quality certifications

## Results Achieved

The quality KPI system successfully:
- Consolidated quality data from 12 facilities
- Created automated SPC charts and alerts
- Identified critical process deviations immediately
- Supported Six Sigma and continuous improvement initiatives
- Reduced defect rates by 25% in 6 months
- Improved supplier quality by 70% (DPPM reduction)
- Enabled fact-based quality decisions

## Key Dashboards

1. **Quality KPI Dashboard** - Overall facility performance
2. **SPC Control Charts** - Real-time process monitoring
3. **Supplier Quality Scorecard** - Vendor performance tracking
4. **Defect Analysis** - Root cause and trending
5. **Process Capability Report** - Cpk/Ppk metrics

## Next Steps

- Implement predictive quality models using machine learning
- Add automated root cause analysis using historical defect patterns
- Expand to include customer complaint integration
- Build mobile app for shop floor quality visibility
- Implement IoT sensor integration for in-process measurements
- Develop Six Sigma project tracking dashboard
