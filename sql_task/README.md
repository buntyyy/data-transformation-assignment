 Approach Summary
🔹 Task 1: Detect Added or Removed Products
- Loaded two CSVs (products_day1.csv, products_day2.csv) into DataFrames: df1 and df2.
- Used pandasql to run SQL queries directly on these DataFrames.
- Compared product_ids using NOT IN and UNION to identify:
    i) Products in df1 but not in df2 → labeled as "removed".
    ii) Products in df2 but not in df1 → labeled as "added".

🔹 Task 2: Detect Column-Level Changes
- Focused on matching product_ids present in both df1 and df2.
- Compared key fields (price, stock) to check for value mismatches.
- Used SQL with conditional filtering to extract only the rows where values differ.
- Added a column_changed, old_value, and new_value to show what was updated.


