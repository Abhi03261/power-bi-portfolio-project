Here’s a polished, GitHub‑ready README description for your Power BI data‑modelling project. I’ve shaped it to sound clear, professional, and aligned with best practices—something you can drop straight into your repository.

📊 Power BI Data Modelling: Star Schema, Merge Queries & Active/Inactive Relationships
This project demonstrates a clean and scalable Power BI data‑modelling approach using industry‑standard best practices. It focuses on building a Star Schema, performing query transformations, and managing multiple date relationships (Order Date vs Shipping Date) using the active/inactive relationship concept.

⭐ Star Schema Design
The data model follows a Star Schema structure to ensure:
- High performance
- Simplified DAX
- Clear separation of facts and dimensions
Model Components
- Fact Table: Sales/Orders fact containing metrics such as quantity, sales amount, and two date fields (Order Date & Shipping Date)
- Dimension Tables:
- Date Dimension
- Customer Dimension
- Product Dimension
- Other lookup tables as needed
This structure improves report performance and supports intuitive analytics.

🔄 Merge Queries (Power Query)
Power Query is used to:
- Clean and transform raw data
- Merge fact and dimension tables where necessary
- Ensure consistent keys for relationships
- Standardize date formats and lookup fields
This step ensures the model is reliable and ready for relationship building.

🔗 Active vs Inactive Relationships (Multiple Date Fields)
The fact table contains two different date fields:
- Order Date
- Shipping Date
Since Power BI allows only one active relationship between two tables, the model uses:
- Active relationship: Order Date → Date Dimension
- Inactive relationship: Shipping Date → Date Dimension
To use the inactive relationship in measures, the model applies the DAX function:
