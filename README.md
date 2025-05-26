🛒 Retail Dataset – Data Cleaning Summary
📌 About the Dataset
I worked with the Retail dataset of a global superstore, covering a period of four years. This dataset includes details such as orders, customers, products, and sales.

🧹 Data Cleaning Steps
1. Removed Duplicate Rows
Used the Row ID column (a unique identifier) to detect and remove duplicate records.

2. Parsed Order ID
The Order ID column contains three pieces of information:
Country Code (e.g., CA, US)
Year the order was placed
Unique numeric ID
Split the Order ID into separate columns: Country, Year, and Order Number.

3. Filtered Unique Orders
Retained only unique Order IDs after the split.

4. Data Type Conversion
Updated data types appropriately:
Order ID: Number
Order Date, Ship Date: Short Date
Ship Mode: Text

6. Processed Customer ID
The Customer ID contains the initials of the customer's first and last name, followed by a unique number.
Used "Text to Columns" to extract and keep only the unique numeric part of the Customer ID.

6. Standardized Customer Info Columns
Updated data types for:
Customer Name, Segment, Country, City, and State to Text

7. Handled Missing Postal Codes
Filtered for the State: Vermont and City: Burlington.
Found some missing postal codes and replaced them with 0.

8. Parsed Product ID
The Product ID column follows the format: Category-Abbreviation-UniqueID
e.g., FUR-BO-10001798
Split into three parts:
First 3 letters of Category
First 2 letters of Sub-Category
Unique numeric product ID

9. Formatted Sales Amount

Converted the Sales Amount column to Indian Currency Format for consistency and easier interpretation.

✅ Final Output
After these steps, the dataset is clean, structured, and ready for analysis or dashboard reporting.


