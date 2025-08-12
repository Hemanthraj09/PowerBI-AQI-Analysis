# Air Quality Index (AQI) Analysis Project

A comprehensive Power BI dashboard analyzing air quality data across multiple Indian cities from 2015 to 2020.

## 📊 Project Overview

This project provides detailed insights into air quality patterns across major Indian cities using historical data spanning from January 2015 to July 2020. The analysis includes various air quality parameters and their impact on the overall Air Quality Index.

## 🎯 Features

- **Multi-City Analysis**: Comprehensive air quality monitoring across major Indian cities including:
  - Ahmedabad, Delhi, Mumbai, Bengaluru, Chennai, Hyderabad, Kolkata
  - Jaipur, Chandigarh, Coimbatore, and many more
  
- **Multiple Air Quality Parameters**:
  - PM2.5 and PM10 (Particulate Matter)
  - Nitrogen compounds (NO, NO2, NOx)
  - Ammonia (NH3)
  - Carbon Monoxide (CO)
  - Sulfur Dioxide (SO2)
  - Ozone (O3)
  - Benzene, Toluene, Xylene

- **Time Series Analysis**: 5+ years of daily air quality measurements
- **AQI Classification**: Air quality categorization and bucket analysis
- **Enhanced Temporal Features**: Additional date-based attributes for improved analysis

## 📁 Project Structure

```
AQI/
├── dataset/
│   └── city_day.csv          # Cleaned dataset (29,532 records)
├── DVZ_AQI.pbix              # Power BI Dashboard (1.1MB)
└── README.md                 # Project documentation
```

## 🧹 Data Processing & Cleaning

The dataset underwent comprehensive cleaning and enhancement processes:

### Data Cleaning Steps:
- **Missing Value Treatment**: Handled null values and inconsistent data entries
- **Data Type Standardization**: Ensured proper formatting for numerical and date columns
- **Outlier Detection**: Identified and addressed anomalous air quality readings
- **Data Validation**: Cross-checked AQI calculations and parameter correlations

### Enhanced Attributes Added:
- **YearMonth**: Combined year-month attribute (e.g., "2015-01") for monthly trend analysis
- **Year**: Extracted year component for yearly comparisons
- **Month**: Month number for seasonal pattern identification
- **Month Name**: Full month names for better visualization labels
- **Season**: Categorical seasons (Winter, Summer, Monsoon, Post-Monsoon)
- **Day of Week**: Weekday analysis capabilities
- **Quarter**: Quarterly business analysis support

These additional temporal dimensions enable more granular analysis and better understanding of air quality patterns across different time periods.

## 📈 Dataset Information

- **File**: `city_day.csv`
- **Size**: 29,532 records (post-cleaning)
- **Time Period**: January 1, 2015 - July 1, 2020
- **Cities**: 26+ major Indian cities
- **Parameters**: 15+ air quality measurements per record (including derived attributes)

### Core Data Columns:
- `City`: City name
- `Date`: Measurement date (YYYY-MM-DD)
- `PM2.5`, `PM10`: Particulate matter concentrations
- `NO`, `NO2`, `NOx`: Nitrogen oxide measurements
- `NH3`: Ammonia levels
- `CO`: Carbon monoxide concentration
- `SO2`: Sulfur dioxide levels
- `O3`: Ozone concentration
- `Benzene`, `Toluene`, `Xylene`: Volatile organic compounds
- `AQI`: Air Quality Index value
- `AQI_Bucket`: AQI category classification

### Enhanced Columns (Added during preprocessing):
- `YearMonth`: Year-Month combination for trend analysis
- `Year`: Year component
- `Month`: Month number
- `Season`: Seasonal categorization
- Additional temporal attributes for comprehensive time-based analysis

## 🚀 Getting Started

### Prerequisites
- Microsoft Power BI Desktop
- Basic understanding of air quality metrics
- Knowledge of data visualization principles

### Installation
1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd AQI
   ```

2. Open the Power BI file:
   ```
   DVZ_AQI.pbix
   ```

3. The cleaned dataset is automatically linked - ensure `dataset/city_day.csv` is in the correct path.

## 📊 Dashboard Features

The Power BI dashboard (`DVZ_AQI.pbix`) leverages the cleaned and enhanced dataset to provide:

- **City-wise AQI Trends**: Compare air quality across different cities
- **Monthly/Yearly Analysis**: Enhanced temporal insights using YearMonth attributes
- **Seasonal Patterns**: Air quality variations across seasons using derived seasonal data
- **Parameter Correlation**: Relationship between different pollutants
- **AQI Distribution**: Air quality category breakdown
- **Pollution Hotspot Identification**: Cities with highest pollution levels
- **Time-based Filtering**: Advanced filtering using enhanced date attributes

## 🔍 Key Insights Enabled by Data Enhancement

- **Seasonal Pollution Trends**: Clear identification of pollution patterns across seasons
- **Monthly Comparisons**: Year-over-year monthly air quality comparisons
- **Long-term Trend Analysis**: Multi-year pollution trend identification
- **Temporal Correlation**: Understanding time-based pollution patterns
- **Enhanced Forecasting**: Better prediction capabilities with enriched temporal features

## 🛠️ Technical Specifications

- **Data Format**: CSV (Comma-separated values)
- **Visualization Tool**: Microsoft Power BI
- **File Size**: 1.1MB (Dashboard), ~2MB (Dataset)
- **Data Quality**: Professionally cleaned and validated
- **Enhancement Level**: Multiple derived attributes for comprehensive analysis
- **Update Frequency**: Historical data (2015-2020)

## 📝 Data Quality Notes

1. **Preprocessing Applied**: Dataset underwent thorough cleaning and validation
2. **Enhanced Features**: Additional temporal attributes added for better insights
3. **AQI Calculation**: Based on Indian National Air Quality Standards
4. **Geographical Scope**: Limited to major Indian cities
5. **Time Sensitivity**: Data covers pre-COVID period (ending July 2020)
6. **Derived Attributes**: YearMonth and seasonal features enable advanced analysis

## 🎨 Visualization Capabilities

The enhanced dataset supports:
- **Trend Analysis**: Using YearMonth for smooth temporal trends
- **Seasonal Decomposition**: Leveraging seasonal attributes
- **Comparative Analysis**: Year-over-year and month-over-month comparisons
- **Advanced Filtering**: Multiple temporal dimensions for detailed exploration
- **Pattern Recognition**: Enhanced temporal features reveal hidden patterns

## 🤝 Contributing

Feel free to contribute by:
- Adding new visualizations using enhanced temporal features
- Incorporating additional cities
- Extending the time period with newer data
- Further improving data quality and preprocessing
- Adding more derived attributes for analysis

## 📄 License

This project is for educational and research purposes. Please cite appropriately if used in academic work.

## 📞 Contact

For questions or collaboration opportunities, please reach out through the repository issues.

---

*Last Updated: August 2024*  
*Dashboard Version: v1.0*  
*Data Processing: Enhanced with temporal attributes and comprehensive cleaning*
