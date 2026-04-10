# UK Household Income Dashboard | Power BI

## Overview
This Power BI project analyses UK household income trends and regional inequality from 2014 to 2024.

The aim was to transform inconsistent annual Excel files into a clean analytical model and build a professional dashboard suitable for executive reporting and regional drill-down analysis.

The final solution includes:
- Page 1: Executive dashboard with KPI cards and trend analysis
- Page 2: Regional comparison drill-down page

## Business Objective
This dashboard was built to answer three questions:
1. How has UK household income changed over time?
2. Which regions consistently outperform or underperform?
3. What is the size of the regional inequality gap?

## Data Preparation
The source data included:
- separate yearly Excel files
- inconsistent sheet layouts
- duplicate category labels
- blank rows and empty columns
- null numeric rows
- junk categories and malformed headers

Using Power Query, I:
- combined yearly Excel files into one master dataset
- standardised duplicate category names
- removed blank rows and empty columns
- fixed null values
- added a Year field
- appended all years into one clean fact table
- removed invalid slicer categories and structural junk rows

## Final Data Model
Fact grain:

**One row = Region × Year × Category**

Columns:
- Year
- Region
- Country
- Category
- Amount

## Dashboard Features

### Page 1 — Executive Dashboard
- KPI cards for UK average, highest region, lowest region, and regional gap
- trend line chart for long-term income analysis
- synced slicers for year and category
- executive title and subtitle layout

### Page 2 — Regional Comparison
- horizontal regional ranking chart
- dynamic title using DAX
- insight text for highest vs lowest comparison
- slicer-driven drill-down by year and category

## DAX Highlights
Measures were created for:
- highest region KPI
- lowest region KPI
- regional gap KPI
- dynamic title logic
- ranking-based comparison logic
- interaction-safe KPI behaviour

## Key Insight
The dashboard highlights persistent regional inequality in UK household income, with London and the South East often outperforming lower-income regions such as the North East.

## Skills Demonstrated
- Power BI
- Power Query
- DAX
- Data cleaning
- Data modelling
- KPI design
- Dashboard UX
- Filter context debugging
- Executive storytelling

## Files
- `UK_Household_Income_Dashboard.pbix`
- `dashboard-export.pdf`
- `dashboard-page1.png`
- `dashboard-page2.png`

## Portfolio Value
This project demonstrates an end-to-end BI workflow, from messy Excel source files through to a stakeholder-ready dashboard designed for UK Data Analyst and BI Analyst roles.
