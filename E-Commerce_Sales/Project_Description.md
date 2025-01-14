# E-Commerce Sales Overview Dashboard
## *Visualization in Power BI*
*PowerBI file and the dataset is provided in the repository*. 

## About the Dataset
The dataset used for this project was sourced from <a href= "https://www.kaggle.com/datasets/apoorvaappz/global-super-store-dataset">Kaggle</a> and includes details of online orders placed worldwide between January 1, 2011, and December 31, 2014. It consists of 51,290 rows and 24 columns, providing an overview of global e-commerce sales during this period.

## Visualization Workflow
The dashboard was developed in Power BI, adhering to the following workflow:
## 1. Data Transformation
 - Verified data cleanliness and checked datatypes.
 - Derived **Dimension Tables** for Calendar, Product, Region, and Segment from the **Master Table** to support visualization.
## 2. Data Modeling
Designed a **Star Schema Data Model** with one-to-many relationships between the *Master Table* and *Dimension Tables*.
## 3. DAX Calculations
Key measures for analysis and visualization were calculated using DAX:
 - **Gross Sales, Profit, and Shipping Cost**: Calculated using SUMX() function.
 - **Order Count and Customers Count**: Derived using COUNTX() and DISTINCTCOUNT().
 - **Rank of Product Sub-Categories**: Ranked based on the order of contribution to metrics such as Total Profit, Total Sales, and Profit Margin using RANKX().
## About the Dashboard Visuals
## 1. Navigation Panel
 - A navigation panel on the left side allows users to filter visuals by Product Segment, Year, Quarter, Market, Country, and Product Category.
## 2. Top-Level Metrics
 - Displays overall sales metrics: **Gross Sales, Shipping Cost, Profit, Number of Customers, and Number of Orders**, with disaggregation options by Year, Quarter, Segment, Market, Country, and Product Category.
## 3. Sales Key Metrics
Highlights top-performing product sub-categories by **Sales amount, Profit, Contribution to Gross Sales and Profit, as well as Profit Margin**. Notably, products are ranked primarily based on their profit margin, emphasizing the importance of profitability as a critical metric for e-commerce business. This approach enables a more nuanced assessment of product performance, highlighting that high sales and profit figures alone do not necessarily equate to profitability. By focusing on profit margins, the business can make informed decisions to refine pricing strategies and improve overall financial outcomes.
## 4. Sales Amount vs Profit Margin Matrix
To further analyze the relationship between sales amount and profit margin, I developed a visual representation that highlights the profitability and sales performance of each product group. This visualization is inspired by the "Menu Engineering" concept, commonly used in the restaurant industry to compare the profitability and popularity of menu items for revenue optimization.

Applying this concept to e-commerce, the matrix plots **sales amount** on the X-axis and **profit margin** on the Y-axis. The visualization is divided into four quadrants using **average sales amount** (vertical line) and **average profit margin** (horizontal line) as thresholds. Each dot represents a product sub-category, color-coded based on its category.

## Matrix Quadrants:
 - **Stars**: High sales and high profit margins—these are the most desirable products.
 - **Plowhorses**: High sales but low profit margins—strategies may be needed to improve profitability.
 - **Puzzles**: Low sales but high profit margins—focus on strategies to boost sales.
 - **Dogs**: Low sales and low profit margins—these products may require restructuring or removal.

This visual provides actionable insights for decision-makers to optimize the product portfolio, prioritize high-profitable products, and make strategic adjustments to maximize overall sales amount and profitability.

*The Dashboard image*

![Sales_Dashboard](https://github.com/user-attachments/assets/fd9d5990-8376-4ab9-9eeb-b1514cfa46e9)
