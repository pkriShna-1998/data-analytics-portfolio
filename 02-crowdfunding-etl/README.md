# Crowdfunding Data ETL Pipeline

## Project Overview

This project demonstrates the design and implementation of a robust ETL (Extract, Transform, Load) pipeline to transform raw crowdfunding data from Excel into a clean, normalized relational database. The project showcases data engineering best practices including schema design, data cleaning, and relational database implementation.

## Objectives

1. Extract raw crowdfunding data from Excel files
2. Clean and transform data (split combined fields, parse JSON)
3. Design normalized relational database schema
4. Implement referential integrity with keys
5. Load clean data into PostgreSQL database
6. Validate data quality and integrity

## Technologies Used

- **Python 3.8+**
  - Pandas & NumPy: Data manipulation
  - SQLAlchemy: ORM and database interactions
  - JSON: Data parsing

- **Database**
  - PostgreSQL: Relational database
  - pgAdmin: Database administration
  - SQL: Query language

- **Data Sources**
  - Excel files with crowdfunding campaign data
  - CSV exports

## Project Structure

```
02-crowdfunding-etl/
├── README.md
├── data/
│   ├── raw/                    # Raw Excel data
│   ├── processed/              # Cleaned CSV exports
│   └── database_schema/        # DDL scripts
├── notebooks/
│   ├── 01-data-exploration.ipynb
│   ├── 02-data-transformation.ipynb
│   └── 03-database-loading.ipynb
├── scripts/
│   ├── extract_data.py
│   ├── transform_data.py
│   ├── load_database.py
│   └── validate_data.py
├── requirements.txt
└── outputs/
    ├── data_quality_reports/
    └── database_logs/
```

## ETL Pipeline Steps

### Extract
- Read crowdfunding data from Excel/CSV files
- Initial data exploration and profiling
- Identify data quality issues

### Transform
- **Data Cleaning**:
  - Handle missing values
  - Remove duplicates
  - Standardize formats
  - Split combined fields (e.g., names into first/last)
  - Parse JSON contact information

- **Data Normalization**:
  - Create separate tables for categories, subcategories
  - Split campaigns into normalized structure
  - Establish relationships

### Load
- Create PostgreSQL database
- Execute DDL scripts for table creation
- Insert transformed data with constraints
- Verify referential integrity

## Database Schema

### Tables
1. **contacts** - Contact information
2. **category** - Campaign categories
3. **subcategory** - Campaign subcategories
4. **campaign** - Main crowdfunding campaigns

### Relationships
- campaign -> category (Many-to-One)
- campaign -> subcategory (Many-to-One)
- campaign -> contacts (One-to-One)

## Data Quality Checks

- Primary key uniqueness
- Foreign key relationships
- Data type validation
- Null value policies
- Duplicate detection
- Referential integrity
- Business rule validation

## Getting Started

### Prerequisites
```bash
python 3.8 or higher
PostgreSQL 12+
pgAdmin or PostgreSQL client
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/pkriShna-1998/data-analytics-portfolio.git
cd data-analytics-portfolio/02-crowdfunding-etl
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up PostgreSQL:
```bash
psql -U postgres -f data/database_schema/create_tables.sql
```

### Running the Pipeline

1. **Extract Data**:
```bash
python scripts/extract_data.py
```

2. **Transform Data**:
```bash
python scripts/transform_data.py
```

3. **Load to Database**:
```bash
python scripts/load_database.py
```

4. **Validate Results**:
```bash
python scripts/validate_data.py
```

## Key Results

- Successfully processed [X] campaigns
- [X] contacts extracted and standardized
- [X] categories and subcategories normalized
- Zero data integrity violations
- Complete referential integrity maintained

## Dependencies

See `requirements.txt`:
- pandas>=1.3.0
- numpy>=1.21.0
- sqlalchemy>=1.4.0
- psycopg2>=2.9.0
- openpyxl>=3.6.0 (for Excel reading)

## Future Enhancements

- [ ] Incremental data loading (CDC)
- [ ] Data validation framework
- [ ] Automated error handling and logging
- [ ] Power BI dashboard on top of data
- [ ] Performance optimization for large datasets
- [ ] Data quality monitoring

## Contact

- Email: kanchan.ocpgmail.com
- LinkedIn: [linkedin.com/in/kanchan-ratan](https://www.linkedin.com/in/kanchan-ratan-a82193273)
- GitHub: [@kanchanratan1980](https://github.com/kanchanratan1980)

## License

MIT License
