# Heath Dashboard Project

A Tableau dashboard visualization project analyzing health outcomes and prevention measures across United States counties and states.

## Overview

This dashboard provides interactive visualizations of health data for counties across the United States, allowing users to explore various health outcomes, prevention measures, and demographic information.

## Data Sources

The dashboard uses the following data:
- **Primary Dataset**: `cleaned_places_long_AA_US_only.csv`
  - Contains health data for US counties from 2021
  - Includes state, county, FIPS codes, and population data
  - Covers multiple health categories: Health Outcomes and Prevention

## Health Measures Included

The dashboard includes interactive parameters to visualize the following health measures:

### Health Outcomes
- All teeth lost among adults aged ≥65 years
- Any disability among adults
- Arthritis among adults
- Binge drinking among adults
- Cancer (non-skin) or melanoma among adults
- Chronic obstructive pulmonary disease among adults
- Cognitive disability among adults
- Coronary heart disease among adults
- Current asthma among adults
- Current cigarette smoking among adults
- Depression among adults
- Diagnosed diabetes among adults
- Fair or poor self-rated health status among adults
- Feeling socially isolated among adults
- Frequent mental distress among adults
- Frequent physical distress among adults
- Hearing disability among adults
- High blood pressure among adults
- High cholesterol among adults who have ever been screened
- Independent living disability among adults
- Lack of social and emotional support among adults
- Mobility disability among adults
- Obesity among adults
- Self-care disability among adults
- Short sleep duration among adults
- Stroke among adults
- Vision disability among adults

### Prevention Measures
- Cholesterol screening among adults
- Colorectal cancer screening among adults aged 45–75 years
- Taking medicine to control high blood pressure among adults with high blood pressure

## Data Structure

The dataset includes the following fields:
- `year`: Data year (2021)
- `state`: State abbreviation
- `state_full`: Full state name
- `county`: County name
- `fips`: FIPS code
- `category`: Health category (Health Outcomes, Prevention)
- `measure`: Specific health measure name
- `measure_id`: Measure identifier
- `data_value_type`: Type of data value (e.g., Age-adjusted prevalence)
- `data_value`: Actual data value
- `low_ci`: Lower confidence interval
- `high_ci`: Upper confidence interval
- `total_population`: Total population for the geographic area
- `total_pop_18plus`: Population aged 18 and over

## Files

- `Heath_Dashboard_Project.twbx`: Packaged Tableau workbook containing the dashboard, data extracts, and associated resources

## Tableau Features Used

This dashboard utilizes a comprehensive set of Tableau features to create an interactive and dynamic visualization:

### Core Components
- **8 Dashboards**: Multiple dashboard layouts for different views and analyses
- **34 Worksheets**: Various chart types and visualizations
- **Parameters**: Interactive parameter controls for dynamic measure selection
  - List-type parameters with multiple health measure options
  - Parameters for filtering and customizing views
- **Filters**: 46+ filters for data refinement and user interaction
- **Groups**: 380+ data groups for organizing and categorizing data

### Advanced Calculations
- **124 Calculated Fields**: Custom calculations for data transformation and analysis
- **Level of Detail (LOD) Expressions**: 
  - FIXED LOD expressions for aggregations at specific dimensions
  - Used for computing averages and percentiles by measure
- **Statistical Functions**: 
  - PERCENTILE calculations (25th, 75th percentiles)
  - AVG (Average) aggregations
  - RANK_UNIQUE for ranking counties
  - COUNTD (Count Distinct) for unique measures
- **Conditional Logic**: IF/THEN/END statements for dynamic filtering
- **String Functions**: CONTAINS for text matching and string concatenation
- **Parameter Integration**: Calculations that reference parameters for dynamic behavior

### Interactive Features
- **Dashboard Actions**: 10+ actions for interactivity between worksheets
- **Quick Filters**: Interactive filter controls on dashboards
- **Parameter Controls**: User-selectable parameters for measure selection

### Geographic Visualization
- **Maps**: Extensive use of geographic visualizations (592+ map references)
- **Geographic Roles**: State, county, and FIPS code mappings for map-based analysis

### Data Connections
- **Multiple Data Sources**: Multiple connections to the same CSV dataset for different visualization needs
- **Embedded Data Extracts**: Packaged data for offline use

## Tableau Version

- Created with Tableau version 2025.2.4 (18.1)
- Source platform: Windows

## Usage

1. Download the `.twbx` file
2. Open it with Tableau Desktop (version 18.1 or later)
3. The dashboard includes interactive parameters to select and compare different health measures
4. Explore health data by state, county, or FIPS code

## Notes

- The workbook is packaged with embedded data extracts, so no external data connections are required
- All data sources are included within the `.twbx` file
- The dashboard includes multiple data sources based on the same CSV file for different visualizations

