# RIT Dataset — Week 1: Data Cleaning

Week 1 deliverable for the Excelerate Program internship. Covers initial cleaning and preparation of the RIT Opportunity Wise Student Participation dataset.

## Files
| File | Description |
|------|-------------|
| `Data cleaning.ipynb` | Cleaning pipeline |
| `RIT+Opportunity+Wise+Data+-+Sheet1.csv` | Raw dataset |
| `RIT_Cleaned_Dataset.csv` | Cleaned output |

## What Was Done
- Removed duplicates
- Nulled 1,864 malformed timestamps across 3 date columns
- Parsed all date columns to proper datetime format
- Standardised institution name casing (2,089 → 1,818 unique)
- Anonymised 2 records with student IDs in First Name field
- Documented missing values — Start Date nulls are structural (internships)
- Validated Status Code consistency
- Derived `Age_at_Signup` column from DOB and sign-up date

**Final dataset: 8,558 rows × 17 columns**
