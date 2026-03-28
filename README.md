# US Energy Transition: The Decline of Coal & Rise of Renewables (1973–2035)
# Project Objective
Analyzed 50+ years of US energy consumption data to identify the "Crossover Point" where renewable energy sources surpassed coal and leveraged predictive modeling to forecast the US energy mix through 2035.
# Data & Tools
Source: U.S. Energy Information Administration (EIA) - Monthly Energy Review (Table 1.3).
Tools: Microsoft Excel (Advanced).
Key Techniques: String Manipulation (Text-to-Date), ETL, Time-Series Analysis, Exponential Smoothing (ETS) Forecasting.
# The Data Engineering Process (The "How")
Extraction: Processed raw CSV data containing over 600 months of energy consumption metrics (Quadrillion BTU).
Date Transformation: Solved a "Data Trap" where dates were stored as text (e.g., "1973 January"). I used a nested formula to reconstruct the timeline: =DATEVALUE(MID(A12, 6, 20) & " 1, " & LEFT(A12, 4)).
Data Cleaning: Performed a "Data Audit" to remove annual totals and non-numerical values that would skew the trend analysis.
Predictive Modeling: Utilized the Excel Forecast Sheet (ETS Algorithm) to project consumption trends for the next decade, accounting for seasonal seasonality.
# Key Insights & Storytelling
The Great Crossover: My analysis confirms that US Renewable energy consumption officially overtook Coal in the year 2020.
Coal’s Collapse: Since its peak in 2005 - 2007, Coal consumption has plummeted by 61%, driven by shifts toward Natural Gas and Renewables.
The 2030 Horizon: Based on current historical trends, my model forecasts that Renewables will reach 0.7994674 Quadrillion BTU by 2030, a 6.6% increase from current levels.
