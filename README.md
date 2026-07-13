# Bike Buyers — Customer Analysis & Sales Dashboard

An interactive Excel dashboard that analyzes customer demographics to understand what drives bicycle purchase decisions, built with PivotTables, PivotCharts, and Slicers.

## Objective

To explore how factors like income, gender, commute distance, and age influence whether a customer purchases a bike, and to present the findings through a single-page interactive dashboard.

## Repository Contents

| File | Description |
|---|---|
| `Excel_Project.xlsx` | Main workbook — raw data, cleaned data, pivot tables, and dashboard |
| `README.md` | Project documentation (this file) |
| `screenshots/dashboard.png` | *(add this — see checklist below)* Preview image of the dashboard |

## Dataset

- **1,000 customer records**
- **13 attributes:** ID, Marital Status, Gender, Income, Children, Education, Occupation, Home Owner, Cars, Commute Distance, Region, Age, Purchased Bike

## Workbook Structure

**1. `bike_buyers` — Raw Data**
Unmodified source dataset as originally received.

**2. `Working Sheet` — Cleaned Data**
- Standardized values (e.g. `M` → `Married`, `F` → `Female`)
- Added a calculated **`Age Bracket`** column using a nested `IF` formula:
  ```
  =IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
  ```

**3. `Pivot Tables` — Summary Tables**
Three PivotTables built from the cleaned data:
- Average Income by Gender × Purchased Bike
- Count of Purchases by Commute Distance
- Count of Purchases by Age Bracket

**4. `Dashboard` — Interactive Report**
- PivotCharts (bar + line) visualizing the tables above
- 3 slicers for interactive filtering: **Marital Status, Education, Region**

## Key Insights

- **48.1%** of customers purchased a bike (481 of 1,000)
- Average income was **₹56,360**; male customers averaged higher income (₹58,062) than female customers (₹54,581), regardless of purchase outcome
- Customers with the **shortest commute (0–1 miles)** had both the highest purchase count (200) and the highest purchase rate, while those commuting **10+ miles** were the least likely to buy (33 of 111)
- The **"Middle Age" bracket (31–54 yrs)** made up the majority of both the overall customer base (701) and of buyers specifically (383)

## Tools & Techniques

- Microsoft Excel
  - Formulas (nested `IF`)
  - PivotTables & PivotCharts
  - Slicers for interactive, cross-filtered analysis
  - Manual data cleaning / standardization

## How to Use

1. Clone or download this repository
2. Open `Excel_Project.xlsx` in Microsoft Excel (2016+ recommended for full slicer support)
3. Go to the **Dashboard** sheet
4. Use the slicers (Marital Status, Education, Region) to filter the visuals interactively

## Dashboard Preview

*(Add a screenshot of your Dashboard sheet — see checklist below)*

```markdown
![Dashboard Preview](https://github.com/Aaravvv-git/bike-buyers--excel-dashboard/blob/main/Screenshot%202026-07-13%20195900.png)
```

## Author

**Aarav Gupta**
Production & Industrial Engineering, BIT Mesra

- LinkedIn: *(www.linkedin.com/in/aaravgupta14)*
- GitHub: *(https://github.com/Aaravvv-git)*

