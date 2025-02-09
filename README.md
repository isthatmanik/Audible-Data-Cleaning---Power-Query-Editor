# Audible Dataset Cleaning and Standardization using Power Query Editor

This project demonstrates how to use Power Query Editor in Excel to clean and standardize an Audible dataset. The goal is to prepare the dataset for further analysis by ensuring data consistency and formatting. The following tasks are accomplished:

## Tasks

1. **Standardize Name Column**
   - Convert names in the "name" column to title casing to ensure consistent capitalization.

2. **Separate Combined Author Names**
   - Split combined first and last names in the "author" column into separate columns for first and last names.

3. **Consistent Date Formatting**
   - Ensure all entries in the "releasedate" column follow a consistent date format (DD-MM-YYYY).

4. **Convert Time Column**
   - Change the time column from text format to a duration format that Excel recognizes.

5. **Numeric Price Column**
   - Ensure the "price" column is in a numeric format. Identify and address any non-numeric values.

6. **Convert Text Ratings to Numeric**
   - Convert text ratings in the "stars" column to numeric values for easier analysis.

7. **Split NarratedBy Column**
   - Separate the "narratedby" column into multiple columns if it contains multiple narrators.

8. **Merge Releasedate and Language**
   - Combine the "releasedate" and "language" columns into a new column named "releaseinfo" with the format "DD-MM-YYYY, Language."

9. **Format Currency Values**
   - Ensure all currency values in the "price" column are formatted consistently with two decimal places.

## Steps to Clean and Standardize the Dataset

1. **Open Power Query Editor**
   - Load your dataset into Power Query Editor in Excel.

2. **Standardize Name Column**
   - Select the "name" column, use the "Transform" tab, and apply the "Capitalize Each Word" transformation.

3. **Separate Combined Author Names**
   - Select the "author" column, use the "Split Column" feature to divide by delimiter (if space or comma), and rename columns as "First Name" and "Last Name."

4. **Consistent Date Formatting**
   - Select the "releasedate" column, use the "Change Type" feature, and set the data type to "Date" ensuring the format is set to DD-MM-YYYY.

5. **Convert Time Column**
   - Select the "time" column, use the "Transform" tab to convert text to a duration format by changing the type to "Duration."

6. **Numeric Price Column**
   - Select the "price" column, ensure it is in a numeric format. Use the "Detect Data Type" feature to find and correct any non-numeric values.

7. **Convert Text Ratings to Numeric**
   - Create a new column with numeric ratings by mapping text values to numbers using the "Add Column" feature and "Custom Column" with an appropriate formula.

8. **Split NarratedBy Column**
   - Select the "narratedby" column, use the "Split Column" feature based on delimiter (e.g., comma) to create multiple columns.

9. **Merge Releasedate and Language**
   - Use the "Add Column" feature to create a new column "releaseinfo" by combining the "releasedate" and "language" columns with a custom formula.

10. **Format Currency Values**
    - Select the "price" column, use the "Transform" tab to set the format to a numeric type with two decimal places.

## Final Steps

- **Apply Changes**
  - Click "Close & Load" to apply changes and load the cleaned dataset back into Excel.

- **Verify Data**
  - Review the dataset to ensure all transformations have been applied correctly and the data is ready for analysis.
