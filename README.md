# Sales Performance Dashboard – Tableau Project

## Project Overview

A comprehensive Tableau dashboard analyzing U.S. retail sales performance across multiple dimensions including time periods, market segments, product categories, and geographic regions. This interactive dashboard enables stakeholders to explore sales trends, analyze returns impact, and evaluate regional manager performance through dynamic filtering and comparative analytics.
![Sales Dashboard](https://github.com/user-attachments/assets/fd76ff3e-85ff-420f-9a35-468ef36b71b3)

## Business Objective

To provide actionable insights into sales performance by creating a dynamic, user-friendly dashboard that:
- Compares current year (CY) vs. previous year (PY) performance metrics
- Identifies trends across segments, categories, and regions
- Analyzes return rates and their impact on profitability
- Attributes performance to individual regional managers
- Supports data-driven decision making for sales leadership

## Dataset Overview

**Primary Data Source**: `Sales Data.xls`

### Data Structure:
- **Orders Table**: Core transactional data including order dates, regions, products, quantities, sales amounts, and profit margins
- **People Table**: Regional manager assignments and contact information
- **Returns Table**: Returned order tracking with binary flags for return status analysis

### Key Metrics:
- Sales Revenue
- Profit Margins
- Quantity Sold
- Return Rates
- Geographic Distribution
- Temporal Trends

## Technical Implementation

### Data Preparation Pipeline:
1. **Power Query Transformation**:
   - Standardized date formats to `mm-dd-yyyy`
   - Data quality checks and validation
   - Column standardization and cleansing

2. **Tableau Data Source Configuration**:
   - Applied filter: `Country/Region = United States` (excluded Canada)
   - Established data relationships between tables

3. **Data Modeling**:
   - **Primary Join**: `Orders.Region = People.Region`
   - **Secondary Join**: `Orders.Order ID` (left join) `Returns.Order ID`

4. **Validation & QA**:
   - SQL queries for KPI verification
   - Python scripts for data sanity checks
   - Cross-validation of calculated fields

## Dashboard Architecture

### Core Worksheets:

## Tableau Worksheet Screenshots

To view the visualizations created in Tableau for this project, please refer to the screenshots available at the following link:
[View Tableau Worksheets](https://github.com/gbadrain/us-sales-performance-tableau/tree/main/Worsksheet%20Screen%20shots)

These screenshots showcase the key dashboards and visual analyses designed in Tableau to explore U.S. sales performance across categories, regions, and time periods. They highlight KPIs, trend lines, and interactive filters that were part of the original workbook.


#### Performance KPIs:
- **Sales KPI**: Current vs. previous year sales comparison
- **Profit KPI**: Profitability analysis with return adjustments
- **Quantity KPI**: Volume metrics and trends

#### Trend Analysis:
- **Sales Sparkline**: Monthly sales trajectory visualization
- **Profit Sparkline**: Profit trend analysis over time
- **Quantity Sparkline**: Volume pattern identification

#### Geographic & Segmentation Views:
- **Sales & Profit by State**: State-level performance mapping
- **Average Sales/Profit by State**: Normalized regional comparisons
- **Monthly Sales by Segment**: Segment performance over time

#### Leadership Analytics:
- **Total Sales by Location & Manager**: Manager performance attribution
- **Region-wise Sales**: Regional performance breakdown

### Dashboard Variants:
- **Sales Dashboard**: Complete analytical view with full filter controls
- **Sales Dashboard LIGHT**: Executive summary with key insights only

## Key Features

### Interactive Controls:
- **Temporal Filters**: Year-over-year selection
- **Segmentation**: Customer segment filtering
- **Leadership**: Manager-specific performance views
- **Geographic**: Regional and state-level filtering

### Advanced Analytics:
- **Comparative Analysis**: Automated CY vs PY calculations
- **Return Impact**: Integrated return rate analysis in profit calculations
- **Dynamic Visualizations**: Context-aware charts that adapt to filter selections
- **Performance Attribution**: Individual manager performance tracking

### User Experience:
- **Responsive Design**: Optimized for different screen sizes
- **Intuitive Navigation**: Clear visual hierarchy and filter placement
- **Export Capabilities**: Data and visualization export options

## Project Structure

```
Sales-Performance-Dashboard/
├── data/
│   └── Sales Data.xls           # Raw source dataset
├── tableau/
│   └── Sales Dashboard.twbx     # Packaged Tableau workbook
├── documentation/
│   └── README.md                # Project documentation
└── validation/
├── sql_queries/                 # Data validation scripts
└── python_scripts/              # QA and analysis scripts
└── Worksheet Screen shots     # Collection of screenshots of Tableau Sheets
```

## Business Impact

### Decision Support Capabilities:
- **Strategic Planning**: Year-over-year performance trends inform future strategy
- **Operational Efficiency**: Return analysis identifies process improvement opportunities
- **Resource Allocation**: Regional performance guides investment decisions
- **Performance Management**: Manager-level insights support HR and sales operations

### Stakeholder Value:
- **Sales Leadership**: Comprehensive performance overview with drill-down capabilities
- **Operations Teams**: Detailed segment and regional analysis
- **Executive Leadership**: High-level KPI monitoring and trend identification
- **Regional Managers**: Individual performance tracking and benchmarking

## Technical Achievements

- **Data Integration**: Successfully merged multiple data sources with proper relationship modeling
- **Performance Optimization**: Efficient calculations and visualizations for responsive user experience
- **Scalability**: Framework designed to accommodate additional data sources and metrics
- **User-Centric Design**: Intuitive interface balancing analytical depth with usability

## Future Enhancements

- **Predictive Analytics**: Integration of forecasting models
- **Real-time Data**: Live data connection capabilities
- **Mobile Optimization**: Enhanced mobile dashboard experience
- **Advanced Segmentation**: Customer lifetime value and cohort analysis

## Contact & Support

**Gurpreet Singh Badrain**  
*Market Research Analyst & Aspiring Data Analyst*

- **My portfolio**: [Data Guru](https://datascienceportfol.io/gbadrain)
- **GitHub**: [gbadrain](https://github.com/gbadrain)
- **LinkedIn**: [gurpreet-badrain](http://linkedin.com/in/gurpreet-badrain-b258a0219)
- **Email**: gbadrain@gmail.com
- **Streamlit**: [gbadrain-Machine Learnning](https://gbadrain-machine-learning.streamlit.app)
- **Tableau**: [gurpreet.badrain](https://public.tableau.com/app/profile/gurpreet.badrain/vizzes)

## **Support gratitude**  
**Copilot AI** provided valuable assistance.  
Subscriber Youtube : **datatutorials1**


## Show Your Support

If you found this project helpful, please consider giving it a star on GitHub!

---

*This project demonstrates advanced data visualization skills, business intelligence acumen, and the ability to transform raw data into actionable insights for enterprise decision-making.*
