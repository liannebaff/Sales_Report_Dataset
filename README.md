# 👛 Sales Report Dataset Analysis

### 📝 Project Summary
This Power BI project analyses sales data to provide insights into company performance, trends and customer behaviour. The interactive dashboard enables users to explore sales and profit across product categories and segments, countries and years. The aim was to create an interactive reporting tool to support business decision-making and highlight trends in revenue and profit.

🔗 [View dashboard on Power BI online](https://app.powerbi.com/links/GCNBri31iT?ctid=3ea7c128-c601-4479-a003-e14d00c0b5cb&pbi_source=linkShare)

### 🗂️ Dataset Overview
- The dataset consists of two related tables (by Order ID):
  - ListOfOrders: contains general order information with fields such Order ID, Order Date, Segment, Customer Name, Country, City and Ship Date.
  - OrderBreakdown: contains line-item information for each order with fields such as Order ID, Product Name, Discount, Sales, Profit, Quantity and Category.
- The dataset is comprised of sales transactions between 2011 and 2014.
  
### 🎯 Key Skills Demonstrated:
`POWER BI DESKTOP` &nbsp; `POWER BI ONLINE` &nbsp; `POWER QUERY` `DASHBOARD DESIGN` &nbsp; `DASHBOARD INTERACTIVITY` &nbsp; `FILTERS` &nbsp; `SLICERS`

----

### 🧩 Data Preparation
- Power Query was used to review and clean the dataset before loading it into Power BI:
  - Checked for missing values using **Column Quality**, which displays the percentage of _Valid, Error,_ and _Empty_ values for each column.
  - Reviewed value distributions using Column Distribution to identify outliers or unusual patterns.
  - Profiled each column wiith **Column Profile** to verify data types, ranges and unique values.
    
 <img width="1208" height="201" alt="image" src="https://github.com/user-attachments/assets/1bbb5a7a-7250-4569-a0da-56e863620ca4" /> <br>

- Linked ListOfOrders and OrderBreakdown in Power BI **Model View** using Order ID.

---
### 🎨 Dashboard Creation
This section describes the technical work carried out inside Power BI to create the dashboard:

#### 🔎 Filters
- Filters were added to the charts to allow users to focus on specific countries, product categories, segments or time periods.
- Clicking on a visual (e.g., a bar in the stacked bar chart, or a point on the map) acts as a filter, updating all other visuals.
- This ensures the dashboard tells a cohesive story and supports exploratory, interactive analysis.

#### 🖼️ Design & Layout
- Colours were chosen for visual appeal and readability, different colours used on geographic map to more easily differentiate the countries.
- Titles added to each chart for clarity and context.
- A cleam, grid-based layout was used to allow for quick scanning and easy comparison of key metrics.

#### ⬇️ Drill-Downs
- The Sales vs. Profit line graph uses a date hierarchy allowing drill-down from Year → Quarter → Month → Day.
- This enables exploration of trends at multiple time levels, from long-term annual patterns to daily performance.
- Drill-down works in combination with the filters so selecting a category, for instance, will dynamically update the line chart and the other visualisations.

---
### 📊 Dashboard Overview
The dashboard combines multiple visualisations to provide an interactive view of sales performance. The dashboard includes filter controls for exploratory analysis. PDF of dashboard included below.

**1) Total Sales by Category & Segment**
- A stacked bar chart highlighting total sales across each product category and segments.
- Allows easy comparison of category and segment contributions to the total sales.
- Filters for category, segment and total sales (`=sum(sales`) added.

**2) Total Sales and Profit by Year**
- A line chart tracking trends in total sales and profit over time.
- Dual lines (sales vs profit) enable comparison of revenue and profitability trends.
- The chart uses a dual-axis to show both metrics on the same view, allowing a comparison of total sales and profit trends over time, even though the two measures have different magnitudes.
- Includes drill-down from Year → Quarter → Month → Day.

**3) Profit by Country** 
- Geographic map visualising total profit distribution across the countries.
- Each point indicates a country and each colour indicates a continent.
- Filters enable users to focus on specific countries.

**4) Total Profit by Country and Category** (stacked column chart)
- Stacked column chart illustrating how total profit varies across countries and different  product categories, sorted in descending order of profit.
- Each segment of the column represents a product category within that country.
- Enables quick comparison of profit contributions from different categories across countries.

<img width="1324" height="760" alt="image" src="https://github.com/user-attachments/assets/d724b25d-28f5-42f5-8ec2-3f770f12a3a6" />

🖱️ [Open Sales Report PDF](Sales_Report_Dashboard_PDF.pdf) | 🔗
[View dashboard on Power BI online](https://app.powerbi.com/links/GCNBri31iT?ctid=3ea7c128-c601-4479-a003-e14d00c0b5cb&pbi_source=linkShare)

----
### 🪞 Insights & Reflections
- The highest-performing category was Technology and the lowest-performing category was Furniture, the highest-performing segment across all categories was the consumer segment.
- The United Kingdom generated the largest total profit was obtained, followed by Germany and France. The Netherlands was the lowest-performing market, recording a loss.
- Total sales and profit show a steady increase from 2011 to 2014.
- The dashboard allows users to quickly identify trends, compare categories and assess regional profitability.
- A limitation with the dataset is that it does not include customer demographics, marketing spend and inventory data, which limits deeper analysis of sales drivers.
- Future improvements could include forecasting and profit margin analysis.

---
### 📁 Files in This Repository  
- **[Sales_Report_Dashboard_PDF](Sales_Report_Dashboard_PDF.pdf)**
- **[Sales_Dataset.xlsx](Sales_Dataset.xlsx)**
  
  **Worksheet(s):**
  - **ListOfOrders:** contains general order information. 
  - **OrderBreakdown:** contains line-item information for each order. <br> <br>
  
### 📋 Dataset Structure

**Table 1: ListOfOrders**

| Column Name   | Description                                            |
| ------------- | ------------------------------------------------------ |
| Order ID      | Unique identifier for each order                       |
| Order Date    | Date when the order was placed                         |
| Customer Name | Name of the customer                                   |
| City          | City of the customer                                   |
| Country       | Country of the customer                                |
| Region        | Geographic region of the customer                      |
| Segment       | Customer type (e.g., Consumer, Corporate, Home Office) |
| Ship Date     | Date when the order was shipped                        |
| Ship Mode     | Shipping method (e.g., Standard, Express)              |
| State         | State or province                                      |
| lon           | Longitude coordinate of the city                       |
| lat           | Latitude coordinate of the city                        | 

<br>

**Table 2: OrderBreakdown**

| Column Name  | Description                                     |
| ------------ | ----------------------------------------------- |
| Order ID     | Unique identifier linking to Table 1            |
| Product Name | Name of the product ordered                     |
| Discount     | Discount applied to the order                   |
| Sales        | Revenue from the order                          |
| Profit       | Profit from the order                           |
| Quantity     | Number of units sold                            |
| Category     | Product category (e.g., Furniture, Electronics) |
| Sub-category | Product sub-category                             |




