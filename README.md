# Deskify Office Supply Co.: Sales and Profit Reporting Dashboard

**Tools:** Power BI, Power Query (M), DAX
**My role:** Data Analyst
**Data:** Sales and transaction data from January 2009 to December 2012: 5,496 orders from 795 customers, $14.74M in revenue.

## Business overview
Deskify Office Supply Co. is a leading retailer of office supplies, technology and computer accessories, and furniture. It serves both individual consumers and businesses, and it has grown significantly over the past four years. The company focuses on reliability, efficiency and customer satisfaction.

## The business problem
Deskify relies on Excel to compile, analyse and report monthly sales and transaction data. As transaction volumes and data complexity have grown, this has become slow and cumbersome. Manual data entry and consolidation from multiple sources introduce errors and inconsistencies into the reports.

## Project aim
Build a data model in Power BI from Deskify's sales and transaction data that centralises the data sources and streamlines data cleaning. By reducing manual work, the project improves the accuracy and efficiency of reporting and provides interactive dashboards for faster, data-driven decisions.

## My role and approach
1. **Centralised the data** 
2. **Cleaned and transformed the data in Power Query:** fixed data types, removed duplicates, handled missing values.
3. **Built the data model:** Data modelling was performed by transforming the flat-file dataset into a star schema consisting of fact and dimension tables. Duplicate records were removed from the dimension tables to ensure that primary keys contained unique values. Relationships were then established between the dimension tables and the fact table, primarily using one-to-many cardinality to support efficient data analysis and reporting.
4. **Created DAX measures:** Total Revenue, Total Profit, Total Orders, Total Customers and Profit Margin (profit divided by revenue). 
5. **Designed two interactive report pages:** a Product Analysis page and a Customer Analysis page, with year and category slicers and navigation buttons so leaders can filter and move between views.


## Key findings
**Overall (2009 to 2012):** $14.74M revenue, $1.52M profit, 5,496 orders, 795 customers and a 10.33% profit margin.

### Product analysis
- **Top locations by profit:** California was the top-performing location, generating a total profit of $2,292,354.46.
- **Profit by category:** Office Supplies contributes $985K (64.7% of profit), Furniture $331K (21.7%) and Technology $206K (13.5%).
- **Shipping method:** Regular Air handles about 74% of orders, followed by Delivery Truck (14%) and Express Air (12%).
- **Top 5 products by profit:** Eldon ClusterMat Chair Mat ($22K), Performers Binder/Pad Holder ($16K), Avery Reinforcements ($15K), Panasonic KX-T7736-B phone ($15K) and Fellowes Bases and Tops ($14K). Together they make up only about 5% of total profit, so profit is spread across many products rather than a few.
- **Profit by month (all years combined):** profit peaks in October ($177K), January ($174K) and September ($167K), and is lowest in August ($81K).

### Customer analysis
- **Segments:** Corporate is the most profitable segment at $527.15K (about 35% of profit), followed by Home Office ($389.66K), Consumer ($310.89K) and Small Business ($294.65k).
- **Regions:** Northwest ($569K) and Nunavut ($341K) together generate about 60% of profit. Quebec ($14K) and Yukon ($6K) contribute the least. Segment performance varies by region. In the Northwest, Home Office ($178K) leads Corporate ($163K).
- **Top 5 customers by profit:** Emily Phan ($34.0K), Deborah Brumfield ($31.1K), Grant Carroll ($28.0K), Karen Carl... ($21.7K) and Alejandro Grove ($20.6K), about 9% of total profit combined.
- **Sub-categories:** Binders ($260K) and Paper ($242K) alone generate about a third of profit. Copiers is the only sub-category making a loss (-$16K).

## Recommendations
1. **Protect the core.** Binders and Paper drive a third of profit, so keep them well stocked and consider bundling them with higher-margin items.
2. **Fix or reconsider Copiers.** It loses money. Review pricing, discounts and costs to decide whether to reprice, renegotiate supplier terms or reduce the range.
3. **Look at Technology.** It contributes only 13.5% of profit. Check whether this is a demand problem or a margin problem before investing.
4. **Focus on regional strengths and gaps.** Protect the Northwest Territories and Nunavut, which carry most of the profit, and investigate why Quebec and Yukon contribute so little (low sales, heavy discounting or high costs).
5. **Build on the Corporate segment.** Corporate is the largest profit source, so offer business accounts, bulk pricing or contracts, while growing Home Office as the strong second segment.
6. **Plan around seasonality.** Prepare stock and staffing for the peaks in September, October and January, and test promotions to lift the August low.
7. **Keep Regular Air reliable.** It carries about three-quarters of orders, so delivery reliability on this option matters most to customers.
8. **Reward top customers without relying on them.** The top 5 customers contribute about 9% of profit, so a loyalty programme would be useful but profit is not dangerously concentrated.

## What I learned
This project strengthened my skills in data modelling, DAX and Power Query, and in designing multi-page, interactive Power BI reports that replace manual Excel reporting with a single trusted source.

## Repository contents
- README.md: this write-up
- data/: the dataset
- dashboard/: screenshots of both report pages
- powerbi/: the Power BI (.pbix) file
