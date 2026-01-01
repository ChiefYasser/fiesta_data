Project: Supply Chain Analysis with Pandas
1. The Goal
The objective of this project is to analyze a dataset of supply chain operations (supply_chain.csv) to help a company optimize its production. We want to understand manufacturing costs, defect rates, and supplier performance.
2. The Tools
We are using Python with two main libraries:
Pandas: To load the data, filter it, and perform calculations (like an advanced, automated Excel).
Matplotlib: To turn these numbers into visual graphs.
3. Step-by-Step Workflow
Step 1: Data Loading & Inspection
We start by importing the raw CSV file. We check the structure (rows and columns) to ensure the data is clean (no missing values) and understand what variables we are working with (e.g., SKU, Production Volumes, Manufacturing Costs).
Step 2: Cleaning & Filtering
We don't need to look at every single product. We use filtering to focus on critical areas:
Quality Control: We isolate products with a Defect Rate > 3% to identify quality issues.
High Volume: We filter for products with Production Volumes > 500 to see where the factory is busiest.
Step 3: Engineering & Calculation
The raw data isn't enough. We create new metrics (new columns) to get deeper insights:
Total Manufacturing Cost: We multiply the Volume by the Unit Cost to see the total money spent per product.
Estimated Defective Units: We calculate exactly how many items are likely to be broken based on the defect rate.
Step 4: Aggregation (Grouping)
Instead of looking at individual products, we group the data to see the "Big Picture":
By Supplier: We calculate the average defect rate for each supplier to see who is the most reliable.
By Location: We sum up production volumes to see which factory location is producing the most.
Step 5: Visualization
Finally, we generate a Line Graph. We compare the manufacturing costs of the top 3 suppliers (Supplier 1, 2, and 5) to visually analyze how their costs fluctuate across different products.
4. Conclusion
This project demonstrates how data analysis can transform raw logistics numbers into actionable business insights, allowing managers to choose better suppliers and reduce waste.
