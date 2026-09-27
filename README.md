# DecodeLabs Project 1 — Data Cleaning & EDA (Excel)

**Internship:** HexSoftwares / DecodeLabs — Data Analyst

## Dataset
E-commerce Orders Dataset — 16,505+ rows

## Tools Used
Microsoft Excel, Power Query Editor, Pivot Tables, Pie Charts

## Problems Found in Raw Data
- Date column displaying as `########` (column-width/formatting issue)
- NULL values and empty rows
- Duplicate OrderIDs
- Inconsistent text in `PaymentMethod` and `OrderStatus`
- Missing `TotalSales` calculation

## Cleaning Steps (Change Log)

| Change | Reason | Timestamp |
|---|---|---|
| Load CSV | Initial data load | 9/10/2026 |
| Cleaned NULLs | Removed empty rows | 9/10/2026 22:00 |
| Added Column | Created `TotalSales = Quantity * UnitPrice` | 9/10/2026 22:00 |
| Created Pivots | Revenue by Product & Revenue by Referral Source | 9/10/2026 22:09 |

## Key Insights (from Pivot Tables)

**Revenue by Referral Source:**

| Source | Revenue |
|---|---|
| Instagram | 108,240.78 *(highest)* |
| Email | 100,147.67 |
| Google | 95,567.23 |
| Facebook | 93,189.60 |
| Referral | 91,608.62 *(lowest)* |
| **Grand Total** | **488,759.90** |

- Instagram drove the highest revenue among referral sources at 108,240.78.
- Referral had the lowest at 91,608.62.

## Repo Files
- `Raw_Data.xlsx` — original, unedited data
- `DecodeLabs_Project1_Cleaned.xlsx`
  - **Sheet1** — Raw data
  - **Sheet2** — Cleaned data (dates fixed, duplicates removed, NULLs cleaned)
  - **Change_Log** — all cleaning steps documented
  - **Sheet3** — Pivot Table + Pie Chart for revenue analysis

## Final Outcome
Cleaned all 16,505 rows and added a `TotalSales` column. Data is now ready for SQL analysis — used in Project 3 as `database.db`.
