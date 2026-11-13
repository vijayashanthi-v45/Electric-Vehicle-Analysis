# Data Cleaning Log — Electric Vehicle Registration Analysis

## Dataset Overview

- Source: Electric Vehicle registration dataset provided for the GROWAI internship project
- Initial records: **289,564**
- Initial columns: **16**
- Duplicate records: **0**
- Missing values: Found in **8 columns**
- Zero values in `Electric Range`: **188,456**

## Cleaning Steps

| Issue | Action Taken |
|---|---|
| 727 missing values in `Legislative District` | Filled using the column median to retain records. |
| 16 missing values in `Vehicle Location` | Replaced with `Unknown` because the actual coordinates were unavailable. |
| 10 missing values in `Electric Range` | Filled using the column median, which was 0. |
| 9 missing values each in `County`, `City`, and `Electric Utility` | Replaced with `Unknown` because the actual information was unavailable. |
| 9 missing values each in `Postal Code` and `2020 Census Tract` | Filled using the respective column medians to retain records. |
| Duplicate records | Checked for duplicates; none were found. |
| Geographic coordinates | Extracted latitude and longitude from the `Vehicle Location` field. |
| VIN values | Created a numeric label using factorization of the existing `VIN (1-10)` values. |

## Why Were These Missing Value Methods Used?

**Categorical columns:** Missing values in County, City, Vehicle Location, and Electric Utility were replaced with `Unknown` because the actual information was unavailable. This avoids assigning incorrect categories.

**Numeric columns:** Median values were used for missing Legislative District, Postal Code, and Census Tract entries to retain records. However, these are location identifiers, so the filled values may not represent actual locations.

**Electric Range:** The 10 missing values were filled using the median, which was 0. The existing zero values were also retained because they were recorded in the original dataset.

## Final Data Check

- Customer/vehicle records: **289,564**
- Original columns: **16**
- Duplicate records found: **0**
- Missing values after cleaning: **0**
- Existing zero values in Electric Range retained: **188,456**
- Average Electric Range across all records: **37.4 miles**
- Geographic coordinates extracted where location information was available.

## Output

The analysis was performed using:

`Python/Electric_Vehicle_Analysis.ipynb`

The notebook contains the data loading, cleaning, exploratory analysis, and visualizations. The saved charts are available in the `Reports` folder.

**Note:** The dataset did not contain a `Base MSRP` column, so vehicle price analysis could not be performed.