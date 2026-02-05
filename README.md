# Food Spending Behavior Analysis: Power BI & Excel Dashboard

![Dashboard](/Images/First%20page%20.png)
![Drill](/Images//Drille%20Through%20page%20.png)

## Introduction
Southeast Asia is known for its vibrant street food culture, where diverse culinary traditions reflect the region's rich cultural history. This often translates into a preference for dining out over cooking at home. This study investigates whether this trend holds true in other regions, specifically comparing food spending behavior in Singapore and the United States.

## Objective
This project analyzes how average consumer spending on food and beverages—covering both groceries and dining out—has changed as a share of total household expenditure over the past decade in the United States and Singapore. By comparing these two countries, the analysis highlights key trends, structural differences, and economic factors influencing consumer spending behavior in each market.

## Data Sources:
### U.S. Data
- **Bureau of Labor Statistics (BLS) Consumer Expenditure Survey**


### Singapore Data
- **Department of Statistics (SingStat)**


### Inflation Data
- **World Bank**

## Data Cleaning and Preprocessing
Since the data sources varied from different websites, the templates and formats were inconsistent. This required extensive data cleaning to standardize the data. The following steps were taken:

### Standardization of Data Format:
I created new Excel files to ensure consistency across datasets. Each dataset was transformed and loaded into a standardized format to make the data easier to analyze and compare. Columns and row values were renamed to standardize datasets across all sources.

### Missing Data Handling:
During the cleaning process, I identified several missing values in the dataset. Specifically, Singapore's Average Monthly Expenditure per year along with the Food Expenditure Distribution had missing data for certain years. To handle this:
- I used the CPI- and income-adjusted interpolation method to fill in the gaps. This method estimates expenditure growth using the equation:

  `Expenditure Growth ≈ CPI Growth + α × Income Growth`

  For years where data was missing, I interpolated the values based on available information from the Consumer Price Index (CPI) and income growth trends.

### Expenditure Distribution:
For the expenditure distribution, I used the latest available year (2023) as a reference to estimate the values for previous years (2019-2022). This allowed me to maintain the relevance and accuracy of the data while ensuring no crucial information was left out.

### Ensuring Data Relevance:
I also reviewed the dataset to ensure all of the data was relevant to the analysis. Any irrelevant or redundant information was removed to maintain data quality and avoid bias in the final analysis.

## Analysis
![Main Page](/Images/First%20page%20.png)

The main dashboard is structured using a combination of card visuals and analytical charts. Card visuals highlight key country-year insights, including top food categories, top food expenditure, food-at-home and dining-out proportions, and inflation indicators. These metrics provide a concise overview of consumer food spending behavior and its evolution over time.

- **The donut chart** illustrates the proportion of total expenditure allocated to food consumption, split between food consumed at home and dining out.
- **The real food spending growth vs. real income growth chart** assesses whether food expenditure growth outpaces changes in purchasing power.
- **A combined line and clustered column chart** is used to examine the relationship between food spending growth and inflation over time.
- **The nominal vs. real food spending growth line chart** highlights the divergence between nominal growth and inflation-adjusted growth, emphasizing the impact of food inflation.

### Key Insights:
- Food-at-home consistently accounts for the majority of food expenditure in the United States; however, it is the opposite in Singapore.
- Real food spending growth lags real income growth in both countries during high-inflation periods, indicating cost-of-living pressure.
- Nominal food spending growth overstates consumption growth when inflation accelerates.
- Real food spending growth outpaced real income growth following the COVID-19 lockdown period, peaking in 2021 before gradually moderating in subsequent years.

![Drill Through](/Images/Drille%20Through%20page%20.png)

The drill-through page, which can be accessed from the main page, contains further details regarding each country’s data acquisition method, yearly growths and inflation indexes, a more detailed expenditure distribution, along with the trend of alcohol and tobacco consumption.

### Key Insights:
- Alcohol and tobacco consumption among Americans and Singaporeans has gradually declined. This may reflect positive health-related behavioral changes.

---

## 📊 Data Analysis Skills (Excel & Power BI)
- 🔄 **Data Transformation (ETL):** Cleaned, shaped, and prepared raw data using Power Query by handling missing values, correcting data types, appending datasets, and creating calculated columns.
- 📐 **Data Modeling:** Built efficient data models by defining relationships.
- 🧮 **DAX & Measures:** Created implicit and explicit measures using DAX to calculate KPIs such as averages, growth rates, percentages, rankings, and time-intelligence metrics with the help of Chat GPT.
- 📊 **Pivot Tables & Pivot Charts:** Analyzed datasets using pivot tables, slicers, and dynamic pivot charts to summarize and explore trends.
- 📉 **Data Visualization:** Designed Column, Bar, Line, Area, Donut, and Combo Charts to compare metrics and track trends over time.
- 🎛️ **Interactive Reporting:** Implemented slicers, filters, drill-through pages, and tooltips for dynamic, user-driven insights.
- 🎨 **Dashboard Design & Storytelling:** Designed intuitive, visually appealing dashboards following best practices for layout, color, and data storytelling.
- 📤 **Data Validation & Quality Checks:** Ensured data accuracy using consistency testing.

---

## Conclusion
The objective of this study was to investigate differences in food spending behavior across different regions. The findings show both similarities and differences in consumer behavior, particularly in response to the COVID-19 pandemic. Both regions exhibited similar trends in how the pandemic affected food spending. However, the average Singaporean consumer appears to be more inclined to dine out rather than cook at home. This trend has remained consistent over the years, highlighting a strong preference for dining experiences in Singapore.

Given these insights, businesses and investors looking to enter the Singaporean market should consider focusing on the restaurant industry, as consumer behavior strongly favors dining out over home-cooked meals. This recommendation may also be applicable to the Malaysian market, given similar consumer trends in the region.
