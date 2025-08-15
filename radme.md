# London Bikes Data Analysis 🚴‍♂️

A comprehensive data analysis project examining London's bike sharing system patterns and trends from 2015-2017.

## 📊 Project Overview

This project analyzes bike sharing data from London to uncover insights about usage patterns, weather impacts, and seasonal trends. The dataset contains hourly bike sharing counts along with weather and temporal information.

## 🗂️ Dataset Information

The dataset contains **17,414 records** with the following features:

| Column | Description | Type |
|--------|-------------|------|
| `timestamp` | Date and time (hourly intervals) | datetime |
| `cnt` | Count of bike rentals | integer |
| `t1` | Real temperature in Celsius | float |
| `t2` | Feels-like temperature in Celsius | float |
| `hum` | Humidity (normalized 0-1) | float |
| `wind_speed` | Wind speed | float |
| `weather_code` | Weather condition category | string |
| `is_holiday` | Holiday indicator (0/1) | float |
| `is_weekend` | Weekend indicator (0/1) | float |
| `season` | Season category | string |

## 🌤️ Weather Categories

- **Clear**: Clear skies
- **Scattered clouds**: Partly cloudy
- **Broken Clouds**: Mostly cloudy
- **Cloudy**: Overcast
- **Rain**: Rainy conditions
- **Rain with thunderstorm**: Stormy weather
- **Snowfall**: Snow conditions

## 🔧 Data Processing

The analysis includes several data cleaning and transformation steps:

1. **Humidity Normalization**: Converted humidity values from percentage (0-100) to decimal (0-1)
2. **Categorical Mapping**: 
   - Mapped numeric season codes to descriptive names
   - Mapped weather codes to descriptive weather conditions
3. **Data Type Optimization**: Converted categorical columns to appropriate string types
4. **Export Preparation**: Cleaned dataset exported to Excel format

## 📈 Key Findings

Based on the initial data exploration:

- **Dataset Size**: 17,414 hourly records spanning 2015-2017
- **Weather Distribution**: 
  - Clear weather: 35.3% of records
  - Scattered clouds: 23.2%
  - Broken clouds: 20.4%
  - Rain: 12.3%
- **Seasonal Balance**: Relatively even distribution across all four seasons
- **Data Quality**: Complete dataset with no missing values

## 🔍 Analysis Opportunities

This cleaned dataset enables various analyses:

- 📊 **Temporal Patterns**: Hourly, daily, and seasonal usage trends
- 🌦️ **Weather Impact**: How different weather conditions affect bike usage
- 📅 **Holiday/Weekend Effects**: Usage patterns during special periods
- 🌡️ **Temperature Correlation**: Relationship between temperature and bike rentals
- 💨 **Weather Severity**: Impact of humidity and wind speed on usage

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **Jupyter Notebook**: Interactive development environment
- **Excel**: Data export and sharing
