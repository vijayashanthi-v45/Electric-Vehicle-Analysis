
## Business_Insights.md

```markdown
# Business Insights – Electric Vehicle Registration Analysis

## Business Objective

The objective of this analysis was to understand which electric vehicle manufacturers and models had the highest registration counts, identify counties with higher EV registrations, and examine vehicle characteristics and CAFV eligibility.

## Key Business Findings

### 1. Manufacturer Distribution

**Finding:**

- Tesla had the highest number of registrations, with **118,148**.
- Chevrolet ranked second, with **19,808**.
- Nissan, Ford, and Kia were also among the top five manufacturers.

**Business Insight:**

Tesla had a substantially higher registration count than the other manufacturers in this dataset. This indicates that Tesla vehicles represented a large share of the recorded registrations.

### 2. Popular EV Models

**Finding:**

- Tesla Model Y had the highest number of registrations, with **62,979**.
- Tesla Model 3 followed with **38,325**.
- Nissan Leaf, Tesla Model S, and Chevrolet Bolt EV were also among the top five models.

**Business Insight:**

The Model Y and Model 3 were the most common models in the dataset. Businesses can consider these registration patterns when researching customer demand and planning vehicle-related services.

### 3. Regional EV Distribution

**Finding:**

- King County had the highest number of registrations, with **140,130**.
- Snohomish County followed with **36,508**.
- Pierce County had **24,162** registrations.

**Business Insight:**

EV registrations were concentrated in King County compared with the other counties. This makes King County a useful area to examine when evaluating potential locations for EV-related services and charging infrastructure.

### 4. Vehicle Distribution by Model Year

**Finding:**

- Model year 2023 had the highest vehicle count, with **60,332** records.
- Model year 2024 had **49,277** records.
- Model year 2025 had **37,044** records.

**Business Insight:**

The dataset contained a large number of vehicles from recent model years. This describes the distribution of registered vehicles by model year; it should not be interpreted as a direct measure of annual registration growth.

### 5. Electric Range

**Finding:**

- The calculated average Electric Range across all records was **37.4 miles**.
- The dataset contained **188,456 records with zero Electric Range**.
- The average is therefore strongly affected by the zero values.

**Business Insight:**

The overall average does not represent the typical electric range of vehicles with a reported positive range. A separate analysis of valid positive-range records would provide a more meaningful comparison.

### 6. CAFV Eligibility

**Finding:**

- **26.79%** of records were classified as Clean Alternative Fuel Vehicle Eligible.
- **8.13%** were classified as Not Eligible due to Low Battery Range.
- **65.08%** had unknown CAFV eligibility because the battery range had not been researched.

**Business Insight:**

Most records had unknown eligibility. More complete eligibility information would be needed to make stronger comparisons across CAFV categories.

### 7. Electric Range by Make and Model

**Finding:**

- Jaguar had the highest calculated average Electric Range among the makes in the analysis.
- Roadster had the highest calculated average Electric Range among the models in the analysis.

**Business Insight:**

Electric range varied across makes and models. These comparisons should be interpreted with care because zero-range records are included in the calculations.

## Business Recommendations

- Use manufacturer and model registration counts to guide further market research and understand which vehicles are common in the dataset.
- Examine high-registration counties such as King County when evaluating locations for EV-related services.
- Investigate counties with lower registration counts to understand possible factors such as charging infrastructure, vehicle availability, and affordability.
- Improve the completeness of electric-range and CAFV eligibility information before making detailed comparisons.
- Combine registration records with charging-station and population data to develop a broader view of regional EV adoption.

## Conclusion

The analysis identified the most common EV manufacturers and models, the counties with the highest registration counts, and patterns in vehicle model years and CAFV eligibility.

Tesla, Model Y, and King County led their respective registration categories. The findings provide a starting point for market research and regional planning, while the missing and zero values in the dataset highlight the need for more complete information before making further conclusions.