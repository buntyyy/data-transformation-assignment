✅ Approach Summary – Data Cleaning and Transformation (Python Task)
🔹 Task: Clean Sales Data and Compute Total Price
- Loaded raw_sales.csv into a pandas DataFrame.
- Defined reusable UDFs (User-Defined Functions) to clean each column:
    1)  Converted order_id, product_id, quantity to integers.
    2) Converted price_per_unit to float.
    3) Converted order_date to proper datetime format.
    4) Replaced missing values with default values (0, blank, or NaT).
- Created a separate UDF to calculate total_price = quantity * price_per_unit.
- Applied all cleaning and transformation logic using functions (no hardcoding).
- Added a new column total_price and saved the cleaned dataset as cleaned_sales.csv.
