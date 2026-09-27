# 🚗 Electric Vehicle Sales Analysis - PowerBI 
As part of the Codebasics Data Analytics Course Unguided Project 


## 📝 Problem Statement

AtliQ Motors, a prominent automotive leader from the USA specializing in electric vehicles, has seen its market share in North America's electric and hybrid vehicle segment grow to 25% over the past five years. As part of its global expansion, the company aims to introduce its top-selling models in India, where its current market share is below 2%. To support this initiative, AtliQ Motors conducted an in-depth study of the existing EV and hybrid vehicle market in India.

## 📋 Task List

As a data analyst, I was provided with sample data and a PDF containing primary and secondary business questions. My task was to complete the following:

- Develop metrics based on the primary and secondary questions provided by the business stakeholders.
- Create a dashboard following the stakeholder mock-up, ensuring it is self-explanatory and easy to understand.
- Generate additional insights beyond the provided metrics and mock-up. I could incorporate additional data from my own research to support my recommendations.

## 🗄 Dataset Understanding

Understanding the available data is crucial before analysis. Here's a breakdown:

- Dimension Table: Contains static data related to dates and fiscal years.
- Fact Table: Includes electric vehicle sales data from manufacturers and states.

#### dim_date

- 🌍 date: Ranges from April 1, 2021, to March 1, 2024.
- 👥 fiscal_year: Since the company's fiscal year starts in April, the fiscal years listed are from 2022 to 2024.
- 📅 quarter: Corresponds to the fiscal years' quarters.


#### Electric Vehicle Sales by State

- 🗓 Date: The date on which the data was recorded (Format: DD-MMM-YY). Data is recorded monthly.
- 🏙 State: The name of the state where the sales data is recorded, representing the geographical location within India.
- 🚗 vehicle_category: Indicates whether the vehicle is a 2-Wheeler or a 4-Wheeler.
- 🔋 electric_vehicles_sold: The number of electric vehicles sold in the specified state and category on the given date.
- 📊 total_vehicles_sold: The total number of vehicles (both electric and non-electric) sold in the specified state and category on the given date.

#### Electric Vehicle Sales by Makers

- 🗓 Date: The date on which the sales data was recorded (Format: DD-MMM-YY). Data is recorded monthly.
- 🚗 Vehicle Category: Indicates whether the vehicle is a 2-Wheeler or a 4-Wheeler.
- 🏭 Maker: The name of the manufacturer or brand of the electric vehicle.
- 🔋 Electric Vehicles Sold: The number of electric vehicles sold by the specified maker in the given category on the given date.

## 🧠 Additional Calculated Metrics:

🚗 Penetration Rate: This metric represents the percentage of total vehicles that are electric within a specific region or category, indicating the adoption level of electric vehicles. It is calculated as:

$$
\text{PenetrationRate} = \left(\frac{\text{ElectricVehiclesSold}}{\text{TotalVehiclesSold}}\right) \times 100
$$

📈 CAGR (Compound Annual Growth Rate): CAGR measures the average annual growth rate over a specified period longer than one year. It is calculated as:

$$
\text{CAGR} = \left(\frac{\text{LastYearEVSales}}{\text{FirstYearEVSales}}\right)^{\frac{1}{\text{NumberOfYears}}} - 1
$$

🔄 Penetration Rate Change from 2022 to 2024:

- Absolute Change - Subtracting one value from another gives the absolute change, providing a straightforward comparison in percentage points. It is calculated as:
  $$
AbsoluteChange = PenetrationRate_{2024} - PenetrationRate_{2022}
$$

- Relative Change - Dividing one value by the other gives the relative change, offering insight into how significant the change is compared to the initial value. It is calculated as:

$$
\left(\frac{PenetrationRate_{2024} - PenetrationRate_{2022}}{PenetrationRate_{2022}}\right) \times 100
$$

## 📥 Importing Data into PowerBI

Three Excel files were imported directly into Power BI. Additional datasets, such as charging data, were later added through the same method.

## 🗂 Data Model

<p align="center">
    <img src='https://github.com/Sourav-Git01/EV_Sales_Analysis_PowerBi/blob/57d954122bf88856b7edc80c76aa126ad1f8300e/Resources/EV%20Data%20Modelling.png' height="400">
</p>
 

## 📊 Home Page

<p align="center">
    <img src='https://github.com/Sourav-Git01/EV_Sales_Analysis_PowerBi/blob/57d954122bf88856b7edc80c76aa126ad1f8300e/Resources/Home%20View.gif' width="600">
</p>

## 🏭 Makers Page

<p align="center">
    <img src='https://github.com/Sourav-Git01/EV_Sales_Analysis_PowerBi/blob/57d954122bf88856b7edc80c76aa126ad1f8300e/Resources/Maker%20Analysis.gif' width="600">
</p>

## 🏙 States Page

<p align="center">
    <img src='https://github.com/Sourav-Git01/EV_Sales_Analysis_PowerBi/blob/57d954122bf88856b7edc80c76aa126ad1f8300e/Resources/State%20Analysis.gif' width="600">
</p>

## 🎓 Learnings from this Project 

- Created a new type of bar chart visual (Horizontal Bar chart with labels above), useful for various analysis purposes.
- Implemented dynamic ranking (top/bottom filtration with Top-N Slicer) on the Sales by Makers page and Sales by State pages.
- Categorized the measures into folders and subfolders and provided proper documentation for each measure.
- The electric vehicle market in India is witnessing rapid growth, with 31% increase in CY 2024 against Previous Year 2023.
- EVs made up 6.5% of total vehicle sales last year, with the Electric 2W segment leading at 56% of all EV sales in CY2023, highlighting the growing EV market share in India.
- In terms of YoY sales growth, the electric car segment saw the highest growth rate of 116% in 2023.
- Utilized bookmarks and selection for various purposes, such as page navigation.
- Adopted a color palette for consistency throughout the dashboard ([Color palette link](https://coolors.co/palette/386641-6a994e-a7c957-f2e8cf-bc4749)).

