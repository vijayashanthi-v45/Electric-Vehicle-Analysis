# Data Dictionary – Electric Vehicle Registration Analysis

## Dataset Information

- **Dataset:** `export.csv`
- **Total Records:** 289,564
- **Original Columns:** 16
- **Duplicate Records:** 0
- **Source Folder:** `Dataset/Raw/`

## Column Definitions

| Column | Description |
|---|---|
| VIN (1-10) | First 10 characters of the Vehicle Identification Number. |
| County | County where the vehicle is registered. |
| City | City where the vehicle is registered. |
| State | State associated with the vehicle registration. |
| Postal Code | Postal or ZIP code of the registration location. |
| Model Year | Model year of the vehicle. |
| Make | Vehicle manufacturer or brand. |
| Model | Vehicle model name. |
| Electric Vehicle Type | Type of electric vehicle: Battery Electric Vehicle (BEV) or Plug-in Hybrid Electric Vehicle (PHEV). |
| Clean Alternative Fuel Vehicle (CAFV) Eligibility | Indicates the recorded CAFV eligibility status of the vehicle. |
| Electric Range | Estimated distance the vehicle can travel using electric power, measured in miles. |
| Legislative District | Legislative district associated with the registration location. |
| DOL Vehicle ID | Vehicle record identifier assigned by the Department of Licensing. |
| Vehicle Location | Geographic location represented as coordinate text. |
| Electric Utility | Electric utility provider associated with the vehicle's location. |
| 2020 Census Tract | Census tract associated with the registration location. |

## Additional Columns Created During Analysis

| Column | Description |
|---|---|
| VIN_Anonymized | Numeric label created from the first 10 VIN characters using Pandas factorization. It is a replacement label, not secure anonymization. |
| Longitude | Longitude value extracted from the Vehicle Location coordinate text. |
| Latitude | Latitude value extracted from the Vehicle Location coordinate text. |

## Important Dataset Notes

- The dataset contains **289,564 records** and **16 original columns**.
- The `Base MSRP` column is not available.
- There are no duplicate records.
- The original dataset contains missing values in several columns.
- A large number of records have zero Electric Range.
- The CAFV eligibility field includes an unknown category.
- Additional columns were created during analysis for VIN labeling and geographic coordinates.