# Nashville Housing Market Analysis (2013-2016)

## Project Overview
This data analytics project transforms a raw municipal property-sales export of 56,636 rows into a fully cleaned, validated, and interactive Excel decision tool. The final workbook contains dynamic KPIs, multi-dimensional pivot tables, and a filter-aware dashboard designed to help stakeholders identify market trends, seasonal demand, and value concentrations across the Nashville area[cite: 1].

---

## Key Deliverables & Insights
*   **Data Scale & Peak Activity:** Successfully parsed 56,468 verified unique transactions after comprehensive data cleaning[cite: 1]. Market volume surged by 52.0% in dollar volume from 2013 to a peak of $6.71B in 2015[cite: 1].
*   **Geographic Concentration:** Nashville proper heavily dominates the dataset, accounting for $14.73B (roughly 80%) of the total $18.50B market value[cite: 1].
*   **Market Segments:** The region is predominantly a mid-market economy, with 32,826 sales falling comfortably within the $100K–$300K price band[cite: 1].
*   **Clear Seasonality:** Sales activity consistently spikes during the spring and summer months, reaching an explicit annual peak in June[cite: 1].

---

## Skills & Technical Methods Demonstrated

### 1. Data Cleaning & Engineering
*   **De-duplication:** Identified and safely removed 168 exact-duplicate transactions matching on multiple spatial and financial keys[cite: 1].
*   **Missing Value Guarding:** Formulated a strategy to handle 30,619 missing assessor records by mapping them as "N/A" to prevent structural skews in price tiering[cite: 1].
*   **Feature Engineering:** Converted raw Excel serial numbers into standard date formats and isolated discrete SaleYear and SaleMonth data columns[cite: 1].

### 2. Advanced Formulas & Lookups
*   **Dynamic Matching:** Utilized VLOOKUP (with approximate match for numeric tiering), XLOOKUP, and INDEX/MATCH combinations to dynamically fetch contextual data attributes[cite: 1].
*   **Conditional Aggregation:** Conducted descriptive analytics using localized SUMIFS, COUNTIFS, and AVERAGEIFS functions[cite: 1].
*   **Interactive Architecture:** Built a filter-aware calculation backend using SUBTOTAL and SUMPRODUCT arrays to ensure live visual recalculations[cite: 1].

### 3. Data Visualization & Dashboarding
*   Constructed nine multi-dimensional pivot tables tracking historical volumes, vacancy ratios, and geographic price averages[cite: 1].
*   Engineered a full Interactive Dashboard Layout featuring an optimized 2x3 chart grid, dynamic KPI blocks, and cross-filtering slicers (Year, City, Vacancy Status, and Price Category)[cite: 1].

---

## Dashboard Matrix Reference

### Key Performance Indicators (KPIs)
| Metric | Dataset Value |
| :--- | :--- |
| **Total Sales Value** | $18,497,820,434 |
| **Average Sale Price** | $327,581 |
| **Median Sale Price** | $205,838 |
| **Total Property Count** | 56,468 |
| **% Sold Vacant** | 8.6% |

### Historical Market Evolution
| Year | Transaction Count | Total Sales Value |
| :--- | :--- | :--- |
| **2013** | 11,338 | $2,783,758,501 |
| **2014** | 14,281 | $4,772,768,472 |
| **2015** | 16,794 | $6,708,760,110 |
| **2016** | 14,055 | $4,232,533,351 |

---

## Business Recommendations
1. **Target Logistics & Inventory:** Prioritize marketing capital and broker inventory towards Nashville and Antioch—these two hubs drive the majority of transaction volume[cite: 1].
2. **Capitalize on Seasonality:** Line up fresh property listings for late spring to directly capture the peak consumer demand window between May and August[cite: 1].
3. **Risk Management:** Closely evaluate the slight volume softening observed in 2016 before executing aggressive, unhedged property acquisitions[cite: 1].

---

## Repository Structure
```text
├── Data/
│   ├── raw_nashville_housing.csv      # Original uncleaned 56,636-row dataset
│   └── cleaned_sales_master.csv       # Post-validation export (56,468 rows)
├── Workbook/
│   └── nashville_analysis_tool.xlsx   # Core Excel workbook including dashboard page
└── README.md                          # Project narrative & portfolio brief
